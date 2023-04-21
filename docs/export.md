---
title: Exporting data from eScriptorium
summary: Tutorial on export features in eScriptorium.
authors:
    - Hugo Scheithauer, Alix Chagué, Floriane Chiffoleau
date: 2023-02-13
---

# Export data from eScriptorium

## Export transcription and segmentation models

eScriptorium allows users to export models that were previously imported, or models they trained.

To do so, go to the "My Models" page, accessible via the navigation bar, in the upper right section of the interface, or via `{base_url}/models/`.

All models linked to a specific account are listed there with their metadata.

You can export a model with the download button, located after all its metadata on the right. It will then download a file with the `.mlmodel` extension.

!!! Note
    A model will either have the `Segment` role if it is a segmentation model, or the `Recognize` role if it is a transcription model. See the [train](train.md) section for more details.

![Image: Illustration of the download button for downloading transcription and segmenting models.](img/export/escriptorium_export_model.png "Downloading a model with the download button.")

## Export annotations

eScriptorium allows users to export annotations (segmentation and transcription), with or without images, to three different [output formats](#selecting-the-output-format).  

The exporting feature is located in the "Images" tab (also accessible at `{base_url}/document/{document-id}/images/`), inside an eScriptorium document.  

Select the relevant document-parts by ticking their checkboxes, then click on the "Export" button, next to the "Import" button. A pop-up box then appears. It allows to set four parameters for the export.

!!! Tip
    You can select multiple documents at once by pressing the ++shift++ key.

![image: Demonstration of selecting document-parts and then clicking on the 'Export' button](img/export/escriptorium_export_select_partdocuments.gif "Selecting document-parts and starting the export.")

### Select the transcription version

In the first drop-down menu, you can select which transcription version is to be exported.  

!!! Note
    - Manual transcriptions are registered as the **manual** version.
    - Imported transcriptions, when batch imported with a zip file, are registered as the **Zip import** version by default. You can name a transcription version during [import](import.md#import-segmentation-and-transcription).
    - Transcriptions [predicted with a model](predict.md#predict-the-transcription) are named after the model.

![image: Illustration of the drop-down menu for selecting the version of the transcription](img/export/escriptorium_export_transcription_version.gif "Choosing a transcription version")

!!! Note  
    When a document-part does not contain any segmentation, an XML file will still be created.  

!!! Note  
    When a document part does not contain any transcription in the selected transcription version, an XML file will still be created, containing only segmentation information.  

### Select the output format

In the second drop-down menu, you can select between three output formats:

- Text for plain text  
- PAGE for [PAGE XML](http://www.primaresearch.org/publications/ICPR2010_Pletschacher_PAGE)
- ALTO for [XML ALTO](https://www.loc.gov/standards/alto/) (Analyzed Layout and Text Object)

![image: Illustration of the drop-down menu for selecting the output format](img/export/escriptorium_export_format.gif "Choosing the output format.")

### Include or exclude images

You can include the images corresponding to the selected document-parts by ticking the "Include images" checkbox.

As mentioned in the export pop-up box, and depending on the images' size, including images in the export can significantly increase the time to produce and download the export.

![image: Ticking the checkbox for including images in the export](img/export/escriptorium_export_include_images.gif "Checking the box to include images in the export.")

### Include or exclude certain region types or lines

You can include or exclude lines or whole regions and their associated lines with the last parameter. <!-- todo: add link to the subsection about segment version -->

To do so, tick the checkboxes associated to the region types you want to export or uncheck the ones you want to ignore.  

The list of region types corresponds to the region types activated in the "Ontology" tab <!-- todo: add link to that once it's available -->. Two additional options allow you to include or ignore untyped-regions <!-- todo: add link to segmentation, which would hopefully explain that --> or orphan lines (lines that are not linked <!-- todo: add link to linking segments to regions -->to any region).

You can export a region type even though it does not contain any transcription. In ALTO and PAGE files, the resulting regions will simply be empty elements.  

!!! Note
    Regions' type will only appear in ALTO and PAGE. In a plain text export, only the text contained in the transcription is kept.

![image: Ticking the region types' checkboxes chosen for the export](img/export/escriptorium_export_region_types.gif "Selecting and unselecting region types for the export.")  

### Download the export

Once all options are set, click on the "Export" button at the bottom of the pop-up.  

As soon as the export is ready, a green message box will appear in the upper-right section of the interface, providing you with a download link. Click on "Download" to download the txt file or the zip file resulting from your export.

When exporting ALTO and PAGE, the exported file is saved as a zip file containing an XML file per document-part, the corresponding images if included, as well as a METS XML file describing the ensemble.

When exporting plain text, clicking on "Download" will redirect you to a new URL, displaying the plain text. All the transcriptions are concatenated as a single text file.

![image: Illustration of the export](img/export/escriptorium_export_download.gif "Stating the export task and downloading the result.")

!!! Tip
    If you plan on doing several exports, we recommend to close the green message-box after each export (after downloading the file of course).  

### Find previous exports

Each export is provided a unique permanent link. You can save it, for example to automatically re-download it later without having to set the whole export again but it is also possible to find the links to all your previous exports in the [Profile page, under the "Files" tab](users.md#review-and-edit-your-profile).
