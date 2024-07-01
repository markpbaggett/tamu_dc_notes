Environmental Scan: Collections
===============================

=========================================================================
150 Years and Counting: Celebrating 150 Years of the City of Bryan, Texas
=========================================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/bryan-150-exhibit>`_

26 works including images and postcards to commemorate the founding of the city of Bryan. While most of the site is
delivered with Spotlight, there is an interactive map component delivered using ArcGIS' StoryMaps (not KnightLabs
StoryMap). The interactive map is added as an iframe and an associated dedicated site in StoryMaps also exists and is
linked.

While there are postcards, they seem to be only the fronts and not treated as compound objects.

.. raw:: html

   <iframe src="https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Ffedora%2Fpresentation%2F3b%2F6f%2Fc3%2F25%2F3b6fc325-f6ca-41d8-b91e-8c5db3be8c13%2Fbryan-150_objects%2F15" width="750" height="600"></iframe>

**Stack**

* Fedora: for digital assets management
* Cantaloupe: for Image Service
* IIIF Presentation: for Work Presentation
* Mirador: for Viewer
* Spotlight: for Exhibit Building
* `StoryMaps (ArcGIS) <https://storymaps.arcgis.com/stories/8f7ea1d1287c4a23be85cd1d363ad868>`_: for Georeferencing and story telling

**Questions**

* Do we have the full postcards or only the verso?
* What if StoryMaps went away?  Does navPlace make sense for presentation and storing the geographic metadata in the DAMS like we would descriptive metadata?

**IIIF**

* Current: Image, Presentation, Mirador
* Future: navPlace

**Curator or Stakeholder**


======================================
1940s Brazos County Aerial Photographs
======================================

`Homepage <https://library.tamu.edu/collections/maps/brazos-maps.php>`_

This collections consists of a series of aerial photographs that have been indexed using a highway map from 1980. The
images themselves appear to be flat JPGs with no image server.

The primary access point is an image map split into 3 regions. Once you click on a specific region, a new image map
appears. Clicking on each image map renders the corresponding jpg in the window.

**Stack**

* Unclear

**Questions**

* What is this platform?
* Who georeferenced this?
* Are the assets in a DAMS?
* What if this was georectified in something like StoryMap and exported as IIIF?

**IIIF**

* Current: None
* Future: Image, Presentation, navPlace, `geoReference <https://iiif.io/api/extension/georef/>`_

===========================================================
Amazing, Fantastic, Weird: Science Fiction Studies in Texas
===========================================================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/92159>`_

This is a collection of program and proceedings from the exhibit opening of: One Hundred Years Hence: Science Fiction
and Fantasy at Texas A & M. It consists of PDFs, Powerpoints, etc. This is a complex collection that I need to learn
more about. It doesn't fit easily into a IIIF framework.

**Stack**

* DSPACE

**IIIF**

* Current: None
* Future: Unclear

===========================
A.M.C. Yell Book Collection
===========================

`Homepage <https://library.tamu.edu/collections/digital-library/yell_books.php>`_

The Agricultural and Mechanical College of Texas Yell Book Online Collection consists of bound Yell Books dating from
1904-1905 through 1931-1932. Included in the booklets are yells and songs that reflect the unique experience of cadets
during this period, and the businesses that supported the printing of the booklets. Most of the booklets in this
collection were owned by former students, so names, doodles, and in some cases homemade yells can be seen on the covers
and within the booklets' pages.

This is served with the Internet Archive Bookreader Application thus some assumptions are made about stack.

**Stack**

* Internet Archive Bookreader
* Unclear about DAMS or where files are stored

**Questions**

* Where are files stored? Are they in a DAMS? If not, how are they programatically accessed?
* What's the alure of InternetArchive Bookreader instead of IIIF Presetation with viewingHint or Behavior of paged?

**IIIF**

* Current: None
* Future: Image, Presentation, Paged Behavior, IIIF Viewer

=========================================================
Audio Interviews from the Nicholas A. Basbanes Collection
=========================================================

`Homepage <https://proxy.library.tamu.edu/login?url=https://avalon-library-tamu-edu.srv-proxy1.library.tamu.edu/collections/w3763676r>`_

This collection contains digitized audio interviews conducted by Nicholas A. Basbanes in the course of writing his
books, articles, and editorial features. Interviewees include prominent authors, librarians, scholars, and other figures
in the world of books.

The collection is restricted to on campus only.

There are no transcripts.

**Stack**

* Avalon

**Questions**

* Was there ever interest in transcripts for navigation?

**IIIF**

* Current: None
* Future: IIIF Presentation, RAMP or Clover

=====================================
Stephen F. Austin’s 1830 Map of Texas
=====================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/austin-map>`_

This first edition of Stephen F. Austin’s 1830 Map of Texas is often described as “the first meaningful map of Texas”
and was the first to accurately depict the rivers in Texas and illustrate many of the early settlements including
Brazoria, Gonzales, Harrisburg, Matagorda, Victoria and Waco Village.

This map was published in eight editions through 1845 and is the first map of Texas printed in the United States. The
map was produced as part of a land grant agreement with the Mexican government but it was also intended to be a
showcase for new settlers to Texas. Therefore, it was made to be as open and as inviting as possible.

The map is split into 7 parts and each part is presented independently from the other parts.

There is a Georeferenced data package that is served over HTTP from OAKTrust and thus blocked.  This should minimally
be switched to HTTPS.

**Stack**

* Spotlight
* Cantaloupe
* iRIIIFService
* Mirador
* OakTrust for Georeferenced Dataset

**Questions**

* What does the dataset look like?

**IIIF**

* Current: Image, Presentation, Mirador
* Future: navPlace, `geoReference <https://iiif.io/api/extension/georef/>`_

