<!-- markdownlint-disable MD024 MD051 -->
# Change Log - *@@PROJECT_NAME@@*
<!--
-------------------------------------------------------------------------------------------------------------------------------------
___  [   ]  INSTALLATION  CHECKLIST     __________________________________________
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

- [Unreleased](#unreleasedrepo-urlcomparehead)
- [Seed &nbsp;-&nbsp; <yyy-mm-dd>](#seedrepo-urlreleasestagv000-nbsp-nbsp-yyy-mm-dd)

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

### Fixed

- ...

### Security

- ...

### Removed

- ...

### Deprecated

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

NEW  VERSION  CHECKLIST
´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´´
The first 3 steps below should be taken  on the `develop` branch,
BEFORE  the `telease` branch is created.

  [   ]  COPY-PASTE the desired header  in place of the "[Unreleased](...)" one

  [   ]  UPDATE the new header with the release's <version>, <tag(s)> and <date>.

  [   ]  REPLACE [Unreleased] by the last release's next version

The next step should be done on the `develop` branch, but only
AFTER the `release` branch is created (optional, but recommended).

  [   ]  CHECK OUT the `develop` branch

  [   ]  CREATE a new [Unreleased] entry on top

The step below finalizes the release's changelog. It should be the last commit on the `release`
branch before the final merge happens.

  [   ]  MODIFY the comparison settings from `...HEAD` to `<last-vers-tag>...<new-vers-tag>`

-->

## [Unreleased](<repo-url>/compare/...HEAD)

### Added

- ...

### Changed

- The [.gitignore](/.gitignore) file was rfined.
- The [LICENCE](/LICENSE) was updated with the needed information.
- The [README](/README.md) file was updated to a detailed project description.

### Removed

- ...

### Security

- ...

-------------------------------------------------------------------------------------------------------------------------------------

<a class="toc" title="&uarr; Table Of Contents &uarr;" href="#toc">[&nbsp;Toc&nbsp;]</a>

## [Seed](<repo-url>/releases/tag/v0.0.0) &nbsp;-&nbsp; <yyy-mm-dd>

### Added

- A basic [.gitignore config](/.gitignore) file.
- A copy of an [Open Source LICENCE](/LICENSE).
- A brief description of the project in a @@[README file](/README.md) file.

<!-- markdownlint-disable MD024 MD051 -->

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
</style>
