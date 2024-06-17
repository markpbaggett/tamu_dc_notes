Environmental Scan: Content Models
==================================

About
-----

This page attempts to describe how works are modeled in RDF at TAMU.

In some instances, properties have been removed to make the graph simpler and more easily understandable.

For items with the concept of "Children", a note with an example is included in addition to the graph.

Charting Texas
--------------

Charting Texas is a collection in Fedora that does not seem to have multiple canvases.  This is added for comparisons to
a collection with works with multiple canvases.

==========
Collection
==========

This is the collection with drastically reduced member objects.

**Children**:

* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas/members`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas> rdf:type ldp:Container, fedora-repo:Resource, ldp:RDFSource, fedora-repo:Container, pcdm:Object ;
        fedora-repo:writeable "true" ;
        fedora-repo:created "08-25-22 11:37 AM", "fedoraAdmin";
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/41> .

=========
A "Child"
=========

This is a graph of a child according to CAP. Some notes:

* The namespace used for :code:`ore` is wrong and not dereferenceable.  It should be :code:`https://www.openarchives.org/ore/terms/`.
* :code:`ore:proxyFor` is a property that should be used as linking and not the object of the triple.  I'm not sure yet what they are attempting to express with :code:`ldp:insertedContentRelation ore:proxyFor .`.

**Children**:

* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas/members/10Proxy`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas/members> a ldp:Container, ldp:RDFSource, pcdm:Object, fedora-repo:Resource, ldp:IndirectContainer, fedora-repo:Container ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:insertedContentRelation ore:proxyFor ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas> .

=========
A "Proxy"
=========

This is a graph of a child according to CAP. Some notes:

* The namespace used for :code:`ore` is wrong and not dereferenceable.  It should be :code:`https://www.openarchives.org/ore/terms/`.

**Children**:

* None

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas/members/10Proxy> a pcdm:Object, ldp:RDFSource ,ldp:Container, fedora-repo:Container, fedora-repo:Resource ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ore:proxyFor <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10> .

===========
An "Object"
===========

This is a graph of an Object according to CAP. Some notes:

* The namespace used for :code:`dce` is wrong and not dereferenceable.  It should be :code:`http://purl.org/dc/elements/1.1#`.

**Children**:

* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/orderProxies`
* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/pages`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10> a ldp:RDFSource, pcdm:Object, ldp:Container, fedora-repo:Resource, fedora-repo:Container;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        iana:first <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/orderProxies/page_0_proxy> ;
        iana:last <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/orderProxies/page_0_proxy> ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/:25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/pages/page_0> ;
        dce:format "reformatted digital", "application/tif" ;
        dce:language "eng" ;
        dce:description "Date of object estimated by library to be 1842. Held in the Floyd and Louise Chapman Texas and Borderlands Collection at Cushing Memorial Library and Archives on the campus of Texas A and M University, College Station, Texas." ;
        dce:title "Message from the President of the United States, in relation to the boundary between the United States and the Republic of Texas, January 20, 1842." ;
        dce:identifier "1214433" ;
        dce:rights "A copyright review process in April 2022 has determined that this particular item is in the public domain. http://rightsstatements.org/vocab/NoC-US/1.0/" ;
        dce:subject "Texas--History--Republic--1836-1846", "United States--Foreign Relations--Texas" ;
        dce:creator "United States - President (1841-1845: Tyler)" ;
        dcterms:type "Text" ;
        dcterms:lcc "F390 .U7 1842" ;
        dcterms:issued "[1842]?" ;
        dcterms:spartial "Texas", "United States" .

=================
An "orderProxies"
=================

**Children**:

* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/orderProxies/page_0_proxy`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/orderProxies> a fedora-repo:Resource, ldp:Container, ldp:RDFSource, ldp:DirectContainer, fedora-repo:Container , pcdm:Object ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10> ;
        ldp:isMemberOfRelation ore:proxyIn .

=========
A "pages"
=========

**Children**

* :code:`tamu-repo:3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/pages/page_0`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10/pages> a fedora-repo:Container, ldp:DirectContainer, ldp:Container, pcdm:Object, ldp:RDFSource, fedora-repo:Resource ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/charting-texas_objects/10> ;
        ldp:hasMemberRelation pcdm:hasMember .

Stephen Powys Marks London Collection
-------------------------------------

Stephen Powys Marks London Collection is a collection in Fedora that has works with multiple canvases.  This is added
for comparison to a collection without works with multiple canvases.

=====================================
Stephen_Powys_Marks_London_Collection
=====================================

This collection is interesting as it an `Stephen_Powys_Marks_London_Collection_objects` are direct descendants of the
Cushing Collections.

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection/members`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection> a fedora-repo:Container, ldp:Container, ldp:RDFSource, pcdm:Object, fedora-repo:Resource ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/5> .

