---
title: Search in eScriptorium
summary: About the search feature in eScriptorium.
authors:
    - Alix Chagué
date: 2023-01-31
---

# Walkthrough : search in eScriptorium

!!! warning
    The section needs to be completed.

## Activate search

By default, Search is deactivated on eScriptorium. This is because the feature relies on ElasticSearch, which may not be compatible with every set up. It is up to the administrator of the website to decide whether or not to activate Search on the application.

If you run eScriptorium on your own machine and want to activate the Search feature, you can take a look at corresponding the [developer documentation](https://gitlab.com/scripta/escriptorium/-/wikis/Environment-variables#search-with-elasticsearch-).

When Search is activated, it appears as a search bar in the middle of the navigation bar, at the top of the page.

![image: Screenshot of the search bar](img/search/search_bar.png "The search bar is located in the navigation bar.")

## Use search

You can start a quick search using the search bar in the navigation bar, or you can access to more advance search interface via `{base_url}/search/`.

A search query can be performed in all the projects at once, or inside only one project. 

- if you start a query from any page but a project's page, the query will be launched on all of your project.
- if you start a query from a page inside a project, the querry will by default be launched on that project only.
- the 'advance" search page allows you to set this parameter ("`All Projects`" or "`{project_name}`)

A transcription is not immediately available to search since it needs to be indexed by ElasticSearch. For this reason, you shouldn't expect the query to return anything if you have just uploaded your transcription or applied a transcription model.

The results of the query will be displayed as a list of text extracts along with the corresponding line of text. 

<!-- todo: complete this documentation once I can actually run a successfull query... -->