=================================================
The Berger-Cloonan Collection of Decorated Papers
=================================================

`Homepage <https://library.tamu.edu/discovery/discovery-context/berger-cloonan?direction=ASC>`_

The Berger-Cloonan Collection of Decorated Papers contains more than 20,000 items representing five centuries of paper
production and decoration from across the globe and is one of the most extensive collections of its kind. Among its many
strengths are eighteenth-century Dutch gilt papers, thousands of unique marbled and paste papers, Japanese Chiyogami and
Katazome, historic watermarks, and scores of papermakers’ sample books.

The collection was built by Dr. Sidney E. Berger and Dr. Michèle V. Cloonan in support of their research and teaching
interests, and was acquired by Texas A&M University Libraries in 2016. This digital collection contains non-copyrighted
papers in the Berger-Cloonan Collection. It is offered here as a starting point for students and researchers who wish to
become acquainted with the collection. Digitization of the collection is ongoing, and high-resolution scans of papers
will be uploaded as they become available.

Each work is served as a single canvas with manifests.

There are no context pages and only an index.

**Stack**

* SAGE
* Cantaloupe
* iRIIIFService
* Mirador

**Questions**

* If this is SAGE, how are context pages added? Can they be added?

**IIIF**

* Current: Image, Presentation, Mirador
* Future: Similar

===============================================
The Bibliography of Science Fiction and Fantasy
===============================================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/6316>`_

The bibliographic control of Science Fiction and Fantasy has a long and storied history, from its beginnings in the 1930s to the online tools of today. The works in this collection range from superb productions that serve as best practice standards to quick-and-dirty listings. Virtually all of the entries add a bit to the coverage of the field.

The collection appears to consist of 9 works that are all PDFs.

**Stack**

* DSPACE

**Questions**

* Need to look at more deeply

**IIIF**

* None

===================================================
Charting Texas: A History of the State Through Maps
===================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/charting-texas>`_

This exhibition features maps and books, documenting several centuries of exploration and political competition for one
specific area of North America — Texas. With advancements in geographic knowledge, surveying techniques, and printing
technology, one can begin to see Texas taking its now familiar form from the earliest depictions in the 16th Century.

The collection consists of 57 items that are mostly maps.

**Stack**

* Spotlight
* Cantaloupe
* iRIIIFService
* Mirador

**Questions**

* Have any maps been georeferenced?

**IIIF**

* Current: Image, Presentation
* Future: navPlace, `geoReference <https://iiif.io/api/extension/georef/>`_

=========================
Colección Los Palabristas
=========================

`Homepage <https://proxy.library.tamu.edu/login?url=https://avalon-library-tamu-edu.srv-proxy2.library.tamu.edu/collections/xs55mc14f>`_

Colección Los Palabristas is a collection of 650+ radio interviews with writers and artists from Mexico, South and Central America, and Spain. The interviews were originally broadcast between 1979 and 2002 as episodes of the Buenos Aires-based radio program, Los Palabristas. A collection of original recordings were acquired from Argentinian journalist and host Esteban Peicovich in 2005 by the Department of Hispanic Studies and the University Libraries.

There are no transcripts.  Some works are done as a `playlist <https://avalon-library-tamu-edu.srv-proxy2.library.tamu.edu/media_objects/41687h652>`_.

**Stack**

* Avalon

**Questions**

* Was there ever interest in transcripts for navigation?
* What about English translations?
* What protocol is used for restrictions?

**IIIF**

* Current: None
* Future: IIIF Presentation, RAMP or Clover

=================================
College of Medicine Class Rosters
=================================

The College of Medicine class roster photos connect today to the past and are made available online through a
partnership between the College of Medicine and the University Libraries.

**Stack**

* SAGE
* Cantaloupe
* iRIIIFService
* Mirador

**Questions**

* If this is SAGE, how are context pages added? Can they be added?

**IIIF**

* Current: Image, Presentation, Mirador
* Future: Similar

===============================================
College Of Veterinary Medicine Image Collection
===============================================

`Homepage <https://library.tamu.edu/discovery/discovery-context/cvm-images?direction=ASC>`_

Over the past 100 years, photographers have documented the history of the College of Veterinary Medicine & Biomedical
Sciences. This collection highlights the changing face of the people, technology, and facilities of the college. It
spans the history from the earliest undergraduate classes in veterinary science in the 1890s to the cutting edge
research of the 21st Century. Thanks to the contributions of generous former students and faculty, and the efforts of
various historians and archivists, the images found here, if not complete, are a fair representation of the growth and
development of Veterinary Medicine at Texas A&M.

There are 1491 Works here.

**Stack**

* SAGE
* Cantaloupe
* iRIIIFService
* Mirador

**Questions**

* If this is SAGE, how are context pages added? Can they be added?

**IIIF**

* Current: Image, Presentation, Mirador
* Future: Similar

===========================
Cushing Exhibition Catalogs
===========================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/160506>`_

Collection of catalogs from Cushing Memorial Library & Archives exhibits. All seem to be PDFs.

**Stack**

* DSPACE

**Questions**

* Need to look at more deeply
* What might serving this with Clover or UV look like?

**IIIF**

* None

====================================
Cushing Historical Images Collection
====================================

The Cushing Memorial Library and Archives maintains an extensive photographic collection of over 300,000 images. The collection continues to grow. These images are in a wide variety of formats and sizes, including negatives on glass plates, post cards, and various early types of prints. The collection is organized by subject and contains a visual representation of nearly every aspect of Texas A&M University’s long and storied past beginning with the opening of the school in 1876. Categories include such subjects as campus views, individual buildings, athletics, research, teaching, student life, members of the faculty, visiting dignitaries, and important events. Most of the photographs were acquired through donation or from various units of the university.

Please note that this collection is under construction and some images are missing. These images can be found in the corresponding Flickr collection that mirrors this collection: http://www.flickr.com/photos/cushinglibrary/collections/72157616848695613/

This is split into many collections and subcollections and almost everything appears to be JPG.

Here is a sample of three presidential visit collections merged and served in Canopy.

.. raw:: html

   <iframe src="https://markpbaggett.github.io/tamu-presidential-visits" width="750" height="600"></iframe>


**Stack**

* DSPACE

**Questions and Thoughts**

* Need to review.

**IIIF**

* Image and Presentation

===================================
Electronic Theses and Dissertations
===================================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/1>`_

