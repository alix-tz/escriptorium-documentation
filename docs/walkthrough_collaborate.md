---
title: Collaborate within eScriptorium
summary: About features related to collaboration in eScriptorium.
authors:
    - Hugo Scheithauer, Alix Chagué
date: 2023-02-09
---

# Walkthrough: collaborate within eScriptorium

This walkthrough details features related to collaboration in eScriptorium.

## Teams

Users can be grouped by Teams. The main purpose of a team is to facilitate [sharing documents or projects](#share-a-project-or-a-document). Teams are also helpful to identify a group of people working on the same project or coming from the same institution.  

It is possible to manage teams from the [Profile page](walkthrough_users.md). Team management includes:  

- Creating a team,  
- Leaving a team,  
- Adding or removing members from a team,  
- Transfering ownership to another member.  

Only the owner of a team is allowed to add or remove members or to transfer ownership. The owner of a team cannot leave it without first transferring the ownership to another user.

??? Note "No deleting, no renaming"
    It is currently impossible to delete a team or to rename a team.

??? Note "One owner per team"
    There can only be one owner at a time.

## Invite a user

eScriptorium allows you to invite new users to your instance.

You can find more information about inviting new users in the [user-related features walkthrough](walkthrough_users.md#Invite) section.

## Share a project or a document

You can share projects and documents to others users of your eScriptorium instance.

### Share a project

You can share an opened project you own by clicking on the "Share this project" button. It will then open a pop-up box where you have two options:

- A form in which you can enter any username existing on your eScriptorium instance,
- Or a succession of tick boxes associated to usernames belonging to the team you are a part of. You can check as many boxes as you want.

Then you can click on the "Share" button.

!!! Note
    You can stop sharing a project in the same pop-up box by unchecking tick boxes associated to usernames.

### Share a document

Go to a document you own and that you want to share, and then click on the "Description" tab. You can then click on the "Share this document" button, and the same pop-up box used for sharing a project will open.

## Share a model

eScriptorium allows you to share your models with other users of your eScriptorium instance.

To do so, go to the "My Models" page, accessible via the navigation bar, in the upper right section of the interface, or via `{base_url}/models/`.

You can share a model for which you are the owner with the share button. Once clicked, it will open a new URL, `{base_url}/models/{your model's number}/rights/`, where you can choose to share a model to users from the teams you belong to, or to a whole team.

To share a model, choose an user or a team from either one of the two dropdown menus, and click on the "Add right" button.

All users or teams you shared the model to are also listed here. Users will have the `User` type, and teams the `Group` type. You also have the name of the user or the team, and the full name or identifier.

!!! Note
    You can stop sharing a model to a specific user or team by clicking on the "Stop sharing" button.

![image: Sharing a model from the "My Models" page, to a team](img/collaborate/escriptorium_collaborate_share_model.gif "Sharing a model to a team")