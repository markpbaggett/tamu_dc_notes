Environmental Scan: Services and Technology
===========================================

About
-----

This document attempts to define and document the various services that inform the workings of the digital library.

While specific microservices may be covered or explored, this document attempts to center on the functions of the
various software rather than the software themselves.

Digital Assets Management
-------------------------

IIIF
----

==========
IIIF Image
==========

The `IIIF (International Image Interoperability Framework) Image Service <https://iiif.io/api/image/3.0/>`_ is a
standard and a set of APIs designed to facilitate the sharing, accessing, and viewing of images from various
repositories in a consistent and interoperable way. It provides a standard API for accessing image content, which allows
different systems to retrieve images in a consistent manner and supports dynamic delivery of images, enabling users to
request images at different sizes, qualities, and formats without needing to store multiple versions of the same image.

While the API has many features, its most important features and purposes are related to image manipulation,
interoperability, deep zooming, and scalability and efficiency.

Currently, we use `Cantaloupe <https://cantaloupe-project.github.io/>`_ as our IIIF Image Server. It is available
online `here <https://api.library.tamu.edu/iiif/2/>`_. Our image server uses IIIF Image 2.0 and adheres to level 2 of
the specification.  While level 2 is not complete, it is defined as desirable. Currently, Cantaloupe serves images from
Fedora and DSPACE.

The most important outcome of an image server is that it adheres to the things defined in its response in a performant
way.

Here are the results of several requests and processing times with an image from DSPACE.

* `Get image response <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/info.json>`_: 58 milliseconds
* `Get full image as jpg on largest size <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/full/0/default.jpg>`_: 4.36 seconds
* `Get next lower resolution version <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/1108,/0/default.jpg>`_: 3.54 seconds
* `Get mid <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/554,/0/default.jpg>`_: 2.00 seconds
* `Get lowest in original state <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/69,/0/default.jpg>`_: 1.47 seconds
* `Grab full image with 516 width, rotate it 90 degrees, return as GIF <https://api.library.tamu.edu/iiif/2/ddabcc96-0637-38ba-b2fe-0baf58efa8b0/full/516,/90/default.gif>`_: 1.93 seconds
* `Grab full image, rotate it 180 degrees, return as PNG, and grayscale <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/full/180/gray.png>`_: 6.16 seconds
* `Grab image at 50 pct <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/full/pct:50/0/default.jpg>`_: 3.24 seconds
* `Grab a small region <https://api.library.tamu.edu/iiif/2/6d8552af-83dd-3897-846b-aa71695e36bc/10,75,75,800/full/0/default.jpg>`_: 1.45 seonds

============================================
Presentation of Works with IIIF Presentation
============================================

The IIIF (International Image Interoperability Framework) `Presentation API <https://iiif.io/api/presentation/3.0/>`_ is
a specification designed to enable the structured presentation of digital objects in a way that supports rich user
interactions and interoperability between different systems. The API supports advanced viewing capabilities, such as
zooming, panning, and page-turning and builds upon the IIIF Image API to do this. While primarily focused on images, the
IIIF Presentation API can also support other media types, such as audio and video, enabling the presentation of diverse
digital objects. It is also designed to integrate with the W3C Web Annotation framework so that resources can be annotated
and displayed to tell unique stories about a work.

IIIF Presentation is enabled by a manifest that describes how a viewer should display a work. Because the API is interoperable,
IIIF viewers are interchangeable.  For instance, here is the :code:`Geological Survey (United States)` manifest from our
repository in 4 different viewers:

* `Clover <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Fdspace%2Fpresentation%2F1969.1%2F2808>`_
* `Theseus <https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/2808>`_
* `Mirador <https://projectmirador.org/embed/?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/2808>`_
* `Universal Viewer <https://uv-v3.netlify.app/#?c=&m=&s=&cv=&manifest=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Fdspace%2Fpresentation%2F1969.1%2F2808&xywh=-391%2C-116%2C2558%2C2309>`_
* `Glycerine <https://demo.viewer.glycerine.io/viewer?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/2808>`_

IIIF Presentation and manifests are provided by `IRIIIFService <https://github.com/TAMULib/IRIIIFService>`_. This application
works with resources hosted in either DSPACE or Fedora and adheres to IIIF Presentation 2.0. This version of the API only
supports images. IIIF Presentation 3.0 allows resources to include AV.  For instance, here is:

* `An audio work with a transcript from my previous institution <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://digital.lib.utk.edu/assemble/manifest/wwiioh/2248>`_
* `A video work with a closed captioning in Spanish and English from my previous institution <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://digital.lib.utk.edu/assemble/manifest/rfta/168>`_
* `A compound work from my previous institution with an image in the first canvas and a video with closed captions in the second canvas <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://digital.lib.utk.edu/assemble/manifest/rftaart/75>`_