This collection includes digitized theses and dissertations (1922-2004) and theses and dissertations directly deposited
after 2004.

**Stack**

* DSPACE

==========================================
The Frederick C. Cuny/INTERTECT Collection
==========================================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/159819>`_

Frederick C. Cuny was an American humanitarian and preeminent disaster relief specialist who worked to improve the lives of people affected by natural and man-made disasters around the world. Over his 26 year career, Cuny worked in crises in more than fifty countries, including Biafra, Guatemala, Bangladesh, Cambodia, India, Iraq, Kuwait, Somalia, Bosnia, and Chechnya. His larger than life personality, uncanny ability to “make things happen,” and his innovative ideas drove him to the forefront of the disaster response field.

The collection contains the working library, office files, press clippings, slides, photographs and Beta and VHS tapes of Cuny and his team at the disaster relief/response firm, Intertect, and at the non-profit organization he co-founded in 1987, the Intertect Institute. The items currently digitized represent a small section of the collection chosen for their significance by members of the Cuny Center for the Study of Societies in Crisis.

This appears to be a mix of PDFs and JPGs.

.. raw:: html

   <iframe src="https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/160086" width="750" height="600"></iframe>

**Stack**

* DSPACE

**Questions and Thoughts**

* Parts of this should be driven by IIIF.  Is it?
* How does IRIIIFService serve IIIF from DSPACE? Ah! https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/160086
* Need to review.

**IIIF**

* Image and Presentation where possible

===================================
Geologic Atlas of the United States
===================================

A set of 227 folios published by the U.S. Geological Survey between 1894 and 1945. Each folio includes both topographic
and geologic maps for each quad represented in that folio, as well as descriptions of the basic and economic geology of
the area. The Geologic Atlas collection is maintained by the Maps unit.

This is the first collection I've seen with compound works as IIIF. It looks like these are served from DSPACE via an
API at https://api.library.tamu.edu/iiif-service/dspace/presentation.

.. raw:: html

   <iframe src="https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/2808" width="750" height="600"></iframe>

On closer inspection, it appears that the IIIF service makes use of the SPARQL served from `here <https://oaktrust.library.tamu.edu/rdf/handle/1969.1/2808>`_:

.. code-block:: turtle

    @prefix void:  <http://rdfs.org/ns/void#> .
    @prefix rdf:   <http://www.w3.org/1999/02/22-rdf-syntax-ns#> .
    @prefix xsd:   <http://www.w3.org/2001/XMLSchema#> .
    @prefix dcterms: <http://purl.org/dc/terms/> .
    @prefix bibo:  <http://purl.org/ontology/bibo/> .
    @prefix foaf:  <http://xmlns.com/foaf/0.1/> .
    @prefix dspace: <http://digital-repositories.org/ontologies/dspace/0.1.0#> .
    @prefix dc:    <http://purl.org/dc/elements/1.1/> .

    <https://oaktrust.library.tamu.edu/rdf/resource/1969.1/2808>
            dspace:hasBitstream        <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/24/001pg08.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/4/001pg08.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/7/001pg05.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/17/001pg01.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/12/001insidefrontcover.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/13/001frontcover.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/26/GFolio001.zip> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/22/001pg06.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/25/001pg09.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/8/001pg04.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/5/001pg07.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/14/001backcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/1/GFolio001.pdf> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/18/001pg02.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/6/001pg06.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/23/001pg07.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/3/001pg09.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/19/001pg03.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/9/001pg03.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/16/001insidefrontcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/10/001pg02.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/20/001pg04.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/11/001pg01.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/21/001pg05.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/15/001frontcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/2/001backcover.tif> ;
            dspace:isPartOfCollection  <https://oaktrust.library.tamu.edu/rdf/resource/1969.1/2490> ;
            dc:date                    "2012-06-01T22:02:19Z"^^xsd:dateTime , "2005-12-01T21:36:07Z"^^xsd:dateTime ;
            dc:format                  "109947612 bytes" , "110574680 bytes" , "109797024 bytes" , "17586214 bytes" , "110608596 bytes" , "110535360 bytes" , "111346436 bytes" , "108709108 bytes" , "106885740 bytes" , "application/pdf" , "109609844 bytes" , "108326004 bytes" , "109371844 bytes" , "image/tiff" , "109275132 bytes" ;
            dc:language                "en-US" ;
            dc:publisher               "Geological Survey (United States)" ;
            dc:rights                  "No copyright; for more information see: https://rightsstatements.org/page/NoC-US/1.0/" ;
            dcterms:available          "2005-12-01T21:36:07Z"^^xsd:dateTime , "2012-06-01T22:02:19Z"^^xsd:dateTime ;
            dcterms:hasPart            <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/5/001pg07.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/9/001pg03.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/18/001pg02.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/3/001pg09.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/6/001pg06.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/22/001pg06.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/4/001pg08.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/20/001pg04.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/21/001pg05.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/7/001pg05.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/26/GFolio001.zip> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/25/001pg09.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/10/001pg02.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/2/001backcover.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/12/001insidefrontcover.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/15/001frontcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/24/001pg08.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/19/001pg03.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/14/001backcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/11/001pg01.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/17/001pg01.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/13/001frontcover.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/16/001insidefrontcover.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/8/001pg04.tif> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/23/001pg07.jpg> , <https://oaktrust.library.tamu.edu/bitstream/1969.1/2808/1/GFolio001.pdf> ;
            dcterms:isPartOf           <https://oaktrust.library.tamu.edu/rdf/resource/1969.1/2490> ;
            dcterms:issued             "1894" ;
            dcterms:rights             <https://rightsstatements.org/page/NoC-US/1.0/> ;
            dcterms:title              "Livingston folio, Montana." ;
            bibo:uri                   <https://hdl.handle.net/1969.1/2808> ;
            void:sparqlEndpoint        <https://fuseki.library.tamu.edu/dspace/sparql> ;
            foaf:homepage              <https://oaktrust.library.tamu.edu> .

