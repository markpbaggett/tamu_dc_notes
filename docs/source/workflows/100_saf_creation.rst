SAF Creation
============

SAF Creator, or Simple Archive Format Creator, is a tool used to build import packages for DSpace.  It is also used for
creating packages for FCRepo.

To get started, you first need to `download SAF Creator <https://github.com/TAMULib/SAFCreator>`_. From here you can clone
and build with mvn or download and prebuild jar.

Once you've built or downloaded the jar, you can run like so:

.. code-block:: shell

    java -jar ~/link/to/saf_creator.jar

Initial SAF Settings
--------------------

Once SAF Creator is running, you need to give it a few things. First, it needs a metadata CSV file that describes each
work. Fields in the csv must match DSpace style fieldnames (e.g. dc.creator).  It's not clear currently what is allowed
here, but from looking at other existing sheets it looks like any `DublinCore Elements <http://purl.org/dc/elements/1.1/>`_
or `DCTERMS <http://purl.org/dc/terms/>`_ property. Namespacing must be done with a period rather than a colon.

Files are added via an additional :code:`filename` column.  All fields can have multiple values by separating with double
pipe characters (e.g. :code:`file_1.jpg||file_2.pdf` ).

To add your CSV, simple click **Select metadata CSV file**.

Once you've created and added your CSV, you'll need to point at the files related. To do that, click **Select source files directory**.

Now, you must choose where to write your package, to do that click **Select SAF output directory**.

Now, click **Load specfied batch now**.

Verifying Batch
---------------

Once you've loaded your batch, you must verify it.  Click **Batch Verificaiton**.

Then click **Verify Batch**.

Creating Package
----------------

After validation passes, go back to **Batch Details** and click **Create**.
