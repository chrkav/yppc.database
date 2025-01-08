---
title: Metadata Guidelines
layout: page-narrow
permalink: /metadata.html
---

# Metadata Guidelines 

CollectionBuilder-Sheets loads and parses a metadata CSV directly to create your digital collection pages.
To create metadata compatible with this CollectionBuilder-Sheets instance the best way to get started is to make of copy of our template in Google Drive:

[CollectionBuilder Metadata Template](https://docs.google.com/spreadsheets/d/1Uv9ytll0hysMOH1j-VL1lZx6PWvc1zf3L35sK_4IuzI/copy?usp=sharing){:.btn .btn-outline-success target="_blank" rel="noopener"}
{:.text-center}

Alternatively, you can [download the template CSV]({{ '/assets/metadata-template.csv' | relative_url }}) and work on your local machine.
We suggest editing your CSV using [LibreOffice](https://www.libreoffice.org/) Calc, [OpenRefine](https://openrefine.org/), or Google Sheets (and do not suggest using Excel, since Excel's CSV output is not correctly formatted).

Describe your items in your copy of the template, following the [guidelines below](#metadata-fields). 

Once you have items added you can test your metadata using the Config modal:

<button class="btn btn-success" data-bs-toggle="modal" data-bs-target="#cbSetUpModal">Change the Metadata!</button>

----------

## Metadata Spreadsheet Terminology

{% include feature/image.html objectid="/assets/img/metadata_spreadsheet_parts.svg" alt="spreadsheet interface with parts labeled, including header, row, column, cell, and active cell" %}

When creating metadata in a spreadsheet we tend to use this terminology for the parts of the table:

- *columns* => "fields" (the metadata template elements used to describe specific qualities of all objects, essentially the categories of descriptions)
- *rows* => "records" or "items" (each row represents one object's description)
- *cells* => "values" (the individual chunks of metadata)

-----------

## Metadata Fields 

Each of the columns of the metadata template spreadsheet are described below
(i.e. **this is how to fill in your spreadsheet!**).
Please note *required* means that not having a value will result in your metadata not functioning in the digital collection.
All other fields are optional, but suggested!

These guidelines are a summary of fields used in this demo collection. 
For creating your own project (where you can customize the metadata however you want) and more details, see the full [CollectionBuilder metadata docs](https://collectionbuilder.github.io/cb-docs/docs/metadata/).

### id

- *required*
- Unique identifier for the record. Each record needs to have a unique objectid or it won't show up in the collection. It allows us to refer to the item in the collection.
- Value must be all **lowercase** with no spaces or special characters. Underscores (`_`) and dashes (`-`) are okay; **slashes (`/`) should NOT be used in this field**.
- Examples:
    - `example-01`
    - `example-02`

### filename 

- The full URL to the object's file online *or* the full filename of the item's file contained in the "objects" folder of this repository.
- *Please note:* if you are testing online using the demo collection, only links will work!
- Leave blank if their is no object file, or if it is a YouTube video.
- Examples:
    - link to image: `https://digital.lib.uidaho.edu/digital/iiif/bar-stock/1147/full/max/0/default.jpg`
    - link to image: `https://www.lib.uidaho.edu/collectionbuilder/demo-objects/mg101_b6_photographs_01.jpg`
    - link to PDF: `https://cdm17254.contentdm.oclc.org/utils/getfile/collection/idahowater/id/186/filename/iwdl-cda_ellis_1932.pdf`
    - image in the repository "objects" folder: `demo_001.jpg` 
    - PDF in the repository "objects" folder: `demo_002.pdf`
- **Important note on external items:** URLs to external media should always be secure HTTPS links. Media at HTTP links are likely to be blocked by browser security defaults as [mixed content](https://developer.mozilla.org/en-US/docs/Web/Security/Mixed_content), thus will not appear on your pages!

### youtubeid

- This is the unique string assigned to a video when it is uploaded to YouTube. An easy way to find this is to look at the url for your YouTube video. The ID will be the string attached to the end of the url. For example, in "https://www.youtube.com/watch?v=sHhk1eAgopU" the youtubeid is `sHhk1eAgopU`.
- Fill in `youtubeid` **only** for YouTube items--leave it blank for all other items! If your collection does not contain YouTube videos, you can delete the column.
- Example value: `sHhk1eAgopU`

### title

- *required*

### author

### age_group

### boy

### girl

### gender_neutral

### required_cast

### ensemble

### length

### date_published

### publisher

### licensing

### copies

### musical

### adaptation

### adaptation_of

### description

### colocated

### notes

### format
