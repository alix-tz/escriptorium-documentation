---
title: eScriptorium Tutorial - FAQ
summary: Frequently asked questions about eScriptorium.
authors:
    - Alix Chagué
date: 2023-02-22
---

# Frequently asked questions about eScriptorium

???+ Tip "Missing answers!"
    Feeling like we missed an important question? See how to [contribute](contribute.md) to this tutorial and submit your idea!

[TOC]

---

## How can I have an eScriptorium account?  

!!! Note
    The text in this section cites eScriptorium's FAQ:  

    ➡️ [https://gitlab.com/scripta/escriptorium/-/wikis/How-can-I-get-an-account-on-eScriptorium%3F](https://gitlab.com/scripta/escriptorium/-/wikis/How-can-I-get-an-account-on-eScriptorium%3F)

> eScriptorium is provided as Free and Open Source Software, not as a service. This means that there is no one eScriptorium site, but instead there are many different servers running the software which have been set up by different people in different institutions. To use eScriptorium, then, you can either set up an installation yourself (for which see [Deploying eScriptorium](https://gitlab.com/scripta/escriptorium/-/wikis/Deploying)) or find an existing one and ask the owners for access. Unfortunately we don’t know all the different installations because, again, eScriptorium is entirely free and open source, so people can and do install it without any connection to us and often without even telling us that they are using it.
>  
> The advantage of this is that the software is truly free and open, meaning that you can download and use it yourself on your own servers, and this in turn means that that you will not be dependent on us (unlike most other systems). This makes the whole system more sustainable, and it also means that if we change anything in future in a way that you do not accept then you are still free to continue without us. For instance, if some day we find that we can no longer sustain our own instance of eScriptorium, this would have no impact on you running it on your own servers. However, the disadvantage is that installing the software is not trivial, and realistically it needs a high-performance computing cluster if you want to train your own material, which normally you do, and this makes it harder for people without institutional support.

## Who is responsible for this documentation/tutorial?

This tutorial was created by users of eScriptorium, not by the [creators of eScriptorium](#who-is-responsible-for-escriptorium).  

!!! Tip "More info"  
    ➡️ See [About](about.md)

## Who is responsible for eScriptorium?

!!! Note
    The text in this section cites eScriptorium's FAQ:  

    ➡️ [https://gitlab.com/scripta/escriptorium/-/wikis/Who-is-responsible-for-eScriptorium%3F](https://gitlab.com/scripta/escriptorium/-/wikis/Who-is-responsible-for-eScriptorium%3F)

> eScriptorium is an Open Source project and so it has a number of contributors and partners around the world. However, the project is hosted and lead by the Digital Humanities team at the [École Pratique des Hautes Études – Université Paris Sciences et Lettres](https://ephe.psl.eu/), in [AOROC](http://www.archeo.ens.fr/) in Paris. This core team comprises:
> 
> - [Daniel Stökl Ben Ezra](https://www.ephe.psl.eu/daniel-stoekl-ben-ezra) (Co-Director)
> - [Peter Stokes](https://www.ephe.psl.eu/peter-stokes) (Co-Director)
> - Benjamin Kiessling (machine vision engineer, responsible for [Kraken](https://kraken.re/))
> - Robin Tissot (lead project engineer for eScriptorium)
> 
> In addition to this are several other contributors, including a team from [Teklia](https://teklia.com/), and from the [Open Islamicate Texts Initiative](https://openiti.org/) at the University of Maryland and Northeastern University, among others.
>
> If you have questions or need help then you can try contacting us (follow the links for the names above to find contact details), but a more effective means might be to join [our community on Gitter](https://gitter.im/escripta/escriptorium) and ask your questions there.
>
> Finally, if you want to contact the eScriptorium team then please do not use the 'Contact' form on the website, as this goes to the local admins for the site and not to us (see [I contacted you via the eScriptorium website: why didn't you reply?](https://gitlab.com/scripta/escriptorium/-/wikis/I-contacted-you-via-the-eScriptorium-website:-why-didn't-you-reply%3F)).

## Is eScriptorium accessible offline?

If you use an instance of eScriptorium hosted on a web server, no, you cannot access eScriptorium offline.

If you use a [local deployment](https://gitlab.com/scripta/escriptorium/-/wikis/docker-install) of eScriptorium (installed on your machine and hosted by a virtual server), yes, you can access eScriptorium offline.

## Can I synchronize a local eScriptorium application with a server?

eScriptorium is a decentralized software, which means that there are as many databases as there are instances of eScriptorium. It is impossible to synchronize two instances, unless they share the same database, which is unlikely.

You can, however, update the content of your projects and documents from one instance to another with the help of the [export](walkthrough_export.md) and [import](walkthrough_import.md) features. For this, you need to have an account on both the source and the target instances.

## Who can I contact to request a new feature or signal a bug?

If you want to provide feedback on the application, you can contact the eScriptorium developer team with their [Gitter community](https://gitter.im/escripta/escriptorium). You can also open [tickets](https://gitlab.com/scripta/escriptorium/-/issues) in the Gitlab repository hosting the source code of the application. If you want to offer a bug fix or contribute to the project, you can check the ["Contributing" page](https://gitlab.com/scripta/escriptorium/-/wikis/contributing).

!!! Note
    If you use eScriptorium on a server, we recommend identifying and contacting the owners of the application/server before reporting a bug to the eScriptorium development team. They may have deactivated some already existing features or be aware of a bug caused by the infrastructure rather than the application itself.

## Where can I find more documentation in eScriptorium? Is there a documentation in another language?

A listing of known existing documentations on eScriptorium is available here: [escriptorium-doc-finder](https://github.com/alix-tz/escriptorium-doc-finder)

It intends to cover documentation in all available languages. If you know of other resources not listed there, you should consider adding it, even if you were not its creator.

## I made my own documentation for eScriptorium, where can I reference it?

You could reference your documentation in the [listing of known existing documentations](https://github.com/alix-tz/escriptorium-doc-finder) on eScriptorium.

Additionally, you could also compare your documentation with the current tutorial and [suggest editions](contribute.md) if you think we missed something important. It's the beauty of a collaborative documentation!  

## How can I contribute to eScriptorium?  

You can check the ["Contributing" page](https://gitlab.com/scripta/escriptorium/-/wikis/contributing) in the wiki of the eScriptorium's Gitlab repository.

## What is onboarding? How can I reset it?

Onboarding is a mini tutorial explaining the basics of eScriptorium to new users. It will take the form of several boxes highlighting and documenting certain areas of the interface.  

Any user can reset onboarding by going into their profile and clicking "Reset onboarding".

!!! Tip "More info"  
     For more information on the Profile page, see [user-related features](walkthrough_users.md)
