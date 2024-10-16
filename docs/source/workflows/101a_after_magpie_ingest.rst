Post MagPie Tasks
=================

After MagPie runs, there a few things you need to do.

Since we've moved to Rancher from Chef, Solr documents don't get automatically written to fcrepo's Solr instance. As a
result, you must trigger it by shelling into fcrepo and posting this HTTP request:

.. code-block:: shell

    curl -X POST http://localhost:9080/reindexing -H "Content-Type: application/json" -d '["broker:queue:solr.reindex"]'

You can then watch the logs to make sure every thing is running well like so:

.. code-block:: shell

    # karaf log:
    tail -f /usr/local/karaf/data/log/karaf.log
    ls -al /usr/local/karaf/data/log/

You can also generate a Collection manifest like so:

.. code-block:: shell

    curl  https://api-pre.library.tamu.edu/iiif-service/fedora/collection/bb/97/f2/3e/bb97f23e-803a-4bd6-8406-06802623554c/london-maps-batch-2-jamess-test
