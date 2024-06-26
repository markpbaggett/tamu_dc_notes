Initial Priorities
==================

- Create Guiding Principles for Digital Collections and Vet Broadly
    - Listen to stakeholders
    - Preservation
    - Collection Development
    - Digital Assets Management
    - Restrictions
    - Interoperability
    - Discoverability
    - Accessibility
    - Project Management
    - Collections as Data
- Create decision tree for DAMS selection
    - When does something go to OakTrust
    - When does something go to Fedora
    - When does something go to OpenONI
    - When does something go to Avalon
    - If something is delivered with something else (Cervantes, IA Bookreader), where are files and works managed
    - Are OpenONI / Avalon files stored directly in those platforms
- Understand Current Landscape and Microservices that make up the DAME
    - What gets a graph in Fuseki and DSPACE
        - `Cushing Exhibition Catalogs <https://oaktrust.library.tamu.edu/rdf/handle/1969.1/160506>`_ (collection with graph)
        - `Primeros Liberos <https://oaktrust.library.tamu.edu/rdf/handle/1969.1/92213>`_ (collection no graph)
        - Any Djatoka driven resource (no graph)
    - Figure out how ordering of canvases work from both DSPACE and Fedora
        - `Fedora example <https://spotlight.library.tamu.edu/spotlight/london-collection/catalog/d46adeb610031a28bf682e4f68817128>`_
        - `DSPACE <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Fdspace%2Fpresentation%2F1969.1%2F94147>`_
    - What collections exist and how do they work
    - What are the microservices and how do they work together
    - Understand and document how Solr is implemented for Collections and Works
        - Document
    - Understand OAI-PMH and where it's available
    - How long is a manifest cached in REDIS / IRIIIFService
        - How long will this be cached for
- Increase accessibility, usability, and discoverability of collections
    - Create plan to add closed captioning for existing video collections
    - Create transcripts / audio descriptions for existing audio collections
    - Determine pathway and document how to get transcriptions from From the Page
    - Document existing content models and how IIIF presentation is informed
    - Collaborate with stakeholders and developers to document needs and content models for new works
    - Propose a single search interface based on underlying Solr
    - Understand OAI-PMH and where it's available
    - Advocate for `Implementation of FAIRiCat <https://signposting.org/FAIRiCat/>`_ where possible
    - Create standards for access copies and intermediate files
- Increase trust in Digital Collections platforms
    - Make sure all OakTrust links are over HTTPS (are any right now?)
