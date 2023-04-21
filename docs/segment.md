---
title: Segment with eScriptorium
summary: About segmentation features in eScriptorium.
authors:
    - Alix Chagué, Floriane Chiffoleau
date: 2023-04-07
---

# Segment with eScriptorium


## Overview of the segmentation panel

The segment editing panel allows you to perform several essential operations:

- Drawing baselines corresponding to the locations of the text on the image in two ways:
    - Point by point plot;
    - Free route (not recommended).
- Adding points on a line (select it then double-click at the point’s location);
- Moving one or more point(s) by a simple select-drag;
- Deleting one or more point(s) on a line;
- Cutting one or more lines using the scissors tool;
- Joining one or more lines;
- Configuring the reading direction of a line;
- Activating the calculation of the polygons associated with each line (this task is automatic and managed asynchronously without any action on the part of the user after the first use).

In this panel, it is also possible to create regions (or zones ) and associate segments to them. Note that a segment located within the perimeter of a region is not always automatically associated to it.

All the operations that can be carried out in this panel are detailed in a help window (to display it, click on “?”). It will thus be noted that there are many shortcuts making it possible to simplify all these operations.

!!! Note
    The following is a copy of the content of the contextual window appearing when clicking on "?".

- ++left-button++ on the image to create new line, ++right-button++ to **add points** and ++left-button++ again to finish it.
- You can keep the mouse button pressed for free drawing.
- Hitting ++escape++ while drawing a line cancels it.
- If regions matter to you switch to region mode first (++r++).
- when in region mode ++left-button++ to create a new rectangular region, left click again to finish it.
- lines drawn inside a region will automatically be bound to it.
- When the quality of the segmentation is good, you can prompt the system to calculate masks ,
- once a page already has masks new lines will automatically get a mask and - updating a line will also recalculate its mask.
- **Note** that the quality of the masks is highly dependent on the quality of the whole segmentation, not only the corresponding line,
- so make sure to draw all the lines before calculating the masks.
- You can also have the option to calculate the masks en masse in the Images tab -> segment -> choose 'Only masks'.

- ++left-button++ on a line to select it, then you can drag its closest control point.
- **Double click** on the line will create a new control point at the mouse location.
- You can reverse the order of the line's points by selecting a line (or multiple) and using reverse (++i++).
- When in region mode, Regions can be edited the same way.
Selected lines can be linked or unlinked to regions with the corresponding buttons (++y++) (++u++).
- By using the cut mode (++c++) you can cut through lines, splitting them in two or removing part of them.
- If at least two lines are selected a option to join them becomes available (++j++).
You can go through your changes history back and forth with ++ctrl+z++ (undo) and ++ctrl+Y++ (redo) or by using the corresponding buttons .

- ++shift+left-button++ allows to add or remove a line from the selection,
- Clicking on an empty space clears the selection,
- ++shift++ and drag creates a lasso selection tool that allows to select control points (they then appear black).

- **Note:** If lines are already selected the lasso will only select points in those lines.

- ++ctrl++ and drag allows to move all the selected control points at once (or the selected lines if no control points are selected).

- The red trash button deletes all selected lines/regions,
- The yellow trash button only deletes selected control points.

<!--## Editing lines

## Editing regions -->

## Reordering

The playback order of the segments is calculated automatically. You can display the order number of each segment from the “Segmentation” panel by clicking on “Toggle ordering display (L)” or from the “Text” panel where the lines are displayed in the following order.

It is possible to modify this order from the “Text” panel by clicking “Toggle sorting mode.” A simple drag and drop of the lines is then enough to carry out the modification.

!!! warning
    It is advisable to ensure the quality of the segmentation before changing the order of the lines because adding or deleting lines systematically restarts the calculation of this order, overwriting manual modifications in the process.