It's not clear from here whether canvases are derived from :code:`dcterms:hasPart`, :code:`dspace:hasBitstream`, or something else.

**Stack**

* DSPACE
* Cantaloupe
* iRIIIFService
* Mirador

**Questions and Thoughts**

* How does IRIIIFService leverage RDF or something else to order sequences and canvases?
* What about the PDFs in DSPACE? What happens with those? (see turtle above)

**IIIF**

* Image and Presentation where possible

============================================================
The Sandy Hereld Memorial Digitized Media Fanzine Collection
============================================================

`Homepage <https://oaktrust.library.tamu.edu/handle/1969.1/149935>`_

The Sandy Hereld Collection consists of thousands of digitized images of media fanzines, letterzines, and club
newsletters, dating from the late 1960s through materials published online or in print in 2013. The collection is an
unparalleled assembly of media fanworks that document generations of fans’ continued creative engagement with media
productions meaningful to them. Among the productions chronicled particularly well in the Hereld Collection are: Beauty
and the Beast (1987-1990), Blake’s 7, Doctor Who, The Professionals, Star Trek, Star Wars, and Starsky & Hutch. But the
collection also contains fanzines relating to numerous other productions, such as the Harry Potter book/movie series,
Due South, Miami Vice, Simon & Simon, and many others. Also in the collection are many anthologies of stories from
multiple fandoms.

This collection must be viewed on campus or via the VPN. It appears to consist entirely of PDFs.

**Stack**

* DSPACE

**Questions and Thoughts**

* ?

**IIIF**

* ?

===================================================================
Hernán Contreras & Gerald Griffin Collection of NASA A/V Recordings
===================================================================

`Homepage <https://avalon.library.tamu.edu/collections/sf268521w>`_

This collection contains digitized video and audio from the Hernán Contreras ’62 Collection of NASA Events Film Reels
and the Gerald D. “Gerry” Griffin ’56 Collection of NASA Video and Audio Recordings. Contreras was an In-flight Design
Specialist for Lockheed and later worked for United Space Alliance, a spaceflight operations company co-owned by
Rockwell International and Lockheed Martin. Griffin served as a Flight Director during the Apollo Missions and later as
Director of the Johnson Space Center in Clear Lake, TX. The original audio cassette tapes, VHS tapes, and/or 16 mm films
for both the Contreras and Griffin Collections are housed at Cushing Memorial Library & Archives.

Unlike most other Avalon collections, this is not restricted.

There are no Closed Caption Files even though some items `like this <https://avalon.library.tamu.edu/media_objects/v118rd703>`_
have an audio codec.

**Stack**

* Avalon

**Questions and Thoughts**

* Should we generate closed captions?
* If we were to upgrade Avalon, we'd get IIIF.
* For now, maybe it'd be worth building out a IIIF recipe around one of these as proof of concept.
* Are files delivered with Avalon stored in Avalon?

**IIIF**

* Current: None
* Future: Presentation

=======================
Historical Maps of Cuba
=======================

`Homepage <https://library.tamu.edu/discovery/discovery-context/tamu-cuba-maps?direction=ASC>`_

This collection contains digital versions of historical maps of Cuba held by the Texas A&M University Libraries. Subject
matter includes soils and population.

There are 39 items. Many of the maps include a corresponding :code:`KML` that supplements the item loaded in the viewer.
The KMLs I've seen thus far are relatively simple and only contain and initial starting location for where to associate
the map with lat / long coords:

.. code-block:: xml

    <?xml version="1.0" encoding="UTF-8"?>
    <kml xmlns="http://www.opengis.net/kml/2.2" xmlns:gx="http://www.google.com/kml/ext/2.2" xmlns:kml="http://www.opengis.net/kml/2.2" xmlns:atom="http://www.w3.org/2005/Atom">
    <NetworkLink>
        <name>Cuba 1943</name>
            <LookAt>
                <longitude>-79.5</longitude>
                <latitude>22.5</latitude>
                <altitude>0</altitude>
                <range>1250000</range>
                <tilt>0</tilt>
                <heading>0</heading>
            </LookAt>
        <Style id="inline">
            <ListStyle>
                <listItemType>checkHideChildren</listItemType>
                <bgColor>00ffffff</bgColor>
                <maxSnippetLines>2</maxSnippetLines>
            </ListStyle>
        </Style>
        <Link>
            <href>http://arcgis.library.tamu.edu/flexviewer/travis/cuba_1943/Cuba 1943_1_3_4_2.kmz</href>
        </Link>
    </NetworkLink>
    </kml>

Interestingly, some of the intermediates here have JPF extensions. Normally, this would indicate the file is a
:code:`JPX (JPEG 2000 part 2)` and PRONOM :code:`fmt/151` but Siegfried says this is a :code:`JP2 (JPEG 2000 part 1)`
with an extension mismatch.

