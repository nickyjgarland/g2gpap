# Aerial photography case study

Wroxeter, a small village in present-day Shropshire, England lies on the site of Viroconium, the fourth largest Roman town in Britain and civitas capital of the Cornovii. The site may already have been of importance in the Iron Age, as it controls the middle Severn river valley and part of the Shropshire plains from its location near the Wrekin and on a major Severn ford.

Wroxeter and its hinterland are being studied by teams from the University of Birmingham’s Field Archaeology Unit (BUFAU). Funding for this project was provided from 1994 to 1997 by the Leverhulme Trust. One of the aims of the project is to provide as detailed and accurate a mapping of the town as is possible using modern field techniques including differential GPS, high resolution magnetometry, georeferencing, and photogrammetry.

There is a lot of aerial photographic material available for Wroxeter, which often shows features in great detail. However, to use these photos for mapping we need reliable ground control points, which unfortunately are lacking or insufficient in number in most. A new high resolution geophysical mapping of the town now shows archaeological features in sufficient detail to be able to find the requisite number of control points needed to fix the exact location of air photographic features. A set of high quality vertical aerial photographs from CUCAP, and oblique aerial photographs drawn from the University of Birmingham Library special Baker Collection, were therefore scanned and digitally processed in order to obtain a high resolution and high quality mapping of Roman Wroxeter. This worked example shows how one of the aerial photographs, negative 86/140 from the Baker Collection taken in 1969, was produced.

## Digital image creation

As the original negative and print are in black and white, the scanning was done with 256 greyscale values. This provides sufficient greyscale discrimination for subsequent enhancing and operations to succeed. The scanning resolution was chosen in order to obtain approximately 20cm ground resolution, sufficient for the reliable detection of the smaller archaeological features but not so high as to result in a huge digital file (which would have made further processing and storage more difficult).

## Digital image procesing

The contrast in the image was maximised by greyscale equalisation, an operation that is intended to distribute the 256 available greyscale values equally over the image. No further enhancement (such as destriping, sharpening) was deemed necessary.

The image was imported into GRASS GIS software, where it was georeferenced using the ‘i.points’ and ‘i.rectify2’ procedures. The source for the georeferencing information was itself a georeferenced image containing high resolution geophysical (fluxgate gradiometer) survey data. In order to ‘warp’ the oblique aerial photograph onto the geometrically correct gradiometer data, a second order polynomial ‘warp’ was applied. A simpler first order polynomial, for example an affine transformation, would not sufficiently remove distortions from the image. A third order polynomial ‘warp’ was not possible because that requires a higher number of good ground control points than could be identified in the image.

Finally, parts of the georeferenced image lying away from the control points were clipped, as geometric control would be poor here, and the remaining image was again greyscale equalised to maximise contrast. A 10 x 10 m grid was overlaid on the image to facilitate measurements.

The resulting image looks like this:

```{figure} ../images/g2gp_aerial_survey_aprs.png
---
name: aerial-image
alt: An example of a digitised aerial image.
---
_Copyright: Martijn van Leusen_
```

**Table 1: Sample metadata**

|    Training   |   Validation   |
| :------------ | -------------  |
|     Subject   |	Wroxeter, Roman, urban villa    |
|   Coverage    |	just over 1 ha centred at 356790 308830     |
|   Format      |	Gif     |
|   Type        |	Oblique black and white aerial photograph      |
|   Rights      |	Digital image © Martijn van Leusen from an original aerial photograph © Arnold Baker    |
|   Creator     |	Martijn van Leusen      |
|   Date        |	1998 from a 1969 original       |
|   Identifier  |	Negative 86/140     |
|   Instrument  |	handheld camera     |
|   Resolution  |	approximately 20 cm ground resolution   |
|   Processing Log	    | 1. Scanned at 256 greyscale values and approximately 20 cm ground resolution,  2. Clipped detail from this, and greyscale equalised it, 3. Applied second order transformation using GRASS i.rectify2, 4. Clipped central area and greyscale equalised., 5. Added 10 m grid lines.        |
|      Source   |	University of Birmingham Library Special Baker Collection   |
|   Estimated Error     |	Overall RMS error 0.98 m        |
|   Legend      |	not applicable      |
|   Bibliography        |	Baker, W A 1992 Air Archaeology in the Valley of the River Severn. University of Southampton Ph.D. Thesis.	|