Like with images, there are many IIIF viewers that support video.  For instance, here is:

* `A video work from my previous institution with closed captioning in Spanish and English and segmented interview questions <https://ramp.avalonmediasystem.org/?iiif-content=https://digital.lib.utk.edu/assemble/manifest/rfta/168>`_

Ideally, all works served via digital collections would have a corresponding manifest that is informed by its work type.
Doing so ensures the best presentation of our resources and encourages the reuse of digital collections in research and
other creative activity. It also allows us to easily reuse an asset from any digital collection in an exhibit.

For instance, let's look at the Galston Studienbuch exhibit from my previous institution by clicking the
:code:`Explore the Volume` button and launching the modal.

.. raw:: html

   <iframe src="https://exhibits.lib.utk.edu/galston/" width="750" height="600"></iframe>

These are annotations added by researchers that allow users to explore the multiple Works and see specific information.
This helps tell an important story about this unique collection and does so without changing the underlying work.

Additionally, let's look at the `Letter, Dom Lynch in New York N.Y. to Ebenzer Hazard.,1793 July 5 <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fdigital.lib.utk.edu%2Fassemble%2Fmanifest%2Finsurancena%2F181>`_.
This resource has accompanying annotations of the handwritten text that is searchable and displayable.

------
IRIIIF
------

IRIIIF is a Spring backend for the Institutional Repository International Image Interoperability Framework (IRIIIF) Service
developed and maintained by Texas A&M University Libraries. This service provides IIIF manifest generation for works in
OakTrust and from Fedora. IRIIIF supports single and multicanvased works, but since it is based of IIIF Presentation v2,
does not support AV.

One interesting thing that this service seems to be able to do is build canvases in a manifest from pages in a PDF. This
means that an ETD and other PDF works should be able to be served in a IIIF viewer with a modern viewing experience.

Redis is used for manifest cache and resource URL caching. There are still many things I need to learn about this service
including:

1. When a Manifest is generated, how long is it cached for in Redis?
2. Can a Manifest be regenerated on demand via a HTTP get parameter ( :code:`?update=true` )?
3. How are manifests from DSPACE RDF informed? For instance, how does IRIIIF know sequence order?
4. Does IRIIIF assume all files on a work need to be delivered as canvases? In other words, if a work has a PDF, jp2s, and jpgs, do all get rendered as canvases?
5. When a new collection goes online, are manifests generated and cached or is that done on demand? If the latter, what if the work has 2000 pages?

--------------
OCR and Search
--------------

How is OCR presented?

---------------------------------
Transcription of Handwritten Text
---------------------------------

Handwritten text is present in some works found in our repositories. Historically, handwritten text has been costly for
Libraries, Archives, and Museums to transcribe in order to make works more searchable, understandable, and useful. At
previous institutions I have worked at, there was a history of text encoding with TEI. This required humans to interpret
the text, transcribe it, and encode it as well formed XML and valid TEI. This was a costly process but it provided an
easy approach to present the work with IIIF annotations:

.. raw:: html

   <iframe src="https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://digital.lib.utk.edu/assemble/manifest/burford/155" width="750" height="600"></iframe>

At Texas A&M, a different approach has been taken. Rather than transcribe the resources in house, pilots with
`From the Page <https://fromthepage.com/>`_ have been pursued. FromThePage is an open-source tool that allows
volunteers to collaborate to transcribe handwritten documents rather than having all the work be done in house. With
From the Page, a work or collection is imported as IIIF Manifests.  Each page is then loaded from the providing institution
as IIIF Image resources and volunteers transcribe the work according to guidelines created by the providing institution.

At any point after the transcription begins, the providing institution can export a project as HTML, plain text, CSV,
TEI, IIIF, or another export format. The export format chosen greatly affects the interoperability of the resource. For
instance, `TEI from the Houston Oil Minutes Project <https://fromthepage.com/export/minutes-of-houston-oil-company-of-texas-b1bc1655-1b0c-4947-8144-c0f657acebb4/tei>`_
easily provides the transcription in a format that many TEI powered platforms (like TEI Publisher) can import and use.
The `IIIF export <https://fromthepage.com/iiif/52425/manifest>`_ includes an annotation list that can be opened in viewers
like `Mirador <https://projectmirador.org/embed/?iiif-content=https://fromthepage.com/iiif/52425/manifest>`_ or
`Theseus <https://theseus-viewer.netlify.app/?iiif-content=https://fromthepage.com/iiif/52425/manifest>`_.

.. code-block:: json

      "otherContent": [
        {
          "@id": "https://fromthepage.com/iiif/1692120/list/transcription",
          "@type": "sc:AnnotationList",
          "label": "Transcription"
        }
      ]