.. code-block:: text

    ---
    siegfried   : 1.11.0
    scandate    : 2024-06-12T08:49:11-04:00
    signature   : default.sig
    created     : 2023-12-17T15:54:41+01:00
    identifiers :
      - name    : 'pronom'
        details : 'DROID_SignatureFile_V116.xml; container-signature-20231127.xml'
    ---
    filename : '/Users/mark.baggett/Downloads/map_cuba_ams_1943.jpf'
    filesize : 151732610
    modified : 2024-06-12T08:48:33-04:00
    errors   :
    matches  :
      - ns      : 'pronom'
        id      : 'x-fmt/392'
        format  : 'JP2 (JPEG 2000 part 1)'
        version :
        mime    : 'image/jp2'
        class   : 'Image (Raster)'
        basis   : 'byte match at 0, 23'
        warning : 'extension mismatch'

**Stack**

* DSPACE (DAMS)
* SAGE (Delivery)
* Cantaloupe
* iRIIIFService
* Mirador

**Questions and Thoughts**

* Why are these JPFs? Are they JPEG 2000 part 1s or part 2s?
* Do we have digitization standards for various files and if so where are they?
* What is the purpose of the KML files? If it's really this simple, shouldn't we just capture in :code:`dcterms:spatial`?
* This may be a good collection for demoing georeferencing with IIIF.

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation, navPlace, `geoReference <https://iiif.io/api/extension/georef/>`_

======================
Images of a Rural Past
======================

`Homepage <https://www.flickr.com/photos/cushinglibrary/collections/72157617092580769/>`_

This collection of historical photographs was acquired in the early 1970s from the Agricultural Communications Office of
the Texas Agricultural Extension Service. The physical collection consists of nearly 7,000 photographs and a sampling of
these items have been digitized and made accessible online. The vast majority of the images are black and white and
range from the 1930s through the late 1970s, although some photographs date from earlier and later periods. The images
were captured by photographers working throughout the state and document many activities aimed at improving the lives
and livelihood of rural Texans. Farming, home improvement, livestock raising, and other programs of the Extension
Service were illustrated and the photographs were retained for educational and publicity initiatives.

The items here are all stored in Flickr. There seems to be plenty of metadata.  Why are these not in a DAMS (are they?)?

**Stack**

* Flickr

**Questions and Thoughts**

* Why are these not in a DAMS?
* Could we just pull these and the metadata over into a DAMS and serve these easily?
* Does Special Collections care about this collection?

**IIIF**

* Current: None
* Future: Minimally Image, Presentation

=================================================
Index-Catalogue of Medical and Veterinary Zoology
=================================================

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/90524>`_

**Note**: The link to this collection is over HTTP instead of HTTPs.  How can we change this?

The Texas A&M University Medical Sciences Library has partnered with Oklahoma State University Libraries to digitize the
Index-Catalogue of Medical and Veterinary Zoology, a multilingual periodical published by the US Government Printing
Office. This historical compendium of the parasitological literature is a key resource of importance to researchers in
re-emerging diseases and global animal health. The compilation of content began in 1892, and resulted in over 100
separate publications comprising over 20,000 pages.

It appears that the collection is all PDFs but they are very slow to load from DSPACE. Why? If you must download a
resource to see it and it takes this long, should we have an alternate viewing method?

**Stack**

* DSPACE

**Questions and Thoughts**

* It appears that the collection is all PDFs but they are very slow to load from DSPACE. Why? If you must download a resource to see it and it takes this long, should we have an alternate viewing method?
* Are all collections in DSPACE this slow to load? What about image collections?

**IIIF**

* Current: None
* Future: ?

===============================================================================================================
Live To Build A Better World: Despair, Survival, and Hope in Science Fiction's Response to Environmental Change
===============================================================================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/scifi-exhibit-2021>`_

This digital collection reflects the content of an exhibit presented at Cushing Memorial Library & Archives from January
- June 2021. Consisting of books, movie posters, and, in one case, an elaborate handcrafted tapestry, the exhibit
explored many examples of science fiction's reactions to human-caused climate change over the 20th and early 21st
centuries.

There are 108 items, and this seems to be very exhibit forward. Most of the items are book covers, movie posters, etc.

**Stack**

* Fedora for Digital Assets Management
* Spotlight for Exhibiting
* Cantaloupe
* iRIIIFService
* Mirador

**Questions and Thoughts**

* ?

**IIIF**

* Current: Image, Presentation
* Future: Minimally Image, Presentation

============================
Maps of Brazos County, Texas
============================

`Homepage <https://library.tamu.edu/discovery/discovery-context/brazos-maps?direction=ASC>`_

This digital collection features maps of Brazos County, the cities of College Station and Bryan, and the campus of Texas
A&M University. There are 90 total works.

**Stack**

* Fedora for Digital Assets Management
* SAGE for Exhibiting
* Cantaloupe
* iRIIIFService
* Mirador

**Questions and Thoughts**

* ?

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation, navPlace, `geoReference <https://iiif.io/api/extension/georef/>`_

===========================
The Mina De Malfois Archive
===========================

`The Mina De Malfois Archive`_

The Mina De Malfois Archive contains stories from “Mina” herself (Carlanime), plus numerous others from fans that
Carlanime generously allowed to play in her world. Also included are several podcasts, examples of Mina-oriented fan
art, and pieces of Sanguinity fanfiction. The latter again demonstrates the meta nature of the Minaverse – fanfiction
about a nonexistent fandom that serves as a satire of existing online fandoms. The thumbnail of Mina was created by and
is credited to Mute Cornett.

There is a mixture of works here including: PDF, mp3s, and images.  Also, this may be the first collection I've seen
with creative commons licenses. The badge is displayed and URI is written to :code:`dc.rights.uri`.

**Stack**

* DSPACE

**Questions and Thoughts**

* ?

**IIIF**

* Current: None
* Future: Image, Presentation