=============================================
Stephen_Powys_Marks_London_Collection_objects
=============================================

Like, Stephen_Powys_Marks_London_Collection, this is a direct descendant of Cushing Collections.

Children here are different in that they point to CAP URIs rather than graphs.

**Children**:

* :code:`https://library.tamu.edu/cap/rv/Production-Fedora?context=3b%2F6f%2Fc3%2F25%2F3b6fc325-f6ca-41d8-b91e-8c5db3be8c13%2FStephen_Powys_Marks_London_Collection_objects%2F4`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects> a fedora-repo:Container, ldp:Container, ldp:IndirectContainer, pcdm:Object, fedora-repo:Resource, ldp:RDFSource ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection>;
        ldp:insertedContentRelation ore:proxyFor ;
        ldp:hasMemberRelation pcdm:hasMember .

================================================
Child of "Stephen_Powys_Marks_London_Collection"
================================================

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection/members/10Proxy`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection/members> a ldp:Container, ldp:IndirectContainer, fedora-repo:Resource, pcdm:Object, ldp:RDFSource, fedora-repo:Container ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection> ;
        ldp:insertedContentRelation ore:proxyFor ;
        ldp:hasMemberRelation pcdm:hasMember .

======================
Child Proxy of Members
======================

**Children**:

* None

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection/members/10Proxy> a ldp:RDFSource, fedora-repo:Container, pcdm:Object, fedora-repo:Resource, ldp:Container ;
        ore:proxyFor <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10> ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" .

=========
An object
=========

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies`
* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10> a pcdm:Object, ldp:RDFSource, fedora-repo:Resource, ldp:Container, fedora-repo:Container ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        iana:first <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies/page_0_proxy> ;
        iana:last <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies/page_28_proxy> ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_21>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_18>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_25>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_6>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_27>, <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_13> ;
        dce:publisher "London, J. Taylor", "DIGITAL: Cushing Memorial Library and Archives" ;
        dce:format "Reformatted digital" ;
        dce:subject "Architecture--England--London", London (England)--Description and travel", "NA970 .B8 1825" ;
        dce:title "Illustrations of the public buildings of London; with historical and descriptive accounts of each edifice" ;
        dce:rights "https://rightsstatements.org/page/NoC-US/1.0/?language=en" ;
        dce:description "Two volumes published between 1825 and 1828; Added title-pages, engravings." ;
        dce:creator "Britton, John (1771-1857)" ;
        dce:language "en" ;
        dce:type "Map" ;
        dcterms:medium "Electronic" ;
        dcterms:extent "2 volumes : illustrations, plates, map ; 23 centimeters" ;
        dcterms:isPartOf "Stephen Powys Marks London Collection" ;
        dcterms:created "1825" .

============
orderProxies
============

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies/page_0_proxy`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies > a ldp:RDFSource, fedora-repo:Container, ldp:Container, ldp:DirectContainer, fedora-repo:Resource, pcdm:Object ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        fedora-repo:lastModified "08-25-22 11:37 AM", "fedoraAdmin" ;
        ldp:isMemberOfRelation ore:proxyIn ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10> ;

==========
page proxy
==========

**Children**:

* None

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies/page_0_proxy> a pcdm:Object, ldp:RDFSource, fedora-repo:Resource, ldp:Container, fedora-repo:Container ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        ore:proxyFor <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_0> ;
        ore:proxyIn <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10> .


=====
pages
=====

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_0`
* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages> a fedora-repo:Container, ldp:RDFSource, ldp:Container, ldp:DirectContainer, fedora-repo:Resource, pcdm:Object ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10> .

==============
page with File
==============

**Children**:

* :code:`https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1/files`

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1> a pcdm:Object, ldp:RDFSource, fedora-repo:Resource, fedora-repo:Container, ldp:Container ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        ldp:hasMemberRelation pcdm:hasMember ;
        pcdm:hasFile <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1/files/londonmaps_2858014_01.tif> .

======
A File
======

Files has a Resource instead of Children in CAP.

.. code-block:: turtle

    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix fedora-repo: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix tamu-repo: <https://api.library.tamu.edu/fcrepo/rest/> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix dce: <http://purl.org/dc/elements/1.1/> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1/files> a ldp:RDFSource, fedora-repo:Container, ldp:Container, ldp:DirectContainer, pcdm:Object, fedora-repo:Resource ;
        fedora-repo:createdBy "fedoraAdmin" ;
        fedora-repo:created "fedoraAdmin", "08-25-22 11:37 AM" ;
        fedora-repo:writeable "true" ;
        fedora-repo:lastModifiedBy "fedoraAdmin" ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/pages/page_1> .

