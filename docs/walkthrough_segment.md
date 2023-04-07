---
title: Segment with eScriptorium
summary: About segmentation features in eScriptorium.
authors:
    - Alix Chagué
date: 2023-04-07
---

# Walkthrough : segment with eScriptorium

!!! warning
    The section needs to be completed.

## Overview of the segmentation panel
The segment editing panel allows you to perform several essential operations:

- Drawing baselines corresponding to the locations of the text on the image in two ways:
    - Free route (not recommended);
    - Point by point plot.
- Adding points on a line (select it then double-click at the point’s location);
- Moving one or more point(s) by a simple select-drag;
- Deleting one or more point(s) on a line;
- Cutting one or more lines using the scissors tool;
- Joining one or more lines;
- Configuring the reading direction of a line;
- Activating the calculation of the polygons associated with each line (this task is automatic and managed asynchronously without any action on the part of the user after the first use).

In this pane, it is also possible to create regions (or zones ) and associate segments to them. A segment located within the perimeter of a region is therefore not automatically associated with it.

All the operations that can be carried out in this panel are detailed in a help window (to display it, click on “?”). It will thus be noted that there are many shortcuts making it possible to simplify all these operations.


<!--## Editing lines

## Editing regions -->

## Reordering
The playback order of the segments is calculated automatically. You can display the order number of each segment from the “Segmentation” panel by clicking on “Toggle ordering display (L)” or from the “Text” panel where the lines are displayed in the following order.

It is possible to modify this order from the “Text” panel by clicking “Toggle sorting mode.” A simple drag and drop of the lines is then enough to carry out the modification.

!!! warning
    It is advisable to ensure the quality of the segmentation before changing the order of the lines because adding or deleting lines systematically restarts the calculation of this order, overwriting manual modifications in the process.