===============================================
The Minutes of the Houston Oil Company of Texas
===============================================

`Homepage <https://library.tamu.edu/collections/digital-library/houston-oil-minutes>`_

The Houston Oil Company of Texas was founded by John Henry Kirby in 1901, simultaneously Kirby and his investors founded
the Kirby Lumber Company. These two companies allowed for dual use of land in East Texas, which was rich in both forest
and oil. For many years, the Houston Oil Company of Texas developed into the largest corporation in Texas, a distinction
it retained for many years.

This minute book - one volume, 299 pages - encompasses the first eight years of the corporation’s business.

This is the first exhibit I've seen served from a page like this. It doesn't appear to be SAGE or Spotlight, but instead
something else entirely.  A mirador viewer is embedded on the landing page with descriptive text about the project.

The project also links to From the Page which is what is being used to aid in Transcription.  While over 30% of this
seems to be complete, there is a problem. Some images no longer load.  Sometimes the thumbnail will load but the base
image does not and sometimes both won't load.  Perhaps this is why the crowdsourcing has fallen short here? Weirdly,
I think some of this used to load though as the transcription is complete.  On further inspection, this looks to be
caused by the image server response resulting in a 404.  Here is an example:

https://api.library.tamu.edu/iiif/2/6e82108d-0809-305d-a5b8-7b8c1f252f9c/info.json

Also, the reason some of the views look bad is because the image response loads, some tiles / zoom levels load, but most
return a 404.

How on earth is this being loaded into Cantaloupe? Where are the underlying images?

**Stack**

* Cantaloupe
* From the Page for Transcription

**Questions and Thoughts**

* Is the same manifest used for delivery and From the page? Is this the source of the fail?
* How can we get data out of from the page and back into IIIF annotations?
* The manifest id on the main page has an :code:`id` that doesn't render any canvases.  Whatever is happening here isn't valid and well formed IIIF.

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation

================
Owens Folk Music
================

This collection contains sound recordings made by William A. Owens during the late 1930s to early 1940s, during which
time he was a professor of English at the Agricultural & Mechanical College of Texas. The recordings document folk
songs, ballads, play-party songs, fiddle tunes, and folk culture of East and Central Texas. Some of the material was
later transcribed and published in Owens' books "Texas Folk Music" and "Tell Me a Story, Sing Me a Song..." and are
noted in item descriptions

Audio CDs transfers of the original disks were made in 2002 by The Cutting Corporation. The recordings are of good
quality unless noted otherwise.

Please note that some items in this collection contain racially insensitive and offensive language. In an effort to
represent the resource as accurately as possible, library staff have transcribed the title exactly as it appears on
the archival material or object.

Items are open. Most are served as "playlists," but it's not clear from the metadata how the parts are related. There
are no transcripts or audio descriptions. The audio is in multiple languages.

**Stack**

* Avalon

**Questions and Thoughts**

* Is there a requirement for closed captioning or subtitle files?
* How are the tracks related to the overall work? What was the arrangement based on?

**IIIF**

* Current: None
* Future: Presentation

===============
Primeros Libros
===============

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/92213>`_

The Primeros Libros de las Américas: Impresos Americanos del Siglo XVI en las Bibliotecas del Mundo project is a digital
collection of the first books printed in the Americas before 1601. These monographs are very important because they
represent the first printing in the New World and provide primary sources for scholarly studies in a variety of academic
fields. Of the 220 editions believed to have been produced in Mexico and 20 in Peru, approximately 155 are represented
in institutions around the world.

Only some of the works (34) have associated files. When a work has files, there appears to be a mixture of JP2s (as JPFs)
and jpgs along with a corresponding PDF.

Here is a `sample work <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Fdspace%2Fpresentation%2F1969.1%2F94147>`_.

Is the order here correct? Have I assumed books from DSPACE are sequenced properly?

Also, are PDFs split and added to Cantaloupe?

`Here is a list of all works with files. <https://oaktrust.library.tamu.edu/handle/1969.1/92213/discover?filtertype=has_content_in_original_bundle&filter_relational_operator=equals&filter=true>`_

`Here is the corresponding ttl for the item above. <https://oaktrust.library.tamu.edu/rdf/handle/1969.1/94147>`_

**Stack**

* DSPACE

**Questions and Thoughts**

* Does irIIIFService order canvases? Is it random? Is it based on the RDF? Investigate.
* Are new volumes still being added?
* What's up with all these JPFs? Are there standards for JP2s?
* Does ifIIIFService really split and combine all files (PDFs, JPGs, JP2s)?

**IIIF**

* Current: None
* Future: Image, Presentation

===================================
The Raiford L. Stripling Collection
===================================

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/94833>`_

**Note**: Loaded over HTTP

In the fall of 1927, Raiford L. Stripling (1910-1990) enrolled as a freshman in the department of architecture at the
Agricultural and Mechanical College of Texas. Under the guidance of Samuel Charles Phelps Vosper and Ernest Langford,
two distinguished faculty members in the department of architecture, Stripling was schooled in the Beaux Arts tradition,
which emphasizes classical design, rigorous attention to fine detailing, and sound construction methods. In 1947
Stripling opened his own practice in his hometown of San Augustine, Texas and over the course of his career he worked on
some of Texas’ most significant restoration projects, as well as many single family residences, banks, churches, and
schools. In 1990 Raiford L. Stripling passed away, leaving behind a body of work that will contribute significantly to
the fields of architecture and architectural history for many years to come. This collection is made up of over 250
projects contained in 24 boxes, as well as drawings and construction documents housed in flat files in one map case. In
addition to architectural drawings and blueprints, the collection contains contract documents, correspondence,
brochures, pamphlets, newspaper articles, magazine articles, photographs, sketches, drawings, and miscellaneous notes.

Almost everything here appears to be JPFs.

**Stack**

* DSPACE

**Questions and Thoughts**

* How does this site work: https://library.tamu.edu/research/digital_collections
* Who can edit it?

**IIIF**

* Current: None
* Future: Image, Presentation

=============================================
Science Fiction and Fantasy Research Database
=============================================

`Homepage <https://sffrd.library.tamu.edu/site/>`_

