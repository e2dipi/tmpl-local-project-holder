# README - *Local Project Template*

<div style="
    font-size: normal;
    margin: 0 auto 5ex auto;
    width: 40em;"
>
<div style="font-size: 95%; text-align: justify;">
  <div style=" font-size:135%; text-align: center; font-weight: bold; margin: 0 0 .75ex 0;
                     font-variant:  small-caps;">
    Abstract </div>
  <div style="text-align: justify">
  <i>This template provides a folder hierarchy for holding one or more projects sharing common resources.  Its versatile structure is suitable for all sorts of projects, regardless of their size, complexity, or nature. It is not meant to be used as a repository template, but rather as a template for a local folder structure that will contain one or more repositories. Note that it is not to be confused with a mono-repo either since its root folders are not meant to be versioned. The contents of the <code style="font-style: normal">/workspace(s)</code> folder, however, may consist of one or more repositories.</i>
    </div>
  </div>
</div>
<div style="width: 100%; text-align: center; margin-bottom: 5ex;" >

[![GitHub issues](https://img.shields.io/github/issues/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/issues)
[![GitHub forks](https://img.shields.io/github/forks/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/network)
[![GitHub stars](https://img.shields.io/github/stars/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/stargazers)
[![GitHub license](https://img.shields.io/github/license/e2d2ipi/tmpl-projects-root-folder.svg)](https://github.com/e2d2ipi/tmpl-projects-root-folder/blob/main/LICENSE.md)

</div>
<div>

<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=3 orderedList=false} -->
<details open style="margin: 14pt 0pt 24pt 10pt" id="toc-details">
<summary style="margin-left: -8pt; font-weight: bold; font-size: larger; font-variant: small-caps">
<span style="margin-left: 3pt">Table of contents<span></summary>

<!-- code_chunk_output -->

- [Installing the Template](#installing-the-template)
  - [1. Remove the `.git` folder and the `.gitignore` file](#1-remove-the-git-folder-and-the-gitignore-file)
  - [2. Update the project-specific files](#2-update-the-project-specific-files)
  - [3. Linked Folders & Files](#3-linked-folders--files)
- [Highlights](#highlights)
- [Roadmap](#roadmap)
- [Contributors](#contributors)
- [Project's License](#projects-license)

<!-- /code_chunk_output -->

</detail>
</div>

## Installing the Template As it is not meant to be used as a repository, this template is not saved as a *GitHub template* and, therefore, cannot be used to [instantiate a new repository](https://tinyurl.com/z427byf6). Instead, it is meant to be downloaded and used as a local folder structure template. To do so, download the latest release from the [releases page](https://github.com/e2dipi/tmpl-local-project/releases), extract it at the desired location rename the resulting folder to the name of your project. Once done, the template still needs some cleaning up and customization before it can be used. The following steps are recommended:

### 1. Remove the `.git` folder and the `.gitignore` file The template is a repository itself and, therefore, contains a `.git` folder and a `.gitignore` file that need to be removed. Both are located in the root folder of the template. Note that the `.git` folder is hidden by default, so you may need to enable the display of hidden files and folders in your file explorer to see it. Alternatively, you can remove both files using the following commands:

- In a `Bash terminal`:

<div style="width: 38em; margin: -5pt auto 15pt 25pt">

  ```bash rm -rf .git*
  ```

</div>

- In a `PowerShell terminal`:

<div style="width: 38em; margin: -5pt auto 15pt 25pt">

  ```powershell Remove-Item -Recurse -Force .git*
  ```

  </div>

### 2. Update the project-specific files The template contains a few files that describe the template itself and should be either replaced by the files of your project or deleted. To help you create these files, models are available in the [resources/templates](resources/templates) folder. Placeholders, if any, are marked as `@@<placeholder-name>@@` and should be replaced by the corresponding value. Specific instructions are provided in the `.gitkeep` file of each folder. <div style="width: 90%; margin: 24pt auto; " id="toc-details">

> <div style="padding: 10pt; font-weight: bold; text-align: center; ">Placeholders, if any, are marked as <code>@@&lt;placeholder-name&gt;</code> and should be replaced by the corresponding value. When relevant, additional instructions are provided in the <code>.gitkeep</code> file of each folder.</div>

</div>

 The files to be replaced (or deleted) are:

- [ ] `LICENSE`: the main open-source licenses are available in [this folder](resources/templates/licenses).

- [ ] `README.md`: various templates are provided in [this folder](resources/templates/repo-standard-files/readme-templates).

- [ ] `CHANGELOG.md`: a template is provided in [this folder](resources/templates/repo-standard-files/seeding-files-templates).

### 3. Linked Folders & Files The template contains a few folders that are meant to be replaced by symbolic links pointing to other locations (or deleted). These folders and their associated target locations are listed below. More information may be found in `!!!___REPLACE-ME___!!!` (markdown) file that each of them contains. The procedure to create a symbolic link is described after the list of folders. <div style="width: 90%; margin: 24pt auto; ">

> <div style="padding: 10pt; font-weight: bold; text-align: center; ">The folders to be replaced all have a <code>.$$$</code> sufifix that is meant to be replaced by the rather standard <code>.lnk`</code> extension.</div>

</div>

Note that if you are using VSCode and have the [Folder Path Color](https://tinyurl.com/2pajtxjn) extension installed, these folders will be colored in <span style="color: magenta">magenta</span> and marked with a <span style="color: magenta">$$</span> symbol.

#### Deployments' targets The first two folders are located in the `deploy/` environment and are meant to be replaced by *Symlinks* pointing to the folders where the deployments' targets are located. These subfolders are:

- [ ] [new-release@rel/targ-env.$$$](deploy/new-release@rel) should point to the [@rel](@rell) folder, at the root of the template.

- [ ] [production@host/targ-env.$$$](deploy/production@host) should point to the production environment's folder, if any.

#### External assets The template's hierarchy provides a special folder to store the resources that are maintained outside of the project itself and expects its contents to be linked to where they are expected to be found using *Symlinks* when consisting of files. The concerned folders are all located in `resources/assets/user-interface` and are meant to point to the corresponding subfolder of `/xternal-user-interface`, within `xternal-resources/xternal-assets/`. More specifically:

- [ ] [e2d2ipi.&dollar;&dollar;&dollar;](resources/assets/user-interface/e2d2ipi.$$$) should point to the [e2d2ipi](resources/xternal-resources/xternal-assets/xternal-user-interface/e2d2ipi) folder, and

- [ ] [octicons.&dollar;&dollar;&dollar;](resources/assets/user-interface/e2d2ipi.$$$) should point to the [octicons](resources/xternal-resources/xternal-assets/xternal-user-interface/e2d2ipi) folder.

#### External Templates Finally, the open-source licenses that are provided as templates are also considered to be external resources and, thus, need to be linked to. As for the assets above, the concerned folders are all located in the same parent folder, namely `resources/templates/open-src-licenses`, and are expected to point to the corresponding children of the `xternal-open-src-licenses` folder located within `xternal-resources/xternal-templates/`. More specifically:

- [ ] [apache-v2.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/apache-v2.$$$) should point to the [apache-2.0](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/apache-v2) folder, and

- [ ] [boostsoft-v1.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/boostsoft-v1.$$$) should point to the [boostsoft-v1](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/boostsoft-v1) folder, and

- [ ] [gnu-agpl-v3.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/gnu-agpl-v3.$$$) should point to the [gnu-agpl-v3](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/gnu-agpl-v3) folder, and

- [ ] [gnu-gpl-v3.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/gnu-gpl-v3.$$$) should point to the [gnu-gpl-v3](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/gnu-gpl-v3) folder, and

- [ ] [gnu-lgpl-v3.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/gnu-lgpl-v3.$$$) should point to the [gnu-lgpl-v3](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/gnu-lgpl-v3) folder, and

- [ ] [mit.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/mit.$$$) should point to the [mit](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/mit) folder.

- [ ] [mozilla-public-v2.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/mozilla-public-v2.$$$) should point to the [mozilla-public-v2](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/mozilla-public-v2) folder.

- [ ] [the-unlicense-v1.&dollar;&dollar;&dollar;](resources/templates/open-src-licenses/the-unlicense-v1.$$$) should point to [the-unlicense-v1](resources/xternal-resources/xternal-templates/xternal-open-src-licenses/the-unlicense-v1).

#### Creating Symbolic Links

*Symbolic Links* or, for short, *Symlinks* are a native feature on Unix, Linux and macOS, but not on Windows. On the former, they can be created using the `ln` command in a `Bash terminal` and can be used to link both files and folders. On Windows,  they can only be used to link files. Their equivalent for folders is called a *Junction* and can be created only on `NTFS` partitions. The commands to create such links on the different platforms are:

- On Unix, Linux and macOS:

<div style="width: 38em; margin: -5pt auto 15pt 25pt">

  ```bash ln -s <target> <link-name>
  ```

</div>

- *Symlink* on Windows:

<div style="width: 38em; margin: -5pt auto 15pt 25pt">

  ```powershell New-Item -ItemType SymbolicLink -Path <link-name> -Target <target>
  ```

</div>

- *Junction* on Windows:

<div style="width: 38em; margin: -5pt auto 15pt 25pt">

  ```powershell New-Item -ItemType Junction -Path <link-name> -Target <target>
  ```

</div>

An alternative to the above commands on Windows is to install the [ln.exe](https://schinagl.priv.at/nt/ln/ln.html) utility, which provides a `ln` command that can be used in a `PowerShell terminal` to create *Symlinks*, *Junctions*, *Hardlinks* and combinations thereof. Finally, for those who prefer a *GUI* to the command line, the [Link Shell Extension](https://schinagl.priv.at/nt/hardlinkshellext/linkshellextension.html) brings all the features of the `ln.exe` utility to the Windows Explorer by adding a `Pick Link Source` and a `Drop As...` entries to the context menu of files and folders.

## The Template's Core Structure The tree below shows the template's core structure. It shows only folders and is limited to the first two levels of the hierarchy, but it is exhaustive and provides a brief description of the purpose of each folder. Note that each folder of the template contains a `.gitkeep` file containing a description of its purpose. In addition, the folder `resources/manuals` contain several documents describing in more detail certain aspects of the template and its usage, and suggesting some best practices and conventions. <div style="width: 43em; margin: 20pt 0">

``` tree .                                 ROOT FOLDER (Project's name)
   |                                 ´´´´´´´´´´´´´´´´´´´´´´´´´´´´
   ├─ .bak                            # The project's backups and archives
   |  ├── .history                      # Local-history extension folder
   |  └── archives                      # The project's main archives
   |
   ├─ @rel                            # Stores and exposes the main releases
   |  └── archives                      # Archives the project's main releases
   |
   ├─ admin                           # The administrative environment
   |  ├── audits                        # Autits scripts and reports
   |  ├── guidelines                    # Development best practices and conventions
   |  └── todo&notes                    # User's personal nores and todo lists
   |
   ├─ deploy                          # The deployment environment
   |  ├── .cmds                         # Common commands and scripts
   |  ├── .config                       # Common configuration parameterrs
   |  ├── .source                       # The sourcefiles to be deployed (typically a release)
   |  ├── archives                      # An archive containing a copy of every deployed version
   |  ├── new-release@rel               # An env. for deploying a new release to the @rel targer
   |  └── production@host               # Mimics an env. for deploying to a remote production host
   |
   ├─ resources                       # The user's personal development's resources
   |  ├── assets                        # A library of assets or assets' generators
   |  ├── manuals                       # Stores useful info including mans, tutos and refs
   |  ├── templates                     # Hosts templates, models, snippets, etc...
   |  ├── useful-tools                  # The user's personal tools, utilities and scripts
   |  └── worth-keeping                 # Set aside code fragments, staged devs, worhy ideas, etc...
   |
   └─ workspace(s)                    # The user's personal development's resources
      ├── a-subprojetc                  # A library of assets or assets' generators
      └── another-subproject            # A library of assets or assets' generators

```

</div>

## Highlights Note that not all the folders come empty past their `.gitkeep` file. Some of them contain additional information that is worth mentioning here:

- Various templates including seeding files and structured directories are provided in the `resources/templates` folder, including a `README` template to be used for instances of the present model. A brief description of each of them is available in the latter folder's `.gitkeep` file.  <br/>[Click  to open](/resources/templates/.gitkeep)

- Manuals about VSCode and some of its extensions are provided in the `resources/manuals` folder. They are available in *Markdown* format to be read in *VSCode* itself, using the *Markdown Preview Enhanced* extension. Alternatively, they can be read and converted to *HTML* or *PDF* using that same extension.<br/>[Click to open](/resources/manuals/vscode-custom-features/vscode-custom-features.doc.md)

- Guidelines and best practices are provided in the `resources/guidelines` folder. As the manuals above, they are available in *Markdown* format and, thus, can be either read in *VSCode* or converted to another format. At the time of writing, two guidelines are provided:<br/>1. &nbsp;A detailed discussion on how archives should be named and organized. <br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Click to open](./admin/guidelines/handling-archives/handling-archives.md)<br/>2. &nbsp;A brief presentation of the recommended Git Branching Model to be used.<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;[Click to open](./admin/guidelines/git-branching/git-branching-model.md).

## Roadmap Planned features and improvements as well as known issues and other topics of interest concerning this template's development status are embedded in its `.gitkeep` files in the form of [Todo Tree comments](https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree). The most important ones are also listed here for convenience:

- [ ]  Implement the deployments' scripts.
- [ ]  Create type-specific (*JavaScript*, *TypeScript*, *NodeJS*, *GAS*, *LaTex*, etc ...)  templates
- [ ]  Embed the templates mentioned above as [GitHub Submodules](https://tinyurl.com/2tykz6wr) in the [workspace(s)](workspace(s)/.gitkeep) folder.

## Contributors

- [S. Picozzi](https://github.com/e2d2ipi) &nbsp;-&nbsp; *Initial work*

## Project's License This project is licensed under the **MIT License** &nbsp;-&nbsp; *see the file [LICENSE](./LICENSE) for details.*
