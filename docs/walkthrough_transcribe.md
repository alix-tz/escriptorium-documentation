---
title: Transcribe with eScriptorium
summary: About transcription features in eScriptorium.
authors:
    - Floriane Chiffoleau, Alix Chagué
date: 2023-02-09
---


# Walkthrough: transcribe with eScriptorium  


Once the [segmentation of the images](walkthrough_segment.md) have been achieved and [some annotations](walkthrough_annotate.md) have been added, if needed, the next step in eScriptorium will be the text recognition of the documents.  
This step can be done manually, whether it is by hand, by copying it from a text or by importing an XML transcription, or automatically, with a model and some manual correction. 

## Manual transcription
For the manual transcription, there are two panes that can be used: "Transcription", that will display the transcription as it is structured in the images, and "Text", that will display the transcription as a plain succession of text lines, according to the order from the segmentation.

### Transcription by hand
When the transcription has to be done by hand, the best option is to use the "Transcription" pane.  
To add a transcription to its associated segment, click on the corresponding zone. An input window is displayed. To record a transcription, press “Enter”: the transcription interface automatically displays the input field for the next segment.

![image: Illustration of the transcription of the text by hand.](img/transcribe/by_hand.gif "Illustration of the transcription of the text by hand")

### Transcription by copy/paste
When the only available format of the transcription is text, it is possible to add it swiftly on eScriptorium.  
To do so, make sure that the "Text" pane is open. Then, from the text file of your transcription, copy the portion of text present in the image. You can then check, with the "Transcription" pane if everything correspond to the image.

![image: Illustration of the transcription of the text via copy/paste.](img/transcribe/via_copy.gif "Illustration of the transcription of the text via copy/paste")

!!! Note
    If the transcription does not match the segmentation of the image, you have the possibility to modify the transcription in the lines through one of the two panes, until it matches completly.

### Transcription by import
When the transcription is available in an XML format, whether it is ALTO or PAGE, it is possible to add it to eScriptorium, via the 'Import' option.  
This process and its documentation can be found in [this page](walkthrough_import.md).

## Automatic transcription
The automatic transcription is done with a model. It can be a model you have trained yourself, [on eScriptorium](walkthrough_train.md) for example, or a model that were suited for your documents and that you may have found on the [Zenodo repository dedicated to OCR/HTR models](https://zenodo.org/communities/ocr_models/). If it was trained on eScriptorium, the model will already be available in the interface but otherwise, you will have to import it beforehand, by following the instructions detailed in the [Import](walkthrough_import.md) page.

### Application of the text recognition model
In the "Images" tab, select the images you would like to see transcribed by ticking the checkboxes in the top-left corner of the image thumbnail. Then, click on the "Transcribe" button, at the far right of the page, under the corner of the "Drop image" bloc. A pop-up box will appear and you will be able to choose the model you want to apply to the images you selected. After you chose it, click on "Transcribe" and it will start the process of transcription, as you can see by the yellow boxes that were added above the blue boxes for "Edit" on the thumbail of the images. Once the application of the model is finished, the yellow boxes disappeared from the thumbnail and a message in a green box appears in the top-right corner, under the menubar.

!!! Note
    As the transcription is done page by page, the green message will appear as soon as the first image chosen is transcribed. Then, if you have more than one image transcribed, a number in parenthesis will appear next to the "Transcription done!" message and every time a new transcription is finished, the number will go up, until all of the selected images has been transcribed.

![image: Application of the text recognition model.](img/transcribe/apply_model.gif "Application of the text recognition model")

### Manual correction of the transcription
The automatic transcription is now done but you will have to go check it, because a model is not reliable at 100% and you may have to correct some lines.  
Click on the "Edit" button of the first image you selected for the transcription. Make sure that you are on your transcription by checking in the drop-down box in the top-right corner of the page. Once it is done, you can click on the first line and then check, line by line, the transcription and correct it if needed. Press "Enter" to validate the change and go on to the next line.

![image: Correction of the transcription.](img/transcribe/correction.gif "Correction of the transcription")

!!! Note
    To follow the changes made on the transcription line, you can click on it and select "+Toggle history" in which you can see the changes made.

![image: History of the transcription.](img/transcribe/toggle_history.gif "History of the transcription")

## Versions of transcription

### Manage transcription
A document can be associated simultanously to several versions of transcription. Each version has its own name. There is always a default one named "manual". A new version is created as soon as a text recognition model is applied to the document or a transcription is imported. The version is then named after the applied model, the name given to the import or the import name by default, "Zip Import".  
To display the list of versions of transcription available, click on the drop-down menu in the top-right corner and choose the version you want to see.

![image: Versions of transcription.](img/transcribe/transcription_version.gif "Versions of transcription")

To delete a transcription version, click on the "Transcription management" button (blue button with the gear) in the top-right corner. The "Delete" button will delete the chosen version irrevocably for all the images of the document.

![image: Deletion of transcription.](img/transcribe/delete_version.gif "Deletion of transcription")

!!! Warning
    Even when a text recognition model is applied to only part of the images in a document, the entirety of the document-parts will be associated to this new version of the transcription. This means that, even if the display is at document-part level, the creation or **deletion** of a transcription version will impact all the images of the document.

### Compare transcriptions

It is possible to compare several versions of a transcription. To do so, click on the "Transcription management" button (blue button with the gear) in the top-right corner. Choose the versions you want to compare by ticking the checkboxes under "Compare", then close the pop-up box, by clicking on the cross or simply by clicking somewhere on the page. Then, select any line in the "Transcription" pane and click on "+Toggle transcription comparison" to see the difference.  
The parts in red indicate the deleted characters and those in green indicate the added characters.

![image: Comparison of transcriptions.](img/transcribe/transcription_comparison.gif "Comparison of transcriptions")

<!-- todo: move unicode text normalization to a tip page. -->
## Note on unicode text normalization

Unicode normalization is an important parameter to be aware of when creating transcriptions with Kraken and eScriptorium. 

This normalization refer to the way characters are encoded, it can follow different paradigms:

- Decomposed (NFD or NFKD): where ++"è"++ = ++"e"+"`"++
- Composed (NFC or NFKC): where ++"è"++ = ++"è"++

For more information, see Kraken's documentation on [text normalization and unicode](https://kraken.re/master/ketos.html#text-normalization-and-unicode)

When you apply a recognition model set to follow a decomposed normalization, the text typed manually will likely follow the "composed" paradigm, while the text resulting from prediction will fall within the "decomposed" paradigm. Before working with the overall resulting text, you should consider applying a normalization to it first. 