The Science Fiction and Fantasy Research Database is an on-line, searchable compilation and extension of Science Fiction and Fantasy Reference Index 1878-1985, Science Fiction and Fantasy Reference Index 1985-1991, and Science Fiction and Fantasy Reference Index 1992-1995, including material located since publication of the last printed volume.

**Stack**

* ???

**Questions and Thoughts**

* Is this in the inventory?
* Who is the product owner and maintainer?

**IIIF**

* Current: None

=================================================
The Stephen Powys Marks London Collection, Part 1
=================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/london-collection>`_

This exhibit is split into 2 parts. Some of the manifests appear to be broken. Also, this is one of the first Fedora
collections that seem to have order. For example:
https://spotlight.library.tamu.edu/spotlight/london-collection/catalog/d46adeb610031a28bf682e4f68817128

An example of a broken manifest is here:
https://spotlight.library.tamu.edu/spotlight/london-collection/catalog/bd1184d90258f484e41db991934c5559

**Stack**

* Spotlight
* Fedora
* Cantaloupe
* irIIIFService

**Questions and Thoughts**

* What does the structural metadata look like for complex objects?
* Why are so many manifests broken?

**IIIF**

* Current: Image, Presentation
* Future: Minimally Image, Presentation


=================================================
The Stephen Powys Marks London Collection, Part 2
=================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/london-maps-batch-2>`_

Similar to above, but with what seems to be working manifests.

**Stack**

* Spotlight
* Fedora
* Cantaloupe
* irIIIFService

**Questions and Thoughts**

* Why is this a second part and not linked from homepage?

**IIIF**

* Current: Image, Presentation
* Future: Minimally Image, Presentation

====================================================
Texas A&M Forest Service Radio Broadcasts Collection
====================================================

`Homepage <https://avalon.library.tamu.edu/collections/xp68kg260>`_

The radio programs in this collection were produced between approximately 1946 and 1959 as part of the Cooperative
Forest Fire Prevention (CFFP) Campaign, a collaboration between the United States Department of Agriculture, the
Advertising Council, and state forestry services. Vinyl and electric transcription disc were distributed to radio
station across Texas and the nation. The longest running PSA campaign in U.S. history, the CFFP program introduced the
Smokey Bear character in the early 1940s.

There are no transcripts or audio descriptions. It all appears to be audio.

**Stack**

* Avalon

**Questions and Thoughts**

* Are assets for Avalon stored in Avalon or somewhere else?
* Do we not need transcripts of some type.

**IIIF**

* Current: None
* Future: Presentation

======================================
Texas A&M University Archived Catalogs
======================================

`Homepage <https://library.tamu.edu/collections/digital-library/course-catalogs>`_

This archive is a culmination of Texas A&M University catalogs beginning in 1876. The information included in these
volumes and the way it is presented varies quite a bit, especially in the formative years. The official title for the
catalogs fluctuates as well; therefore, for archival and searching purposes, these volumes will be referenced as
University Catalogs and include the academic year.

Looks like all PDFs from DSPACE into SAGE with IIIF.

**Stack**

* DSPACE for assets management
* Custom Webpage
* SAGE
* Cantaloupe
* irIIIFService


**Questions and Thoughts**

* How does irIIIFService split PDFs?
* How is the custom front end done?
* How do new items get in?

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation

===============================================
Texas A&M Newspapers and Periodicals Collection
===============================================

`Homepage <https://library.tamu.edu/collections/digital-library/newspapers.php>`_

The Texas A&M Newspaper Collection offers a window into student life and campus happenings at Texas A&M. The newspapers
provide a first-hand account of events that impacted student life which occurred on campus as well as from around the
world.

The landing page is maybe apart of the general website and it points to 3 distinct collections in Open Oni. These use
a viewer (looks like Open Oni) that supports HOCR or Alto.

It's not clear where assets are stored.

**Stack**

* Custom Webpage
* OpenOni

**Questions and Thoughts**

* Where are assets stored?
* How is HOCR or Alto done?
* What is the content model?

**IIIF**

* Current: None
* Future: Image, Presentation

=========================================
Texas A&M University Yearbooks Collection
=========================================

`Homepage <https://library.tamu.edu/yearbooks/>`_

The Texas A&M University Yearbook Online Collection begins with the initial 1895 Olio publication. The yearbooks begin
annual publication in 1903 and continue through today. The newer editions are planned to be included on this website in
future developments. The original yearbooks can be viewed at the Cushing Memorial Library & Archives.

The landing page points at an application driven by the Internet Archive Bookreader. For instance:
https://bookreader.library.tamu.edu/book.php?id=yb1895&getbook=Go#page/n0/mode/2up

There is HOCR or Alto?

**Stack**

* InternetArchive bookreader

**Questions and Thoughts**

* Where are assets stored?
* How is HOCR or Alto done?
* What is the content model?
* Why IA Bookreader?

**IIIF**

* Current: None
* Future: Image, Presentation

=====================
Texas Data Repository
=====================

`Homepage <https://dataverse.tdl.org/dataverse/tamu>`_

Dataverse instance provided by Texas Digital Library for Datasets.

Shared instance with TAMU portal.


**Stack**

* Dataverse

**Questions and Thoughts**

* Who is product owner?
* How long are datasets kept for?
* Open and restricted data?

**IIIF**

* Current: None
* Future: None

