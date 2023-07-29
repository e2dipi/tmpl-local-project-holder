# README - Local Projects' Holder

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
<i>This template provides a folder hierarchy for holding one or more projects sharing common
resources.  Its versatile structure is suitable for all sorts of projects, regardless of their size,
complexity, or nature. It is not meant to be used as a repository template, but rather as a template
for a local folder structure that will contain one or more repositories. Note that it is not to be
confused with a mono-repo either since its root folders are not meant to be versioned. The
contents of the <code style="font-style: normal">/workspace(s)</code> folder, however, may consist of one or more repositories.</i>
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
<div>
<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=6 orderedList=false} -->
<details open style="margin: 14pt 0pt 24pt 10pt">
<summary style="margin-left: -8pt; font-weight: bold; font-size: larger; font-variant: small-caps">
<span style="margin-left: 3pt">Table of contents<span></summary>

<!-- code_chunk_output -->

- [Installation](#installation)
- [Structure and Contents](#structure-and-contents)
- [Roadmap](#roadmap)
- [Authors and acknowledgment](#authors-and-acknowledgment)
- [License](#license)

<!-- /code_chunk_output -->

</detail>
</div>

## Installation

As it is not meant to be used as a repository, this template is not saved as a *GitHub template* and,
 therefore, cannot be used to [instantiate a new repository](https://tinyurl.com/z427byf6).
 Instead, it is meant to be downloaded and used as a local folder structure template. To do so,
 simply download the latest release from the [releases page](https://tinyurl.com/4f3ekkzb) and
 extract it to the desired location. Alternatively, you can clone the repository and remove the `.git`
 folder<sup>1</sup> as well as all the files and folders that are not needed: the structure you should
 end up with contains only folders and `.gitkeep` files and is shown in the tree of the next section.
 Also, the `workspace(s)` folder should be renamed to singular or plural form according to the
 number of workspaces the project will contain.

<ol style="font-style: italic; padding-left: 10pt">
  <li>
      <p>
        Note that the <code>.git</code> folder is hidden by default. You may need to enable the
        display of hidden files and folders in your file explorer to see it. Alternatively, you can use the
        following command to remove it.
      </p>
      <ul style="font-style: italic; padding-left: 10pt">
        <li>In a <code>Bash terminal</code>:
          <pre style="color:inherit; margin-top: 5pt">rm -rf .git</pre>
        </li>
        <li>In a <code>PowerShell terminal</code>:
          <pre style="color:inherit; margin-top: 5pt">Remove-Item -Recurse -Force .git</pre>
        </li>
      </ul>
  </li>
</ol>

## Structure and Contents

Each folder of the template contains a `.gitkeep` file containing a description of its purpose. In
addition, the folder `resources/manuals` contain several documents describing in more detail certain
aspects of the template and its usage, and suggesting some best practices and conventions.

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

### Highlights

Note that not all the folders come empty past their `.gitkeep` file. Some of them contain additional
information that is worth mentioning here:

- Default assets are provided in the `resources/assets` folder. There are two sets, each of which is
  located in a subfolder of the `user-interface` assets folder:
    1. The [e2d2ipi logos](resources/assets/user-interface/e2d2ipi/) are available in various shapes
        and colors, including ready-to-use *favicons* bundles.
    2. The full collection of [Octicons](resources/assets/user-interface/octicons/), which are available
        in `SVG`` format.

- Various manuals about VSCode and some of its extensions are provided in the
  `resources/manuals` folder. They are available in *Markdown* format to be read in *VSCode* itself,
  using the *Markdown Preview Enhanced* extension. Alternatively, they can be read and converted
  to *HTML* or *PDF* using that same extension or any other dedicated tool.

- Guidelines and best practices are provided in the `resources/guidelines` folder. As the manuals
above, they are available in *Markdown* format and, thus, can be either read in *VSCode* or
converted to another format. At the time of writing, two guidelines are provided:
    1. A detailed discussion on how archives should be handled and, in particular, on how they should
        be named and organized is available
        [here](admin/guidelines/handling-archives/handling-archives.md).
    2. A brief presentation of the recommended Git Branching Model to be used. The corresponding
        document is available [here](admin/guidelines/git-branching/git-branching-model.md).

## Roadmap

Planned features and improvements as well as known issues and other topics of interest concerning
this template's development status and roadmap are embedded in its `.gitkeep` files in the form of
[Todo Tree](https://tinyurl.com/fy452sjj) comments. They can be viewed in the *Todo Tree* panel of
[Visual Studio Code](https://code.visualstudio.com/) by installing the *Todo Tree* extension and
opening the template's root folder in *Visual Studio Code*'s
[index workspace.](vscode-index.code-workspace)

Note that, due to the custom tags that were used and that are defined in that latter file, opening this
template exactly as just described is mandatory to get an exhaustive view of all the *Todo Tree* tags
that this project contains.

For the record, let's list here the most important entries anyway:

- [ ]  Implement the deployments' scripts.
- [ ]  Create type-specific (*JavaScript*, *TypeScript*, *NodeJS*, *GAS*, *LaTex*, etc ...)  templates
- [ ]  Embed the templates mentioned above as
[GitHub Submodules](https://tinyurl.com/2tykz6wr) in the [workspace(s)](workspace(s)/.gitkeep)
folder.

## Authors and acknowledgment

- [S. Picozzi](https://github.com/e2d2ipi) &nbsp;-&nbsp; *Initial work*

## License

This project is licensed under the **MIT License** &nbsp;-&nbsp; *see the
file [LICENSE.md](./LICENSE.md) for details.*

<!-- CHECK Make sure that all @@-Tags  were either replaced or deleted with their
associated contents. Delete this comment only once this is done! [template]  -->
