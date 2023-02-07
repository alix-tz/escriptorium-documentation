---
title: Exporting annotations from eScriptorium
summary: Tutorial on export features in eScriptorium.
authors:
    - Hugo Scheithauer, Alix Chagué
date: 2023-02-01
---

# Walkthrough : Export from eScriptorium

## Exporting models

## Exporting annotations

eScriptorium allows users to export annotations done manually or automatically with a transcription model. 

The exporting feature is located in the "images" tab `{base_url}/document/{document-id}/images/`, inside an eScriptorium document. 

Select the relevant part-documents by ticking their checkboxes, then click on the blue "Export" button, right next to the "Import" button. A pop-up box will then appear.

!!! Tip
    You can select multiple documents at once by pressing the _shift_ button on your keyboard.
    
![Image: Demonstration of selecting part-documents and then clicking on the 'Export' button](img/export/escriptorium_export_select_partdocuments.gif)

There are four options when exporting part-documents.

### Selecting the version of the transcription to export

You can select the version of the transcription to export in the first drop-down menu. 

!!! Note
    * Manual annotations are registered as the __manual__ version.
    * Imported annotations, when batch imported with a zip file, are registered as the __Zip import__ version.
    * Annotations done with a transcription model are named with the model's name.
    
![Image: Illustration of the drop-down menu for selecting the version of the transcription](img/export/escriptorium_export_transcription_version.gif)

### Selecting the annotation format to export

You can select three exporting formats from the second drop-down menu:
    * Text for plain text
    * PAGE for [PAGE XML](http://www.primaresearch.org/publications/ICPR2010_Pletschacher_PAGE)
    * ALTO for [XML ALTO](https://www.loc.gov/standards/alto/) (Analyzed Layout and Text Object)
    
![Image: Illustration of the drop-down menu for selecting the exporting format](img/export/escriptorium_export_format.gif)

### Including (or not) images linked to the annotations

You can tick the checkbox if you want to include images that are linked to the annotations. As it is mentioned in the export pop-up box, and depending on the images' sizes, including image in the export can significantly increase the time to produce and download the export.

![Image: Ticking the checkbox for including images in the export](img/export/escriptorium_export_include_images.gif)

### Selecting the region types to export

You can select the region types you want to export. <!-- todo: add link to the subsection about segment version -->

To do so, tick the checkboxex associated to the region types you want to export. 

![Image: Ticking the region types' checkboxes chosen for the export](img/export/escriptorium_export_region_types.gif)

!!! Note
    By default, there are __six region types__ available to export : Illustration, Commentary, Main, Title, (Undefined region type), (Orphan lines).

    (Undefined region type) are regions without a name. 

    (Orphan lines) are lines not linked to any region. Make sure to always tick the checkbox for (Orphan lines) to avoid loosing any not-linked annotation.

    You can export a region type even though no annotations are linked to it. It will be mentioned in the resulting exported file, but no annotations will be linked to it. 

!!! Note
    Region types' name will only appear when exporting in ALTO and PAGE. When exporting as plain text, only the annotations will be exported.

## Downloading the export

Once all options are set, click on the blue "Export" button. A green pop-up box will appear in the upper-right section of the interface. Click on "Download" to download the part-documents you selected.

When exporting ALTO and PAGE, the export is downloaded as a zip file containg each part-documents.

When exporting plain text, the download will open a new tab with a new URL, containing the plain text. All annotations will be concatenated as one file text.

![Image: Illustration of the export](img/export/escriptorium_export_download.png)

!!! Tip
    To avoid confusions between exports, make sure to click on the cross icon in the download pop-up box before creating a new export.
