Scriptoria
==========
The source code for the Scriptoria project, a website to track scientific manuscripts
written with distributed revision control systems (RCS) like git and mercurial.

Distributed revision control systems keep the full history of documents, identify
which user is responsible for which change, are safe, and make it easy to fork and modify
scientific output. They are modern tools initially designed to allow
collaboration between several software engineers working on the same code.
Also, websites like github, bitbucket, and gitorious allow users to post "Issues",
essentially a sophisticated and transparent form of peer-review, that can
happen either *during* or *after* the writing process.

Aim of This Project
-------------------
There is currently no easy way to track manuscripts being written on github,
bitbucket, and other servers. The aim of the project is to increase the visibility of
open science developed with distributed revision-control systems (DRCSs) by offering a centralized
database of manuscripts in DRCSs.

As a side-effect, we can also propose best practices for the writing of
manuscripts using RCS. Furthermore, this project can initiate and foster
collaborative research in the scientific community and across disciplines.

Proposed Features
-----------------

* Allow users to add repositories from several common hosting services: github,
bitbucket, gitorious. Perhaps even allow some automatic system based on
a convention (if the repo starts with "ms_", "article_", ... and the user is
registered, then track it).
* Tag the repo by types (manuscript, presentation, thesis, ...) and topic
(machine learning, molecular evolution, ...).
* Use the servers' API to extract basic info on the repo: starting date,
number of commits, participants, branches, issues, DOI.
* Offer a strictly RESTful API.
* Allow authors to inform on the status of their manuscript: where was
it published, etc.

Tools
-----
Scriptoria is written in [Haskell](http://www.haskell.org/) with the
[Yesod](http://www.yesodweb.com/) web framework. The code for the entire
website is available at: https://github.com/PhDP/Scriptoria.

License
-------
[Apache 2.0](http://www.apache.org/licenses/LICENSE-2.0)
