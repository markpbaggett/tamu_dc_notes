Ingesting with MagPie
=====================

Once you have a package from SAF Creator, you can ingest it into MagPie.

To begin, `download MagPie <https://github.com/TAMULib/MagpieService>`_.

If needed, modify the yaml to fit your needs or leave as default:

.. code-block:: text

    src/main/resources/application.yml

Configuring Your Project
------------------------

To get started, you need to modify :code:`project.json` to know about your project. This file is found at:

.. code-block:: text

    src/main/resources/config/projects.json

Copy an existing property of this object.

.. code-block:: json

    "london-maps-batch-2-jamess-test":{
            "ingestType":"SAF",
            "isHeadless":true,
            "repositories": [{
            # Name your collection.
            "name": "London Maps Batch 2",
            "type": "FEDORA_PCDM",
            "settings": [{
                "key": "repoUrl",
                "values": [
                    # Change to "https://api.library.tamu.edu" for PROD
                    "https://api-pre.library.tamu.edu"
                ]
                },
                {
                "key": "restPath",
                "values": [
                    "fcrepo/rest"
                ]
                },
                {
                "key": "containerPath",
                "values": [
                    # Change to PROD's containerPath as needed.
                    # Find here: https://api.library.tamu.edu/fcrepo/rest/
                    "bb/97/f2/3e/bb97f23e-803a-4bd6-8406-06802623554c/london-maps-batch-2-jamess-test"
                ]
                },
                {
                "key": "userName",
                "values": [
                    "fedoraAdmin"
                ]
                },
                {
                "key": "password",
                "values": [
                    # Change to PROD's password as needed.
                    "<PRE's password>"
                ],
                "protect": true
                }
            ]
            }],
            "authorities":[
            ],
            "suggestors":[
            ],
            "metadata":[
            ]
        },

You should set:

* The parent property to something unique
* The :code:`name` property to match the colleciton
* The :code:`settings[0].values[0]` property to match the fcrepo instance
* The :code:`containerPath` to match an existing container and concatenate a unique string to the end
* set user name and password based on Rancher env variables

Running
-------

Assuming you have Java, mvn, and JAVA_HOME set properly, you can start the application with :code:`mvn spring-boot:run`.

You are up and running when you see this message:

.. code-block:: text

    INFO 446 --- [           main] e.tamu.app.observer.FileMonitorManager
        : Starting monitor
    INFO 446 --- [MessageBroker-1] e.t.app.observer.FileObserverRegistry
        : File monitor health check
    INFO 446 --- [MessageBroker-2] o.s.w.s.c.WebSocketMessageBrokerStats
        : WebSocketSession[0 current WS(0)-HttpStream(0)-HttpPoll(0), 0 total,
         0 closed abnormally (0 connect failure, 0 send limit, 0 transport error)],
          stompSubProtocol[processed CONNECT(0)-CONNECTED(0)-DISCONNECT(0)],
           stompBrokerRelay[null], inboundChannel[pool size = 0, active threads = 0,
            queued tasks = 0, completed tasks = 0], outboundChannel[pool size = 0,
             active threads = 0, queued tasks = 0, completed tasks = 0],
              sockJsScheduler[pool size = 2, active threads = 1, queued tasks = 2,
               completed tasks = 2]

Copying SAF Creator Package into Monitored Projects
---------------------------------------------------

Now copy your package described in properties to :code:`target/classes/static/metadatatool/projects`.

The package much match the property you defined.

MagPie should now start reporting progress to :code:`stdout`.

Errors are written to :code:`logs/magpie-service.log`.
