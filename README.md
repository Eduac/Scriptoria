drcs-science
============
Ideas on a potential project to build a central website that tracks
manuscripts being written with distributed revision-control systems (git,
mercurial, ...).

Name
----
*The Open Scriptorium* ?

Why use Revision Control Systems for Open Science?
--------------------------------------------------
RCS keeps the full history of the documents, identify which user is responsible for which change, are safe, makes it easy to fork
and modify scientific output. It *was* made for collaboration after all.
Also, websites like github, bitbucket, and gitorious allow users to post
"Issues", essentially a sophisticated and transparent form of peer-review, that can happen either *during* or *after* the writing of the manuscript.

Aim of This Project
-------------------
There is currently no easy way to track manuscripts being written
on github, bitbucket, and other servers.

The aim of the project is to increase the visibility of open science with
distributed revision-control systems.

As a side-effect, we can also propose best practices for the writing of manuscripts using RCS.

How
---
The system should, at the very least, do the following:

* Allow users to add repositories from several common hosting services: github,
bitbucket, gitorious. Perhaps even allowing some automatic system based on
a convention (if the repo starts with "ms_", "article_", ... and the user is
registered, then track it).
* Tag the repo by types (manuscript, presentation, thesis, ...) and content
(machine learning, molecular evolution, ...).
* Use the servers' API to extract basic info on the repo: starting date,
number of commits, participants, branches, issues, DOI.
* Offer a strictly RESTful API.
* Allow the developper to inform on the status of the manuscript: where was
it published, etc.

What
----
Tools:

* Yesod web framework (Haskell): fast, safe & fun.
* Open identification system.
* MySQL? pgSQL?
* 100% open source: the code should be stored on gitorious (more neutral than github).