========================================================
A Time of Resolve: Texas A&M during the Great Depression
========================================================

"A Time of Resolve: Texas A&M during the Great Depression," was an exhibit at Texas A&M's Cushing Memorial Library and
Archives that ran September 7, 2018 through February 22, 2019.

There are 140 items.  Some manifests aren't working correctly like:
https://library.tamu.edu/discovery/discovery-context/time-of-resolve/aHR0cHM6Ly9hcGkubGlicmFyeS50YW11LmVkdS9mY3JlcG8vcmVzdC8zYi82Zi9jMy8yNS8zYjZmYzMyNS1mNmNhLTQxZDgtYjkxZS04YzVkYjNiZThjMTMvdGltZV9vZl9yZXNvbHZlX29iamVjdHMvMg==

**Stack**

* Fedora for Assets Management
* SAGE for display
* Cantaloupe
* irIIIFService

**Questions and Thoughts**

* What's up with Fedora and bad manifests?

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation

=================================================================================
Toward a Better Living: African American Farming Communities in Mid-Century Texas
=================================================================================

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/91004>`_

This collection of historical photographs was acquired in the early 1970s from the Agricultural Communications Office
of the Texas Agricultural Extension Service. The physical collection, housed in Cushing Memorial Library & Archives,
consists of nearly 7,000 photographs. This subset of the collection illustrates African American farming and community
life in Texas from the early 1930s through 1960s. The vast majority of the images are in black and white and document
activities such as farming, home improvement, livestock raising, and other programs of the Extension Service.

All images.

**Stack**

* DSPACE
* IIPMooviewer
* Djatoka

**Questions and Thoughts**

* ?

**IIIF**

* Current: None?
* Future: Image, Presentation

============================
Vascular Plant Image Gallery
============================

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/97046>`_

This is an archive of images from the Vascular Plant Image Library built by the now defunct Texas A&M Bioinformatics
Working Group. There are over 10000 works and no viewer.

**Stack**

* DSPACE

**Questions and Thoughts**

* There is no RDF so no manifest. Is this in other collections where Djatoka, IIPMooViewer are used?
* What from DSPACE gets RDF?

**IIIF**

* Current: None?
* Future: Image, Presentation

======================
Veterans of the Valley
======================

`Homepage <https://avalon.library.tamu.edu/collections/5999n359j>`_

Veterans of the Valley” is a collection of 140 interviews and preparatory materials created for the KAMU-TV produced
and aired television series of the same name. Created by host Tom Turbiville at WTAW radio as “Bravo Brazos Valley,”
“Veterans of the Valley” was developed in 2004 at the request of KAMU-TV’s Jon Bennett and co-produced by Kyle
Netterville at KAMU-TV’s studio on the Texas A&M University, College Station campus. The collection was donated to
Cushing Memorial Library and Archives in 2017 by Turbiville with the knowledge and understanding from KAMU that the
materials would be made publicly available.

These are open, but there are no captions or transcripts.

**Stack**

* Avalon

**Questions and Thoughts**

* Where are assets managed?
* Should we add captions?
* How do we get them in to Avalon

**IIIF**

* Current: None?
* Future: Presentation

==================
Wheelan Collection
==================

`Homepage <http://oaktrust.library.tamu.edu/handle/1969.1/590>`_

Wheelan was one of a legion of newspaper and magazine reporters and photographers who covered the Mexican Revolution. He
probably arrived in Northern Mexico early in the winter of 1913-1914. The main attraction was General Francisco (Pancho)
Villa, who held Ciudad Juarez, just across the Rio Grande from El Paso, Texas. By this time Villa had the reputation of
being the most able military commander among the Constitutionalists, a coalition of revolutionaries in rebellion against
the provisional government of General Victoriano Huerta. In February, 1913, Huerta had conspired in the overthrow of the
constitutionally elected government of President Francisco Madero. Villa, a devout supporter of Madero, was one of
several leaders in Northern Mexico who were fighting for the restoration of constitutional government and for
revolutionary reforms.

**Stack**

* DSPACE
* Djatoka
* IIPMoo Viewer

**Questions and Thoughts**

* There is no RDF so no manifest. Is this in other collections where Djatoka, IIPMooViewer are used?
* What from DSPACE gets RDF?

**IIIF**

* Current: None?
* Future: Image, Presentation

=======================================================================================
"Who in the world am I? Ah, that's the great puzzle!": The Faces of Alice in Wonderland
=======================================================================================

`Homepage <https://spotlight.library.tamu.edu/spotlight/alice-in-wonderland>`_

This exhibit features images of Alice from artists all over the world, starting with Alice's original illustrator Sir
John Tenniel. Alice may be a single little girl, but she wears many faces and many bodies. A variety of artists have
interpreted Alice and Carroll's other characters in different styles, using different imagery, and with different themes
and motivations. It's a particularly fitting situation for Alice, who repeatedly has her identity questioned (not least
by herself) throughout the books.

There are 27 works and 2 slideshows.

**Stack**

* Spotlight
* Fedora
* Mirador
* Cantaloupe

**Questions and Thoughts**

* How are the slideshows created? Could they be IIIF Collections

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation

=====================
World War I Postcards
=====================

`Homepage <https://library.tamu.edu/discovery/discovery-context/wwi-postcards?direction=ASC>`_

This digital collection contains World War I era postcards held in the Cooper K. Ragan Military Collection at Cushing
Memorial Library & Archives.

There are fronts and backs but there doesn't appear to be an order.

**Stack**

* Spotlight
* DSPACE
* Mirador
* Cantaloupe
* irIIIFService

**Questions and Thoughts**

* Is there a way to order things from DSPACE?
* How come order doesn't match the turtle?

**IIIF**

* Current: Image, Presentation
* Future: Image, Presentation

