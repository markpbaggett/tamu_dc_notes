Environmental Scan: Content Models
==================================

About
-----

This page attempts to describe how works are modeled in RDF at TAMU.

In some instances, properties have been removed to make the graph simpler and more easily understandable.

For items with the concept of "Children", a note with an example is included in addition to the graph.

Concepts
--------

==========
Collection
==========

Collection resources currently look like this:

.. code-block:: turtle

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:04:02.645000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13> ;
        fedora:lastModified "2024-10-15T21:04:02.645000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/10>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/11>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/12>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/13>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/15>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/16>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/17>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/18>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/19>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/2>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/20>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/21>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/22>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/23>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/24>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/25>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/26>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/27>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/4>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/5>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/6>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/7>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/8>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/9> ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members> .

=======
Members
=======

The :code:`Collection` resource points at a :code:`Members` resource via :code:`ldp:contains`. The :code:`Members` resource
contains a list of proxies for each work:

.. code-block:: turtle

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:IndirectContainer,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:04:02.645000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion> ;
        fedora:lastModified "2024-10-15T21:05:12.628000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/10Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/11Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/12Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/13Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/15Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/16Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/17Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/18Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/19Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/20Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/21Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/22Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/23Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/24Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/25Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/26Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/27Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/2Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/3Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/4Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/5Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/6Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/7Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/8Proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/9Proxy> ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:insertedContentRelation <http://www.openarchives.org/ore/terms#proxyFor> ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion> .

============
Work Proxies
============

Each work has a corresponding proxy.  As far as I can tell, these proxies do not include :code:`iana` properties and thus
are not used for ordering works in a collection.

.. code-block:: turtle

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix ns1: <http://www.openarchives.org/ore/terms#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members/3Proxy> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion/members> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ns1:proxyFor <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> .

=====
Works
=====

Every :code:`Work` is described by a resource.  The work, points at its parts via a :code:`pcdm:hasMember` property. Each
work has a :code:`fedora:hasParent` relationship to the :code:`Collection Objects` resource. It does not point at the
:code:`Collection` resource directly. Each work has :code:`iana:first` and :code:`iana:last` properties that point at the
first and last proxy in a work for sequencing. The work has a :code:`ldp:contains` property that points at its :code:`Pages`
resource and its :code:`orderProxies` resource.

.. code-block:: turtle
    :emphasize-lines: 16, 79-82, 20-65

    @prefix dc: <http://purl.org/dc/elements/1.1/> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        pcdm:hasMember <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_0>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_1>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_10>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_11>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_12>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_13>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_14>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_15>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_16>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_17>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_18>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_19>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_2>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_20>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_21>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_22>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_23>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_24>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_25>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_26>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_27>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_28>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_3>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_30>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_31>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_32>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_33>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_34>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_35>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_36>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_37>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_38>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_39>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_4>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_40>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_41>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_42>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_43>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_44>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_45>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_5>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_6>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_7>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_8>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_9> ;
        dc:creator "Blumberg, Stephen Carrie" ;
        dc:description "From the professional archives of Nicholas A. Basbanes, now held by Cushing Memorial Library & Archives, Texas A&M University." ;
        dc:format "reformatted digital" ;
        dc:language "eng" ;
        dc:rights "In copyright - Educational Use Permitted; For more information see:  http://rightsstatements.org/vocab/InC-EDU/1.0/" ;
        dc:subject "Blumberg, Stephen Carrie",
            "Book thefts",
            "Bookplates",
            "Collectibles" ;
        dc:title "Scrapbook of Stolen Bookplates. Volume Two." ;
        dc:type "Albums (Books)" ;
        dcterms:abstract "The bookplates collected here were removed by Stephen Blumberg from volumes he stole and arranged geographically into these blank pages. In addition to being trophies of his many exploits, however, the bookplates provided valuable documentary evidence to suggest whence the books had been stolen. The present volume is one of three such scrapbooks, which were presented to Basbanes following the end of the trial. Ironically, many personal bookplates bear warnings against book-theft and levy curses upon those who borrow but do not return." ;
        dcterms:type "StillImage" ;
        iana:first <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_0_proxy> ;
        iana:last <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_45_proxy> ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages> .

