<!-- markdownlint-disable MD024 MD051 -->
# Change Log - *Local Project Template*
<!--
-------------------------------------------------------------------------------------------------------------------------------------
___  HEADER     _______________________________________________________________
---------------------------------------------------------------------------------------------------------------------------->

All notable changes to this project will be documented in this file.

!!!hint ""
    The format is based on
    [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)<sup>&nbsp;1</sup>,
    <br/>
    and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

</div>
<ol class="note">
<li> To the exception of the <span class="note"><code>Improved</code></span> type, which is not part of the original specification.</li>
</li>
</ol>

<!-- @import "[TOC]" {cmd="toc" depthFrom=2 depthTo=2 orderedList=false} -->
<details open id="toc">
<summary>
<span>List of versions<span></summary>

<!-- code_chunk_output -->

- [1.0.0 &nbsp;-&nbsp; 2023-08-04](#100httpsgithubcome2d2ipitmpl-local-project-holdercomparev000v100-nbsp-nbsp-2023-08-04)
- [Seed &nbsp;-&nbsp; 2023-07-22](#seedhttpsgithubcome2d2ipitmpl-local-project-holderreleasestagv000-nbsp-nbsp-2023-07-22)

<!-- /code_chunk_output -->

</details>

<!--
-------------------------------------------------------------------------------------------------------------------------------------
___  TEMPLATES     ____________________________________________________________
-----------------------------------------------------------------------------------------------------------------------------
Note. The "Unreleased" template is NOT preceded by a [Toc] link (due to the fact that it is the
first entry in the file ... and because its positioning would be different). Therefore, the link must
be added when the version is released (see "Compared / Tag-only Versioned Header" below).

UNRELEASED VERSION (includes the bottom separator line)
´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´
## [Unreleased](https://github.com/e2d2ipi/tmpl-local-project-holder/compare/...HEAD)

### Added

- ...

### Changed

- ...

### Improved

- ...

### Deprecated

- ...

### Removed

- ...

### Fixed

- ...

### Security

- ...

-------------------------------------------------------------------------------------------------------------------------------------

COMPARED VERSIONED HEADER
´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´
<a class="toc" title="&uarr; Table Of Contents &uarr;" href="#toc">[&nbsp;Toc&nbsp;]</a>

## [<vers>](https://github.com/e2d2ipi/tmpl-local-project-holder/compare/<to-that>...<this>) &nbsp;-&nbsp; <yyy-mm-dd>

- - -

TAG-ONLY VERSIONED HEADER
´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´
<a class="toc" title="&uarr; Table Of Contents &uarr;" href="#toc">[&nbsp;Toc&nbsp;]</a>

## [<vers>](https://github.com/e2d2ipi/tmpl-local-project-holder/releases/tag/<the-tag>) &nbsp;-&nbsp; <yyy-mm-dd>

<!--
-------------------------------------------------------------------------------------------------------------------------------------
___ CHANGELOG   ____________________________________________________________
-----------------------------------------------------------------------------------------------------------------------------
NEW  VERSION  CHECKLIST  (!!! Release Brsnch !!!)
´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´
The first 3 steps below should be taken  on the `develop` branch,
BEFORE  the `telease` branch is created.

  [   ]  COPY-PASTE the desired header  in place of the "[Unreleased](...)" one

  [   ]  UPDATE the new header with the release's <version>, <tag(s)> and <date>.

  [   ]  REPLACE [Unreleased] by the last release's next version

The next steps should be done on the `develop` branch, but only
AFTER the `release` branch is created (optional, but recommended).

  [   ]  CHECK OUT the `develop` branch

  [   ]  CREATE a new [Unreleased] entry on top

The step below finalizes the release's changelog. It should be the last commit on the `release`
branch before the final merge happens.

  [   ]  MODIFY the comparison settings from `...HEAD` to `<last-vers-tag>...<new-vers-tag>`

-->

## [1.0.0](https://github.com/e2d2ipi/tmpl-local-project-holder/compare/v0.0.0...v1.0.0) &nbsp;-&nbsp; 2023-08-04

### Added

- A VSCode Workspace [configuration file](./vscode-index.code-workspace)

<!--!!! .BAK -->

- A `.bak` environment to host the project's [backups and archives](/.bak/.gitkeep)
  - An `archives` subfolder to hold the [project's archives](./.bak/archives/.gitkeep)
  - A `.history` folder to hold the development's [continuous backups](./.bak/.history/.gitkeep)

<!--!!! @REL -->

- An `@rel` environment for exposing the [project's releases](./@rel/.gitkeep)
  - An `archives` sufolder to hold the [project's releases](./@rel/archives/.gitkeep)

<!--!!! DEPLOY -->

- A `deploy` environment to host the project's [deployment tools](/deploy/.gitkeep)

<!--!!! ADMIN -->

- An `admin` environment to host [administrative tools and documents](./admin/.gitkeep)
  - An `audit` subfolder to hold the [project's audits](./admin/audits/.gitkeep)
  - A `guidelines` subfolder to hold the [project's guidelines](./admin/guidelines/.gitkeep)
    - Guidelines concerning [archives](./admin/guidelines/handling-archives/handling-archives.md)
    - Guidelines concerning [Git workflows](./admin/guidelines/git-branching/git-branching-model.md)
  - A `todo&notes` subfolder to hold the [project's todo lists and notes](./admin/todo&notes/.gitkeep)

<!--!!! RESOURCES -->

- A `resources` environment for the user to hold its [personal tools and rss](./resources/.gitkeep)

  <!--!! Assets  -->
  - An `assets` foder to hold the [user's shared assets](./resources/assets/.gitkeep)
    - A `css` subfolder to hold the [user's styling assets](./resources/assets/css/.gitkeep)
    - An `execs` subfolder to hold the [user's executable assets](./resources/assets/execs/.gitkeep)
    - A `images` subfolder to hold the [user's images assets](./resources/assets/images/.gitkeep)
    - A `libraries` subfolder to hold the [user's libraries assets](./resources/assets/libraries/.gitkeep)
    - A `multimedia` subfolder to hold the [user's multimedia assets](./resources/assets/multimedia/.gitkeep)
      - An `audio` subfolder to hold the [user's audio media assets](./resources/assets/multimedia/audio/.gitkeep)
      - A `videos` subfolder to hold the [user's video media assets](./resources/assets/multimedia/videos/.gitkeep)
    - A `to-download` subfolder to hold the [user's downloadable assets](./resources/assets/to-download/.gitkeep)
    - A `user-interface` subfolder to hold the [user's ui-related assets](./resources/assets/user-interface/.gitkeep)
      - An [`e2d2ipi.$$$` placeholder](./resources/assets/user-interface/e2d2ipi.$$$/) to be replaced by a symlink pointing to the e2-logos as `.png` files and as [favicons packages](https://realfavicongenerator.net/)
      - An [`octicons.$$$` placeholder](./resources/assets/user-interface/octicons.$$$/) to be replaced by a symlink pointing to the [octicons](https://primer.style/octicons/) collection in `.svg` format

  <!--!! Manuals -->
  - A `manuals` foder to hold the [user's manuals and tutorials](./resources/manuals/.gitkeep)
    - A `.src` folder to hold the [user's manuals sources](./resources/manuals/.src/.gitkeep)
    - A [mini-guide](./resources/manuals/vscode-custom-features) on how to exploit certain VSCode editor extensions in the context of this template
    - A mini-guide on the VSCode Editor features in [markdown format](./resources/manuals/vscode-custom-features/vscode-custom-features.md)

  <!--!! Templates -->
  - A `templates` foder to hold the [user's templates and models](./resources/templates/.gitkeep)
    - Various templates: [Assets folder and standard repo files](./resources/templates/.gitkeep)

  <!--!! Useful tools -->
  - A `tuseful-tools` foder to hold the [user's useful tools and utilities](./resources/useful-tools/.gitkeep)

  <!--!! Worth keeping -->
  - A `worth-keeping` foder to hold the [user's worth-keeping stuff](./resources/worth-keeping/.gitkeep)

  <!--!! External resources -->
  - An `xternal-resources` folder to hold the user's resources that are [maintained by third parties](./resources/xternal-resources/.gitkeep)
    - An `xternal-css` subfolder to hold [external styling assets](./resources/xternal-resources/xternal-assets/xternal-execs/.gitkeep)
    - An `xternal-execs` subfolder to hold [external executable assets](./resources/xternal-resources/xternal-assets/xternal-execs/.gitkeep)
    - An `xternal-images` subfolder to hold [external images assets](./resources/xternal-resources/xternal-assets/xternal-images/.gitkeep)
    - An `xternal-libraries` subfolder to hold [external libraries assets](./resources/xternal-resources/xternal-assets/xternal-libraries/.gitkeep)
    - An `xternal-multimedia` subfolder to hold [external multimedia assets](./resources/xternal-resources/xternal-assets/xternal-multimedia/.gitkeep)
      - An `xternal-audio` subfolder to hold [external audio media assets](./resources/xternal-resources/xternal-assets/xternal-multimedia/xternal-audio/.gitkeep)
      - An `xternal-videos` subfolder to hold [external video media assets](./resources/xternal-resources/xternal-assets/xternal-multimedia/xternal-videos/.gitkeep)
    - An `xternal-to-download` subfolder to hold [external downloadable assets](./resources/xternal-resources/xternal-assets/xternal-to-download/.gitkeep)
    - An `xternal-user-interface` subfolder to hold [external ui-related assets](./resources/xternal-resources/xternal-assets/xternal-user-interface/.gitkeep)
      - An `e2d2ipi` subfolder to hold the [e2d2ipi logos](./resources/xternal-resources/xternal-assets/xternal-user-interface/e2d2ipi/.gitkeep) in various shapes and colors, and as both `.png` files and [favicons packages](https://realfavicongenerator.net/)
      - An `octicons` subfolder to hold the full [Octicons](./resources/xternal-resources/xternal-assets/xternal-user-interface/octicons/.gitkeep) collection ìn `.svg` format (the orignal sources are available [here](https://primer.style/octicons/))

    <!--!! External Manuals -->
    - An `xternal-manuals` folder to hold [external manuals](./resources/xternal-resources/xternal-manuals/.gitkeep)
    - An `xternal-templates` folder to hold [external templates](./resources/xternal-resources/xternal-manuals/.gitkeep)
      - An `xternal-open-src-licenses` subfolder to hold templated copies of the main [open-source licenses](./resources/xternal-resources/xternal-templates/xternal-open-src-licenses/.gitkeep)
    - An `xternal-useful-tools` folder to hold [external useful tools](./resources/xternal-resources/xternal-useful-tools/.gitkeep)
    - An `xternal-worth-keeping` folder to hold [external worth keeping documents](./resources/xternal-resources/xternal-worth-keeping/.gitkeep)

<!--!!! WORKSPACES -->

- A `workspace(s)` environment to host the project and subprojects [directories](./workspaces/.gitkeep)
  - Two `.gitkeep` described subfolders mocking subprojects.

-------------------------------------------------------------------------------------------------------------------------------------

<a class="toc" title="&uarr; Table Of Contents &uarr;" href="#toc">[&nbsp;Toc&nbsp;]</a>

## [Seed](https://github.com/e2d2ipi/tmpl-local-project-holder/releases/tag/v0.0.0) &nbsp;-&nbsp; 2023-07-22

<!-- markdownlint-disable MD024 MD051 -->
<!--
-------------------------------------------------------------------------------------------------------------------------------------
___  [ x ]  INSTALLATION  CHECKLIST     __________________________________________
----------------------------------------------------------------------------------------------------------------------------

[   ]  COPY / MOVE the template to `/CHANGELOG.md` (at repo's root-level)

[   ]  UPDATE the document's title (e.g. "Change Log - My Project")

[   ]  REPLACE https://github.com/e2d2ipi/tmpl-local-project-holder to the actual repository's URL.
       There are 5 instances of it:
        [   ]  3x in the TEMPLATE section
        [   ]  1x in the [0.0.0] vesion
        [   ]  1x in the [Unreleasd] vesion

[   ]  SET the [Seed] version's date to the project's start date

 [   ]  ADD the v0.0.0 tag to the commit tree

[   ]  DONE. Move this checklist at the bottom of this file (or deleting it)

-->

<style>
  .admonition {
    width: 300pt;
    font-size:95%;
    margin-left:50pt;
  }

  a.toc {
    position: relative;
    display: inline-block;
    top: 6ex;
    left: 21em;
    padding-left: 20pt;
    font-size:75%;
    font-weight:400;
  }

  hr {
    top: 2.5ex;
    width: 96%;
    left: 1%;
    position: relative;
  }

  ul {
    padding-bottom: 5pt;
  }

  ul li {
    margin-left: -12pt;
    padding-top: 3pt;
  }

  ol.note {
    font-size:75%;
    padding-left: 10pt;
    margin-bottom:20pt;
  }

  span.note {
    font-size: 110%
  }

  code.note {
    font-size: 110%
  }

  #toc {
    font-size:95%;
    margin-bottom:20pt;
    margin: 14pt 0pt 32pt 10pt
  }

  #toc summary {
    margin-left: -8pt;
    margin-bottom:2pt;
    font-weight: bold;
    font-size: 110%;
    font-variant: small-caps;
    font-weight:500
  }

  #toc span {
    margin-left: 3pt;
  }

  #toc li {
    margin-left: -3pt;
    padding-top: 0pt;
  }
</style>
