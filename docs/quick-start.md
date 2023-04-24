---
title: Quickly starting with eScriptorium
summary: About where to start with eScriptorium.
authors:
    - Alix Chagué
date: 2023-04-24
---

!!! warning
    The section needs to be completed.

In this section, we offer a short tutorial which goal is to get you accounted with the interface of eScriptorium and some basic actions that can be performed on the application.

First of all, you need to ensure that you [possess an account](FAQ.md#how-can-i-have-an-escriptorium-account) either on a local installation of eScriptorium or on an online server. Then you can follow the instructions below:

[TOC]

## Forewords on URL syntax

eScriptorium is a decentralized application, meaning it can be deployed on many servers, including on locally simulated servers. In such condition, it is impossible to point to a URL which would work for every person. For this reason, we use what we think is a universal syntax to point to specific URLs: **place holders**. For example, if the eScriptorium application you have access to is located at `escriptorium.demo`, then "escriptorium.demo" is the `base URL` to any pages inside the application. In such a case, you should understand a URL such as `{base_url}/login/` as meaning `escriptorium.demo/login` (the placeholder `{base_url}` is replaced with your base URL). This is also true for local instances of eScriptorium, generally served at `localhost:8000` (where `{base_url}/login/` would be replaced with `localhost:8000/login/`). This syntax is used throughout this documentation.

## Logging into the application

As long as you are not logged in the application, many pages will not be accessible to you. To log in the application, go to your application homepage, and click on "Login", then enter your username and your password. You can find more information about this step [here](walkthrough_users.md#login-and-logout).

![image: scrolling on the homepage of eScriptorium and logging into the application](img/quick_start/browsing_homepage_and_login.gif "Browsing the homepage before logging into the application (v. v0.13.4b)")

After successfully logging in, you are sent to `{base_url}/projects/` which is your overall dashboard. This page can also be accessed by clicking on "My Projects" in the top navigation bar (the link only appears when you are logged in).

## Creating a new project

In eScriptorium, the data is organized inside **projects** which contain **documents**, which in turn contain **document-parts**.
<!-- todo: this section might change if you explain this somewhere else, even though it makes sense to have it explained here -->

- A document-part is simply an image (a digitization) of a document: it can be the photography of a double page, a single page, or even cropped portion of such images. 
- A document is a collection of such images, similar to how you would organize a directory containing images on your file system.
- Projects can be understood as one more level to gather documents (groups of images) together, but they can be envisioned as workspace for a group of users working for the same project. For example, tags <!--todo: add link to page explaining tag when available --> are managed at project level, available for all the documents inside the given project.<!-- todo: send to voc section once there is one -->

You need to have at least one project in your dashboard to create and/or access a document and use eScriptorium's annotation features. Let's create a new project then!

Go to "My Projects" (`{base_url}/projects/`) by clicking on "My Projects" in the nav bar. It will display a list of projects, or an empty page. Now click on the "Create new Project" button: it will open a new page where you can simply type the name of your future project before clicking on "Create". For this tutorial, let's name the project "Sandbox project".

!!! Danger "Before creating a new project"
    Currently, **it is not possible to delete or rename a project**. We strongly advise you to first consider the actual necessity of creating a new project, and secondly to give enough reflection time to choosing the name of your new project. For example, you should avoid names such as "1" or "project" or "blah blah" to make it easier for you identify your projects later, when you will have several projects.  
    Also, note that if you share your project or a document in this project with another user, they will not be able to rename your project and will see the project name you chose: **the name of the project should be meaningful and compatible with sharing it with other users** (avoid such names as "this is my project" for example).

![image: creating a new project in eScriptorium](img/quick_start/create_my_first_project.gif "From the homepage to the project dashboard, where we create a new project (v. v0.13.4b)")

## Creating a new document

As detailed in the [walkthrough](walkthrough.md) section, you can only [import](walkthrough_import.md) images and data inside a document. So, let's now create a document!

To access your project dashboard, go to "My Projects" (`{base_url}/projects/`), then click on the name of your project (it should be "Sandbox project" if you followed the instructions from the previous step). The project dashboard displays a list of documents belonging to the project. It is currently empty since we just created the project. Click on "Create new Document" to open a form and create a new document. 

This form is much more detailed than the one to create a project, but many of these fields are optional:

- **(mandatory) the document's name:** it will be the name of the document as displayed on the project dashboard, you will be able to change it as many time as you want, but you should probably not make it too long. Let's fill it with "Gallery of Fashion (01/1800)".
- **(optional) the main script:** this is an element of metadata, it will not have any impact of the way the document is handled by the application. In the case of our tutorial, we will import a printed document written in English, so we select "Latin": English is written with the Latin alphabet. You could decide to leave it empty.
- **(mandatory) read direction:** you mush choose the reading direction of your document (left to right or right to left). For this tutorial, since the document is in English, we opt for "left to right". This parameter is very important because it will change how eScriptorium handles the reading direction of your [segments](walkthrough_segment.md). <!-- todo: add link to section of segment that would explain what happens when not set correctly -->
- **(mandatory) line offset:** let's set it to "baseline" (if you want more information on this option, see the [segment](walkthrough_segment.md) <!-- todo: add link to section of segment that would normally explain that --> section.)
- **confidence visualization checkbox:** as explained further in the documentation <!-- todo: add a link when the doc exists --> checking this box will slightly change the way the transcription appear in the application. Let's leave it unchecked.
- **(optional) metadata:** this is a series of free fields where you can associate a value to a key. For example, this allows you to keep track of all the annotators working on your document. When [importing images via IIIF](walkthrough_import.md#3-from-iiif), this section of the document is automatically filled with the metadata contained in the IIIF manifest. You can add, remove or modify this section as many times as you want. For now, let's just put the ARK identifier from the French national library, where the images were taken from: "BnF ID" = "ark:/12148/bpt6k10750420"[^1].

[^1]: If you add `https://gallica.bnf.fr/` in front of this value, you will be able to view [the whole document on Gallica](https://gallica.bnf.fr/ark:/12148/bpt6k10750420/), the French national library's online library.

Once you click on "Create", at the bottom of the form, a green message will appear, confirming the creation of the new document. You can modify any information in this form and click on the button now displaying "Update" to save the change.

![image: creating a new document in eScriptorium](img/quick_start/create_my_first_document.gif "From the homepage to a project dashboard, where we create a new document (v. v0.13.4b)")

Before moving on to the next step, make sure your form contain the following information:

![image: screenshot of the form filled with the correction values (name, main script, read direction, line offset, metadata)](img/quick_start/document_description.png "Make sure the form is filled as shown in this image")








## Importing images

<!-- todo: doable only when IIIF import from Gallica will not be so limited that import misses some images... -->
<!--We will use the [IIIF import](walkthrough_import.md#3-from-iiif) feature, but if it does not work correctly for you, you can also download the corresponding images [here](#) -->
<!-- todo: add link to a downloadable .zip file containing images -->
<!-- and follow the documentation on how to [import images from the local file system](walkthrough_import.md#1-from-the-local-file-system). -->
<!-- example images are taken from https://gallica.bnf.fr/iiif/ark:/12148/bpt6k10750420/manifest.json -->

Let's import images [from the local file system](walkthrough_import.md#1-from-the-local-file-system). First, you need to download the file located [here](#)<!-- todo: add link a repo with the demo images -->.


Remaining steps:

- then load images with IIIF (have a backup with locally saved images)
- then apply segmentation
- then download a transcription model (EN ?)
- then correct the segmentation, maybe remove some lines and/or add regions
- verify that the lines are associated with a regions, and verify the reading order
- then apply a transcription model
- then manually correct the transcription
- then export the result with the images

Then point to other useful pages to go further. 