==================
Collection Objects
==================

Each Collection has a :code:`Collection Objects` resource. It acts a proxy for the Collection, but does not have :code:`iana`
properties allowing the collection to be ordered in a list of other collections. It has a :code:`ldp:contains` property
that points at all the works in the collection. It has a :code:`ldp:membershipResource` that points at the collection it
is a proxy for:

.. code-block:: turtle
    :emphasize-lines: 18-42, 45

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:IndirectContainer,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:04:02.645000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13> ;
        fedora:lastModified "2024-10-15T21:05:12.034000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/10>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/11>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/12>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/13>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/15>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/16>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/17>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/18>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/19>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/2>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/20>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/21>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/22>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/23>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/24>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/25>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/26>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/27>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/4>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/5>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/6>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/7>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/8>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/9> ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:insertedContentRelation <http://www.openarchives.org/ore/terms#proxyFor> ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion> .


============
orderProxies
============

Each :code:`Work` has a corresponding :code:`orderProxies` resource.  This resource :code:`ldp:contains` all proxies in
the work. It has a :code:`fedora:hasParent` relationship and a :code:`ldp:membershipResource` that refers to the parent
work.

.. code-block:: turtle
    :emphasize-lines: 14, 18-63, 65

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:DirectContainer,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_0_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_10_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_11_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_12_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_13_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_14_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_15_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_16_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_17_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_18_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_19_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_1_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_20_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_21_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_22_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_23_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_24_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_25_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_26_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_27_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_28_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_29_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_2_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_30_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_31_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_32_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_33_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_34_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_35_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_36_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_37_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_38_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_39_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_3_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_40_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_41_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_42_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_43_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_44_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_45_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_4_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_5_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_6_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_7_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_8_proxy>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_9_proxy> ;
        ldp:isMemberOfRelation <http://www.openarchives.org/ore/terms#proxyIn> ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> .



=====
Pages
=====

Each work has a :code:`Pages` resource.  This resource lists all the parts / pages in a work. It has :code:`fedora:hasParent`
and :code:`ldp:membershipResource` properties that point at the parent work. It also has a :code:`ldp:contains` property
that lists all the pages / parts in a work.

.. code-block:: turtle
    :emphasize-lines: 14, 18-63, 65

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:DirectContainer,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_0>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_1>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_10>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_11>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_12>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_13>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_14>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_15>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_16>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_17>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_18>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_19>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_2>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_20>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_21>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_22>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_23>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_24>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_25>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_26>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_27>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_28>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_3>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_30>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_31>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_32>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_33>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_34>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_35>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_36>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_37>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_38>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_39>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_4>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_40>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_41>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_42>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_43>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_44>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_45>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_5>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_6>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_7>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_8>,
            <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_9> ;
        ldp:hasMemberRelation pcdm:hasMember ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> .

======
A Page
======

Every part or page of a work is described by a :code:`Page` resource. It has a :code:`fedora:hasParent` property that
refers to a work's :code:`Pages` resource. It has a :code:`ldp:contains` property that refers to the work's :code:`Files`
resource and a :code:`pcdm:hasFile` resource that refers to the actual file resource:

.. code-block:: turtle
    :emphasize-lines: 13, 17, 18

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        pcdm:hasFile <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files/Blumberg-Bookplates-Volume-two_30.jpg> ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files> .

=======
A Proxy
=======

Every page or part has a corresponding :code:`Proxy` for the part.  This resource is critical in that it allows the work's
canvases to be ordered. It does this via properties from :code:`iana`.  The :code:`iana:prev` property (if present), lists
the preceding canvas while the :code:`iana:next` property (if present) lists the following canvas.  If one is missing, that
signifies the proxy is first or last in a sequence. The :code:`ore:proxyFor` property refers to the page or part the :code:`Proxy`
represents and the :code:`ore:proxyIn` property refers to the work it belongs to. It also has a :code:`fedora:hasParent`
property that refers to the :code:`orderProxies` resource it belongs to.

