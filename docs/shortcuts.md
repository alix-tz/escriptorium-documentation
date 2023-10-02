---
title: Shortcuts and tips
summary: About shortcuts and tips in eScriptorium
authors:
    - Alix Chagué, Floriane Chiffoleau
date: 2023-10-02
---

# Shortcuts and Tips

There are many features in eScriptorium and thus many buttons. Luckily, some shortcuts exist to facilitate working with the keyboard and avoiding having to click too many times or switch too often between the keyboard and the mouse.

The following page is an attempt to list all the shortcuts available in the application. It does not describe what the feature triggered by the shortcut is: you should envision this page as an advanced documentation for people already somewhat familiar with the application.

The list is distributed into sections corresponding to the pages or panels where the shortcuts can be applied.

!!! Note
    Most shortcuts are documented in the application, when you hover over a button or a clickable item.

!!! Note "URL syntax"
    See the [quick-start](quick-start.md) preamble if you don't know to read the URL described below.

## Images dashboard

Typical URL: `base_url/document/{doc_id}/images/`.

- hold ++shift++ after clicking on a thumbnail checkbox and before clicking on another one: select an interval of document parts

## Edition Page

Typical URL: `base_url/document/{doc_id}/part/{doc_part}/edit/`.

- ++control+arrow-right++ OR ++page-down++: go to the next element (or document-part)
- ++control+arrow-left++ OR ++page-up++: go to the previous element
- ++control+1++: toggle on/off the Metadata panel
- ++control+2++: toggle on/off the Source image panel
- ++control+3++: toggle on/off the Segmentation panel
- ++control+4++: toggle on/off the Transcription panel
- ++control+5++: toggle on/off the Text panel

??? Note "Mac keyboard variants"

    - ++shift+control+arrow-right++ OR ++fn+page-down++: go to the next element (or document-part)
    - ++shit+control+arrow-left++ OR ++fn+page-up++: go to the previous element
    - ++shift+control+1++: toggle on/off the Metadata panel
    - ++shift+control+2++: toggle on/off the Source image panel
    - ++shift+control+3++: toggle on/off the Segmentation panel
    - ++shift+control+4++: toggle on/off the Transcription panel
    - ++shift+control+5++: toggle on/off the Text panel

### Edition Page - Source Image panel

- ++control+backspace++: reset the zoom
- ++right-button+"(hold and drag)"++: move on the zoomed image

If image annotation is available:

- ++escape++: cancel the annotation in progress or cancel the modification
- ++delete++ with an active annotation: delete the annotation

??? Note "Mac keyboard variants"

    - on the Mac trackpad, right click is performed by clicking with two fingers on the right side of the trackpad.
    - ++fn+backspace++ with an active annotation: delete the annotation

### Edition Page - Segmentation panel

The segmentation panel gathers the biggest amount of shortcuts. They are all described in the information pop-up available when clicking on the "?" button, at the top of the panel.

- ++control+backspace++: reset the zoom
- ++right-button+"(hold and drag)"++: move on the zoomed image
- ++escape++ while drawing a line: cancel the drawing and stop drawing
- ++control+z++ after creating, deleting or modifying a line: undo the creation/deletion/edition
- ++control+y++: undo the creation/deletion/edition
- ++control+a++: select all the lines/regions
- ++shift+left-button+"(hold and drag)"++: draw a selection over lines, regions or points
- ++shift+left-button++ (on a line or a region): add or remove a line from the active selection
- ++control+left-button+"(hold and drag)"++ on an active selection: move all the selection together
- ++delete++ with an active selection: delete the selected lines or the regions
- ++control+delete++ with an active selection of points: delete the selected points, but not the whole line or the whole region

- ++r++: switch to region mode or go back to line mode
- ++l++: toggle the display of line order
- ++m++: toggle mask modes
- ++c++: toggle scissor mode, to cut through regions or lines
- ++t++ with an active selection of lines or regions: change the type of the selection (then use NumPad for additional shortcut on type selection)
- ++i++ with an active selection of lines: invert reading direction
- ++j++ with an active selection of at least two lines: join the selection lines into a single segment
- ++y++ with an active selection of lines, and at least one regions drawn on the image: link selected lines to the corresponding background region(s)
- ++u++ with an active selection of lines, and at least one regions drawn on the image: unlink selected lines from their background region(s)

??? Note "Mac keyboard variants"
    
    - on the Mac trackpad, right click is performed by clicking with two fingers on the right side of the trackpad.
    - ++fn+backspace++ with an active selection: delete the selected lines or the regions
    - ++fn+control+backspace++ with an active selection of points: delete the selected points, but not the whole line or the whole region

### Edition Page - Transcription panel

With the transcription pop-up active:

- ++arrow-down++ or ++enter++: save modification and move to the next line
- ++arrow-up++: go to previous line
- ++escape++: close the transcription pop-up

### Edition Page - Text Panel

If text annotation is available:

- ++escape++: cancel the annotation in progress

If sorting mode is activated:

- ++shift+left-button++: select an interval of lines
- ++control+left-button++ add/remove line from the selection

## Virtual Keyboard

It is possible to add key binding in the configuration of the [virtual keyboard](virtual_keyboard.md#customize-a-virtual-keyboard), which are a sort of shortcut. You can use the creation/edition interface for virtual keyboard to manually set the key bindings.
