The DAME and Our Collections
============================

Collections
-----------

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
* Why is that in OakTrust if the other files are in Fedora?

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