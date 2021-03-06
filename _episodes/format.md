---
title: "File format"
teaching: 15
exercises: 20
questions:
- "What is a file format?"
- "What file formats should I use?"
objectives:
- "Name common formats used in climate-related domains."
- "Understand different types of data."
- "Choose correct file formats for your work."

keypoints:
- "Choose formats that are common to your field/community to ensure the interoperability and reusability of your data."
- "Make sure that the file formats you choose can hold the necessary data elements and information."
- "Decide on how long do you intend to preserve your data."
- "Make sure to check requirements of the repository where data is stored."
---

## File format

A [file format](https://en.wikipedia.org/wiki/File_format) is the structure of a
file. It determines how the data within the file is organized. Files are usually
named as `filename.format`. For example, climate.jpeg is a file named climate
with [jpeg](https://en.wikipedia.org/wiki/JPEG) format. You might know that
`jpeg` is a commonly used format for digital images. Therefore, the file
`climate` is probably an image.

Each file type like images, video, and text can be stored in several formats.
For example, `climate.jpeg`, `climate.png`, and `climate.gif`. All file formats
are used to store image data, but they have differences in compression,
available colors, resulting filesize, etc (for more information see [this
page](https://fixthephoto.com/tech-tips/difference-between-jpeg-and-png.html)).
When deciding which one to use, it’s important to note the advantages and
disadvantages of each.

Also, formats may be dependent on particular software. When data is stored from
a software program, it is usually saved in that program’s standard file format.
One example is creating tabular data using spreadsheet software. Tabular data
have specific properties that are better supported by the spreadsheet software
than a word processor.

> ## No extension or multiple extensions!
>
> In [UNIX-like](https://en.wikipedia.org/wiki/UNIX-like) operating systems, a
> file can have no extensions, or more than one extension. For example, in
> `filename.tar.gz`, the `.tar` indicates that the file is a tar archive of one
> or more files, and the `.gz` indicates that the tar archive file is compressed
> with [gzip](https://en.wikipedia.org/wiki/Gzip). Also, programs reading files
> usually ignore the format; it is mostly intended for the human user. In
> Windows, a file should have at least one extension.
{: .callout}

> ## File formats for geospatial data in your community/research team
>
> Here are some questions about the use case you chose in the introduction.
>
> 1. What is the format of the geospatial data?
> 2. Do you know why the data is in that format?
>
{: .discussion}

> ## This is what [go-FAIR.org](https://go-fair.org/principles) has to say about Format
>
> - I1:(meta) data use a formal, accessible, shared, and broadly applicable
>  language for knowledge representation. For example, if data is provided in
>  commonly understood and preferably open formats.
> - R1.3: (meta)data meet domain-relevant community standards e.g. those for
>   data formats.
{: .checklist}

## Recommended formats for different types

There are several data types like geospatial, tabular, storyline, documentation
and paper, textual, video/audio, and image/figure. Some of them are more in line
with the FAIR principles than some others. Here are some recommended formats for
different types:

<table style="width:40%">
  <thead>
  <tr>
      <th>Data type</th>
      <th>Data format</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Geospatial data</td>
      <td><a href="https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html">NetCDF</a></td>
    </tr>
    <tr>
      <td>Tabular data</td>
      <td><a href="https://www.sqlite.org/fileformat.html">SQLite</a></td>
    </tr>
    <tr>
      <td>Textual data</td>
      <td><a href="https://daringfireball.net/projects/markdown/">Markdown</a></td>
    </tr>
    <tr>
      <td>Image data</td>
      <td><a href="https://www.adobe.io/content/dam/udp/en/open/standards/tiff/TIFF6.pdf">TIFF 6.0 uncompressed</a></td>
    </tr>
    <tr>
      <td>Audio data</td>
      <td><a href="https://xiph.org/flac/">Lossless Audio Codec (FLAC)</a></td>
    </tr>
    <tr>
      <td>Video data</td>
      <td><a href="https://en.wikipedia.org/wiki/MPEG-4">MPEG-4</a></td>
    </tr>
    <tr>
      <td>Documentation</td>
      <td><a href="https://en.wikipedia.org/wiki/Microsoft_Word">Microsoft Word</a>
      or <a href="https://www.iso.org/standard/63534.html">PDF</a></td>
    </tr>
    <tr>
      <td>Papers & Articles</td>
      <td><a href="https://www.latex-project.org/">LaTeX</a></td>
    </tr>
    <tr>
      <td>Storyline Definitions</td>
      <td><a href="https://www.json.org/json-en.html">JSON</a></td>
    </tr>
  </tbody>
</table>

> ## Other data types
>
> Have a look at the list of the recommended formats for different types
> (mentioned above) and pick a data type.
>
> - What are the other formats for the type that you selected?
> - Which of those formats are common in your community?
> - Discuss some of the advantages and disadvantages of those formats.
{: .discussion}

> ## Data Management Plan
>
> Data Management Plan (DMP) covers how data can be stored, described and
> reused. For example, see [DMPonline](https://www.dcc.ac.uk/dmponline) or
> [DSW](https://ds-wizard.org/).
{: .callout}

## Different formats for different purposes

In the previous sections, we learned that different file formats have different
properties. The purpose of a file should help determine which file format to
choose. In the example of creating tabular data using spreadsheet software,
there is no guarantee that the tabular data can be used or displayed in the
future. Because the software can become obsolete or only support a specific
version of formats.

It is good to plan at the beginning of your project, what file formats to use
for each purpose:

- data collection / processing / analysis,
- reuse: the longer you want to use the data, the more you have to use open,
  standard and well-documented file formats to avoid obsolescence.
- preservation: many journals, archives and data repositories require that data
  are uploaded in certain file formats. Therefore, you may have to keep some
  data files in multiple formats.

![format_support_matrix]({{ page.root }}/fig/format_support_matrix.png) If we
store the data in a more open or widely supported format, it will have the
greatest re-usability in the future.

> ## Non/proprietary format
>
> File formats may be either proprietary or non-proprietary (open or free):
>
>- The proprietary format is owned by a company, organization or individual.
>   Their specifications are usually not publicly available and the risk of
>   obsolescence is high. If you want to store data in a proprietary format for
>   a reasonable time, consider including a readme.txt file that documents the
>   name and version of the software used to generate the file, as well as the
>   information of the company that made the software.
>
>- The open format is a file format that is published and free to be used by
> everybody.
{: .callout}

> ## Good practice for format selection
>
> We want to create a checklist for choosing a format that improves the FAIRness
> of the data. What items should be included?
>
>> ## Solution
>>
>> - non-proprietary
>> - open or widely supported format
>> - standard and well-documented
>> - supports relevant metadata
>> - commonly used by your research community
> {: .solution}
{: .challenge}

## Common file formats for geospatial data

In climate-related domains e.g. weather and climate science, earth observation
science, or hydrology, data can be in many types and for different purposes. In
this section, we will introduce some common and acceptable data formats.

### [NetCDF](https://www.unidata.ucar.edu/software/netcdf/docs/netcdf_data_model.html):

![NetCDF]({{ page.root }}/fig/netcdf-classic-uml.png)

NetCDF was originally developed for the Earth science community, but it can be
used for **many kinds of data**. It views the world of scientific data in the
same way that a geo-scientist might: there are various quantities such as
temperature or elevation located at points at particular coordinates in space
and time. The quantities (here temperature or elevation) are stored as netCDF
variables whereas coordinates information is stored as netCDF dimensions. The
**metadata**, such as the units, is stored as netCDF attributes.

### [GRIB](https://www.wmo.int/pages/prog/www/DPS/FM92-GRIB2-11-2003.pdf):

GRIB stands for general regularly-distributed information in binary. It is
**commonly used** by the [World Meteorological
Organization](https://public.wmo.int/en) (WMO) for weather model data. It is
also used operationally worldwide by most meteorological centers, for Numerical
Weather Prediction output. Some of the second-generation GRIB are used in
Eumetcast of Meteosat Second Generation. Another example is the North American
Mesoscale model.

### [GeoTIFF](https://www.geospatialworld.net/article/geotiff-a-standard-image-file-format-for-gis-applications/):

GeoTIFF is a standard image file format to describe and store raster image data
with geographic information. So it can be used by Geographic Information System
(GIS) applications. It is suitable for a **wide range of applications
worldwide**. For example, satellite imaging systems, scanned aerial photography,
scanned maps, digital elevation models, or as a result of geographic analyses.
As an example, GeoTIFF 1.1 is an approved NASA Earth Science Data Systems
standard (see [NASA Standards and
Practices](https://earthdata.nasa.gov/esdis/eso/standards-and-references)).

### [HDF5](https://www.hdfgroup.org/solutions/hdf5/):

The Hierarchical Data Format Version 5 (HDF5) implements a model for managing
and storing data, developed by the [National Center for Supercomputing
Applications](http://www.ncsa.illinois.edu/) (NCSA). HDF5 is a
**general-purpose**, **machine-independent** standard for storing scientific
data in files. An HDF5 structure is **self-describing**, allowing an application
to interpret the structure and contents of a file without any outside
information. As an example, NASA's Earth Observing System, the primary data
repository for understanding global climate change uses HDF5, for more
information see [this
page](https://www.loc.gov/preservation/digital/formats/fdd/fdd000229.shtml).

> ## Other formats for geospatial data
>
> There are many other formats to store geospatial data like
> [SHP](https://en.wikipedia.org/wiki/Shapefile)(shapefiles) for vector data,
> [DBF](https://en.wikipedia.org/wiki/.dbf)(database file), and [NetCDF ZARR
> Data](https://www.unidata.ucar.edu/blogs/developer/en/entry/netcdf-zarr-data-model-specification),
> etc.
{: .callout}

> ## Select a data format
>
> Let's have a look at case-study that you selected in introduction of this
> tutorial, [here]({{ page.root }}{% link _episodes/introduction.md %}). Assume
> that the authors want to publish their data. What suggestions would you give
> the authors for data format?
{: .discussion}

{% include links.md %}
