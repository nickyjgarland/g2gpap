# Overview of data formats

The tables below list some of the common data formats you may encounter in working with aerial photographs and remotely sensed images.

**Table 1:** Image Exchange Formats

|    Format     |   Description   |
| :------------ | -------------: |
|       BIL, BIP & BSQ       |        BIL (Band Interleaved by Line), BIP (Band interleaved by Pixel) and BSQ (Band Sequential) are raster data formats used for storing single and multiband data [1].      |
|     BMP       |	Bit-Mapped Graphics Format created and owned by Microsoft, more information can be found in the Raster Images Guide.
|     GIF       |	Graphics Interchange Format, a proprietary format developed by Compuserve. More information can be found in the Raster Images Guide.    |
|    GeoTIFF    |	An extension to the TIF graphics standard to incorporate georeferencing information. Although currently supported by a limited number of proprietary GIS, many manufacturers have committed to supporting the standard. It aims to provide a platform-independent method for archiving and transferring spatially referenced raster products.       |
|     HDF       |	The Hierarchical Data Format (HDF) is a common format for storing scientific data and can come in a number of versions and subsets/models (e.g. HDF4, HDF5, HDF-SDS, HDS-EOF) [2] [3].   |
|    JPEG       |	Joint Photographic Expert Group. The original name of the committee that designed the standard image compression algorithm. JPEG is designed for compressing either full colour or grey-scale digital images of ‘natural’, real-world scenes. It does not work so well on non-realistic images, such as cartoons or line drawings. JPEG does not handle compression of black-and-white (1-bit-per-pixel) images or moving pictures (Walker 1993).   |
|    TIFF       |	Tagged Interchange File Format. An industry-standard raster data format. TIFF supports black-and-white, gray-scale, pseudocolor, and true-color images, all of which can be stored in a compressed or uncompressed format. TIFF is commonly used in archiving and desktop publishing and serves as an interface to numerous scanners and graphic arts packages (ESRI 1996). When archiving with the TIFF format, LZW compression should not be used. Variations on TIFF i.e. GeoTIFF (single file) and TIFF world files (a TIFF with an accompanying .tfw file) both allow TIFF images to be georeferenced for inclusion in GIS systems.     |

**Table 2:** Proprietary Image Formats

|    Format     |   Description   |
| :------------ | -------------: |
|     ENVI	    | A simple binary file used by the proprietary ENVI software package.   |
|  ERDAS Imagine (.img)	 | A proprietary raster format native to the ERDAS Imagine application. The software also supports a wide range of export options.  |
| ERDAS ER Mapper (.alg, .ers)  |	A proprietary format native to the ER Mapper application but, as with other ERDAS applications, a wide range of alternative export formats are available.   |
| MicroImages TNTMips  |	A single ‘project’ format that can contain a range of data types (raster, vector, etc.) native to the TNTMips application.  |
| PCI Geomatica (PCIDSK .pix)  |	A proprietary format native to the PCI Geomatics Geomatica application (which also supports a wide range of export formats [4]).     |
|  SPOT (DIMAP)   |	An open format used primarily for raster images but with the capability to contain vector data. The format is partly based on GeoTIFF.  |
|  Sun Raster Format (.ras)  |	A raster format native to Sun UNIX platforms.     |


## References

[1] http://help.arcgis.com/en/arcgisdesktop/10.0/help/index.html#//009t00000010000000

[2] http://www.hdfgroup.org/why_hdf/

[3] http://www.ncl.ucar.edu/Applications/HDF.shtml

[4] http://www.pcigeomatics.com/index.php?option=com_content&view=article&id=76&Itemid=4