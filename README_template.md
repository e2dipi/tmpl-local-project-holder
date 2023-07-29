# README - @@PROJECT_NAME

---

<div style="
    font-size: normal;
    margin: 0 auto 5ex auto;
    width: 40em;"
>
<div style="font-size: 95%; text-align: justify;">
<div style="
  font-size:135%;
  text-align: center;
  font-weight: bold;
  margin: 0 0 .75ex 0;
  font-variant: small-caps;"
>Abstract</div>
<div style="text-align: justify">
<i>@@PROJECT_ABSTRACT

This folder is not meant to be a versioned repository, but rather as a local folder structure that will
itself contain one or more repositories. Note that it is not to be confused with a mono-repo either
since its root folders are not meant to be versioned. The contents of the `workspace(s)` folder,
however, *may* be versioned by itself or contain multiple subfolders, each of which being a
mono-repo, a multi-repo or a simple folder.</i>
</div></div></div>
<div style="
   width: 100%;
   text-align: center;
    margin-bottom: 5ex;"
>

[![GitHub issues](https://img.shields.io/github/issues/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/issues)
[![GitHub forks](https://img.shields.io/github/forks/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/network)
[![GitHub stars](https://img.shields.io/github/stars/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/stargazers)
[![GitHub license](https://img.shields.io/github/license/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/blob/main/LICENSE.md)

</div>

<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=false} -->
<details open style="margin: 14pt 0pt 24pt 10pt">
<summary style="margin-left: -8pt; font-weight: bold; font-size: larger; font-variant: small-caps">
<span style="margin-left: 3pt">Table of contents<span></summary>

<!-- code_chunk_output -->

- [Project's Description](#projects-description)
- [Project's Shell Structure](#projects-shell-structure)
- [Project's Roadmap and TODOs](#projects-roadmap-and-todos)
- [Projects' Authors and Acknowledgment](#projects-authors-and-acknowledgment)

<!-- /code_chunk_output -->

</detail>

## Project's Description

@@POJECT_DESCRIPTION

## Project's Shell Structure

Each folder of the template that was used to instantiate this project contains a `.gitkeep` file
containing a description of its purpose. In addition, the folder `resources/manuals` contain several
documents describing in more detail certain aspects of the template and its usage, and suggesting
some best practices and conventions.

As a quick overview, and a reference of the template's structure once the unnecessary files and
folders have been removed, the following tree shows the structure of the template:

<div style="min-width: 45em; font-size: normal; margin: 0 10% 5ex 5%;">

```tree


   .                               PROJECT'S ROOT FOLDER
   |                               ``````````````````````
   ├── .bak                        # Project's Backup and Archives
   |   ├── .history                  # Continous backups
   |   ├── archive                   # The project's main archives
   |   └── ...                       # Temporary backups
   |
   ├── deploy                       # Deployment Environement(s)
   |   ├── ...                        # Sufolders and files ...
   |   └── .gitkeep                   # Describres the deploy folder purpose
   |
   ├── @rel                         # Exposes the (sub)project(s) latest release(s)
   |   ├── ...                        # Sufolders and files ...
   |   └── .gitkeep                   # Describres the deploy folder purpose
   |
   ├── resources                    # Project's Resources
   |   ├── ...                        # Sufolders and files ...
   |   └── .gitkeep                   # Describres the resources folder purpose
   |
   ├── workspace(s)                 # Project's Workspace(s)
   |   ├── ...                        # Sufolders and files ...
   |   └── .gitkeep                   # Describres the workspace(s) folder purpose
   |
   └── .gitkeep                     # Describres the template's core structure

```

</div>

## Project's Roadmap and TODOs

Planned features and improvements as well as known issues and other topics of interest concerning
this template's development status and roadmap are embedded in its `.gitkeep` files in the form of
[Todo Tree](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree)
comments. They can be viewed in the *Todo Tree* panel of
[Visual Studio Code](https://code.visualstudio.com/) by installing the *Todo Tree* extension and
opening the template's root folder in *Visual Studio Code* using the file named
[vscode-index.code-workspace](vscode-index.code-workspace) and located at the root of this
template's folder.

Note that, due to the custom tags that were used and that are defined in that latter file, opening this
template exactly as just described is mandatory to get an exhaustive view of all the *Todo Tree* tags
that this project contains.

For the record, let's list here the most important entries anyway:

- [ ]  @@ROADMAP_ENTRY_1, if applies
- [ ]  @@ROADMAP_ENTRY_2, if applies
- [ ]  etc ...

## Projects' Authors and Acknowledgment

- **@@AUTHOR_NAME** - *Initial work* - [@@USER_NAME](https://github.com/@@USER_NAME)

<!-- CHECK Make sure that all @@-Tags  were either replaced or deleted with their associated contents. Delete this comment only once this is done! [template]  -->
