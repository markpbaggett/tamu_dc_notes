Draft: Intermediate and Access Files
====================================

About
-----

This section establishes some thoughts regarding guidelines for intermediate files in our digital collection projects.

The draft guidelines are informed by many documents including:

* `FADGI's Technical Guidelines for Digitizing Cultural Heritage Materials <https://www.digitizationguidelines.gov/guidelines/FADGITechnicalGuidelinesforDigitizingCulturalHeritageMaterials_ThirdEdition_05092023.pdf>`_

What Is an Intermediate File
----------------------------

Often called service, access, delivery, viewing, or output files, intermediate files as defined by the
PCDM Use Extension are high quality representations of an asset, appropriate for generating derivatives or other
additional processing. [#f1]_ By their nature intermediate files are generally not considered to be permanent parts of
an archival collection or repository but instead as a data source to produce one or more derivatives, each optimized for
a particular use. Typical uses (each of which may require a different optimization) include the provision of end-user
access, high quality reproduction, or the creation of textual representations via optical character recognition (OCR),
handprint character recognition (HCR), or handwritten text recognition (HTR).

In many cases, the derivatives intended to serve end-user access employ lossy compression, e.g., JPEG-formatted images.
Significant benefits can result from the appropriate use of file compression. The type of compression and file format
can be dependent on cost of storage space, amount of available space, type of application, etc. but should not employ
patented techniques or proprietary software due to long-term sustainability concerns.

Why Should We Even Care About This?
-----------------------------------

In order for users to be able to access a high quality representation of an original item, we want to create a digital
representation that is of the highest achievable quality while keeping in mind technical issues that may occur. This
could be file size or even unnecessary capture of additional data that does not improve the visualization of the item
to users.

While the Preservation group sets their own standards for digitization, we need standards to ensure the items in our
asset management systems provide a good user experience and high quality representation of the original item. Failure to
find balance between these two ideas can cause major problems for the viewing experience.

For example, let's look at `Cuba <https://theseus-viewer.netlify.app/?iiif-content=https://api.library.tamu.edu/iiif-service/dspace/presentation/1969.1/128911>`_
from `Historical Maps of Cuba <https://library.tamu.edu/discovery/discovery-context/tamu-cuba-maps?direction=ASC>`_.
This is a multi-canvased map of Cuba from 1992.  The first canvas is a map that shows roads and administrative data
plus biome data like "mangroves", "swamps", and "reefs". The second canvas is a gazetteer that is appears on the verso
of the map. While the map is viewable in the viewer above and likely in most viewers, it's needlessly big. In fact, `the verso fails to
load at its full size <https://api.library.tamu.edu/iiif/2/bb864ab1-84ce-340d-8198-5e4c7bb87ca2;1/full/full/0/default.jpg>`_
and returns a 504 Gateway Timeout error when requested. Due to our manifests and how some viewers build thumbnails,
viewing experience may be affected.

When looking at the technical metadata, it's not possible to see the original dimensions of the map.

.. code-block:: text

      Filename: /Users/mark.baggett/Downloads/map_cuba_cia_1992b_back.jpf
      Permissions: rw-r--r--
      Format: JP2 (JPEG-2000 File Format Syntax)
      Mime type: image/jp2
      Class: DirectClass
      Geometry: 19770x15168+0+0
      Units: Undefined
      Colorspace: sRGB
      Type: TrueColor
      Base type: Undefined
      Endianness: Undefined
      Depth: 8-bit
      Channels: 3.0
      Channel depth:
        Red: 8-bit
        Green: 8-bit
        Blue: 8-bit
      Channel statistics:
        Pixels: 299871360
        Red:
          min: 0  (0)
          max: 255 (1)
          mean: 237.57 (0.931647)
          median: 242 (0.94902)
          standard deviation: 25.3432 (0.0993852)
          kurtosis: 33.9046
          skewness: -5.60416
          entropy: 0.624629
        Green:
          min: 0  (0)
          max: 255 (1)
          mean: 239.143 (0.937817)
          median: 244 (0.956863)
          standard deviation: 26.7176 (0.104775)
          kurtosis: 37.0533
          skewness: -5.93364
          entropy: 0.582965
        Blue:
          min: 0  (0)
          max: 255 (1)
          mean: 236.069 (0.925761)
          median: 240 (0.941176)
          standard deviation: 25.2963 (0.099201)
          kurtosis: 37.1995
          skewness: -5.90491
          entropy: 0.594829
      Image statistics:
        Overall:
          min: 0  (0)
          max: 255 (1)
          mean: 237.594 (0.931742)
          median: 242 (0.94902)
          standard deviation: 25.7857 (0.10112)
          kurtosis: 36.0525
          skewness: -5.81424
          entropy: 0.600808
      Rendering intent: Perceptual
      Gamma: 0.454545
      Chromaticity:
        red primary: (0.64,0.33,0.03)
        green primary: (0.3,0.6,0.1)
        blue primary: (0.15,0.06,0.79)
        white point: (0.3127,0.329,0.3583)
      Matte color: grey74
      Background color: white
      Border color: srgb(223,223,223)
      Transparent color: black
      Interlace: None
      Intensity: Undefined
      Compose: Over
      Page geometry: 19770x15168+0+0
      Dispose: Undefined
      Iterations: 0
      Compression: JPEG2000
      Orientation: Undefined
      Properties:
        date:create: 2024-07-01T16:06:55+00:00
        date:modify: 2024-07-01T16:06:55+00:00
        date:timestamp: 2024-07-01T16:08:15+00:00
        signature: 3fcda332fcd7f58e85a01d5d631eab4240c16b451119316e0aba5430c983fd0f
      Artifacts:
        verbose: true
      Tainted: False
      Filesize: 490.034MiB
      Number pixels: 299.871M
      Pixel cache type: Memory
      Pixels per second: 4.87099MP
      User time: 59.390u
      Elapsed time: 1:02.562
      Version: ImageMagick 7.1.1-33 Q16-HDRI aarch64 22263 https://imagemagick.org

I assume that the original TIFF would have had the physical dimensions, but those aren't here. For that reason, let's
make some guesses on size.  We can use the dimensions we know to make guesses about original size.  Let's do that to
guess the original length of the long edge of the map:

* 600 PPI: :code:`19770/600 = 32.95 inches`
* 400 PPI: :code:`19770/400 = 49.425 inches`
* 300 PPI: :code:`19770/300 = 65.9 inches`
* 200 PPI: :code:`19770/200 = 98.85 inches`

While we can't say for certain, 32 x 25 is a standard map size. Let's pretend we followed FADGI guidelines for this
project:

* FADGI 4 Star: :code:`32.95 inches × 396 PPI = 13048.2 pixels`
* FADGI 3 Star: :code:`32.95 inches × 294 PPI = 9687.3 pixels`
* FADGI 2 Star: :code:`32.95 inches × 242.5 PPI = 7990.375 pixels`
* FADGI 1 Star: :code:`32.95 inches × 190 PPI = 6260.5 pixels`

In other words, assuming this image is 32.5 on the long edge, the image we're saving would be much smaller and processed much
more efficiently.


.. rubric:: Footnotes

.. [#f1] https://pcdm.org/2021/04/09/use#IntermediateFile
.. [#f2] Clover struggles to build thumbnails due to our manifests and this problem. `View in Clover <https://samvera-labs.github.io/clover-iiif/docs/viewer/demo?iiif-content=https%3A%2F%2Fapi.library.tamu.edu%2Fiiif-service%2Fdspace%2Fpresentation%2F1969.1%2F128911>`.