.. code-block:: turtle
    :emphasize-lines: 19-22, 15

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix ore: <http://www.openarchives.org/ore/terms#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_29_proxy> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        iana:next <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_30_proxy> ;
        iana:prev <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/orderProxies/page_28_proxy> ;
        ore:proxyFor <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29> ;
        ore:proxyIn <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3> .

=====
Files
=====

Each page or part has a :code:`Files` resource.  This has a :code:`ldp:contains` property that points at the file this
represents. It also has a :code:`ldp:membershipResource` and a :code:`fedora:has Parent` that points at the page or part it belongs to.

.. code-block:: turtle
    :emphasize-lines: 14, 18, 20

    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files> a fedora:Container,
            fedora:Resource,
            pcdm:Object,
            ldp:Container,
            ldp:DirectContainer,
            ldp:RDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        ldp:contains <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files/Blumberg-Bookplates-Volume-two_30.jpg> ;
        ldp:hasMemberRelation pcdm:hasFile ;
        ldp:membershipResource <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29> .

========
The File
========

Every :code:`File` has a corresponding resource that describes it.  While things point directly at the file, the resource
is available by appending :code:`/fcr:metadata` to the end of the URI. This resource has many properties about the file itself.
It has a :code:`iana:describedBy` property that points at the rdf resource of the file. It also has a :code:`fedora:hasParent`

.. code-block:: turtle
    :emphasize-lines: 17, 24

    @prefix dc: <http://purl.org/dc/elements/1.1/> .
    @prefix fedora: <http://fedora.info/definitions/v4/repository#> .
    @prefix iana: <http://www.iana.org/assignments/relation/> .
    @prefix ldp: <http://www.w3.org/ns/ldp#> .
    @prefix ns1: <http://www.ebu.ch/metadata/ontologies/ebucore/ebucore#> .
    @prefix ns2: <http://www.loc.gov/premis/rdf/v1#> .
    @prefix pcdm: <http://pcdm.org/models#> .
    @prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files/Blumberg-Bookplates-Volume-two_30.jpg> a fedora:Binary,
            fedora:Resource,
            pcdm:File,
            ldp:NonRDFSource ;
        fedora:created "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:createdBy "fedoraAdmin" ;
        fedora:hasFixityService <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files/Blumberg-Bookplates-Volume-two_30.jpg/fcr:fixity> ;
        fedora:hasParent <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files> ;
        fedora:lastModified "2024-10-15T21:07:15.097000+00:00"^^xsd:dateTime ;
        fedora:lastModifiedBy "fedoraAdmin" ;
        fedora:writable false ;
        dc:filename "Blumberg-Bookplates-Volume-two_30.jpg" ;
        ns1:filename "Blumberg-Bookplates-Volume-two_30.jpg" ;
        ns1:hasMimeType "image/jpeg" ;
        iana:describedby <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/BasbanesEternalPassion_objects/3/pages/page_29/files/Blumberg-Bookplates-Volume-two_30.jpg/fcr:metadata> ;
        ns2:hasMessageDigest <urn:sha1:e268fa174a6a15f29ddf7858a5d5ecaeb7aaaf45> ;
        ns2:hasSize "789886"^^xsd:long .

Examples
--------

--------------
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

-------------------------------------
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
        dce:subject "Architecture--England--London", "London (England)--Description and travel", "NA970 .B8 1825" ;
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

    <https://api.library.tamu.edu/fcrepo/rest/3b/6f/c3/25/3b6fc325-f6ca-41d8-b91e-8c5db3be8c13/Stephen_Powys_Marks_London_Collection_objects/10/orderProxies> a ldp:RDFSource, fedora-repo:Container, ldp:Container, ldp:DirectContainer, fedora-repo:Resource, pcdm:Object ;
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

Visualizing Current Practices
-----------------------------

If useful, here is a visualization of a simple collection with 1 collection, 1 work, and 1 file.  For ease of reading, excess
classes and literal relationships have been removed.

.. image:: ../_static/images/1_collection_1_work_1_file_just_relationships.png
