# Changelog

## v1.0.1 -- 2023-03-31

This is a minor release supporting pydata>=0.13.3, with a few import changes from pydata.

## v1.0.0 -- 2023-03-01

This is a major release that brings in the latest PyData Sphinx Theme and a number of new features with it.
It also overhauls and standardizes the HTML structure of the theme.
Because of this large refactor, we are bumping the major version to `1.0`.
Note that this doesn't imply any new long-term support or stability, we will continue to try not to make major breaking changes but will continue incrementing major versions if we must do so.

### Enhancements made

- PyData Sphinx Theme `v0.13`. See [the PyData Sphinx Theme `v0.13` release notes](https://github.com/pydata/pydata-sphinx-theme/releases/tag/v0.13.0) for details.
- Icon links, more source providers, and bug fixes [#691](https://github.com/executablebooks/sphinx-book-theme/pull/691) ([@choldgraf](https://github.com/choldgraf), [@mmcky](https://github.com/mmcky))
  - **We now support GitHub, GitLab, and BitBucket source providers**.
  - **You can now include lists of icon links in your primary sidebar**.
- Allowing inline elements in sidenotes and marginnotes [#641](https://github.com/executablebooks/sphinx-book-theme/pull/641) ([@AakashGfude](https://github.com/AakashGfude))
- Improve Chinese (Taiwan) and Chinese (China) translation [#585](https://github.com/executablebooks/sphinx-book-theme/pull/585) ([@whyjz](https://github.com/whyjz))
- sphinx >=4,<6 [#644](https://github.com/executablebooks/sphinx-book-theme/pull/644) ([@AakashGfude](https://github.com/AakashGfude))

### Bugs fixed

- FIX: Scroll padding on top for anchor links [#669](https://github.com/executablebooks/sphinx-book-theme/pull/669) ([@choldgraf](https://github.com/choldgraf))
- 🐛 FIX: Correcting a broken link in CHANGELOG.md [#623](https://github.com/executablebooks/sphinx-book-theme/pull/623) ([@AakashGfude](https://github.com/AakashGfude))
- FIX: Scroll to active navigation item [#609](https://github.com/executablebooks/sphinx-book-theme/pull/609) ([@ksuess](https://github.com/ksuess))
- [FIX] Use logo url as is to allow for web urls. [#661](https://github.com/executablebooks/sphinx-book-theme/pull/661) ([@feanil](https://github.com/feanil))

### Maintenance and upkeep improvements

- MAINT: Update pre-commit versions and fix minor bugs in tests [#660](https://github.com/executablebooks/sphinx-book-theme/pull/660) ([@choldgraf](https://github.com/choldgraf))
- MAINT: Move dependabot updates to monthly [#658](https://github.com/executablebooks/sphinx-book-theme/pull/658) ([@choldgraf](https://github.com/choldgraf))
- MAINT: Factor publish to pypi workflow into dedicated file [#645](https://github.com/executablebooks/sphinx-book-theme/pull/645) ([@choldgraf](https://github.com/choldgraf))
- MAINT: Remove duplication with pydata-sphinx-theme [#640](https://github.com/executablebooks/sphinx-book-theme/pull/640) ([@choldgraf](https://github.com/choldgraf))
- MAINT: remove incorrect comment from sphinx pin. [#588](https://github.com/executablebooks/sphinx-book-theme/pull/588) ([@rossbar](https://github.com/rossbar))
- IntersectionObserver at 1/3 screen [#567](https://github.com/executablebooks/sphinx-book-theme/pull/567) ([@choldgraf](https://github.com/choldgraf))

### Documentation improvements

- DOCS: Minor typo correction [#649](https://github.com/executablebooks/sphinx-book-theme/pull/649) ([@bmorris3](https://github.com/bmorris3))
- DOC: Update kitchen sink [#610](https://github.com/executablebooks/sphinx-book-theme/pull/610) ([@choldgraf](https://github.com/choldgraf))

### Breaking changes to structure and API

- UPGRADE/BREAKING: PyData v0.13 and HTML refactoring [#677](https://github.com/executablebooks/sphinx-book-theme/pull/677) ([@choldgraf](https://github.com/choldgraf))
- Remove JQuery and update versions [#668](https://github.com/executablebooks/sphinx-book-theme/pull/668) ([@choldgraf](https://github.com/choldgraf))

### Tips for migration

**Long sidebar entries now wrap**. If you'd like to un-do this and revert to old behavior (where they are cut off if too long), then use the following CSS rule in your custom Sphinx CSS:

```css
.bd-sidebar-primary a {
  word-wrap: unset;
}
```

**`single_page` is deprecated**. If you'd like to restore the old behavior (hiding sidebars), then use the following configuration in your `conf.py`:
```python
html_sidebars = {
    "**": []
}
```

### Contributors to this release

([GitHub contributors page for this release](https://github.com/executablebooks/sphinx-book-theme/graphs/contributors?from=2022-07-17&to=2023-02-19&type=c))


@12rambau ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3A12rambau+updated%3A2022-07-17..2023-03-01&type=Issues)) | @AakashGfude ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AAakashGfude+updated%3A2022-07-17..2023-03-01&type=Issues)) | @akhmerov ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aakhmerov+updated%3A2022-07-17..2023-03-01&type=Issues)) | @AllenDowney ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AAllenDowney+updated%3A2022-07-17..2023-03-01&type=Issues)) | @avivajpeyi ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aavivajpeyi+updated%3A2022-07-17..2023-03-01&type=Issues)) | @bmorris3 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Abmorris3+updated%3A2022-07-17..2023-03-01&type=Issues)) | @choldgraf ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Acholdgraf+updated%3A2022-07-17..2023-03-01&type=Issues)) | @chrisjsewell ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Achrisjsewell+updated%3A2022-07-17..2023-03-01&type=Issues)) | @consideRatio ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AconsideRatio+updated%3A2022-07-17..2023-03-01&type=Issues)) | @dependabot ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Adependabot+updated%3A2022-07-17..2023-03-01&type=Issues)) | @feanil ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afeanil+updated%3A2022-07-17..2023-03-01&type=Issues)) | @fm75 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afm75+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ghutchis ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aghutchis+updated%3A2022-07-17..2023-03-01&type=Issues)) | @guillaume-haerinck ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aguillaume-haerinck+updated%3A2022-07-17..2023-03-01&type=Issues)) | @haklc ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ahaklc+updated%3A2022-07-17..2023-03-01&type=Issues)) | @iasbusi ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aiasbusi+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ivirshup ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aivirshup+updated%3A2022-07-17..2023-03-01&type=Issues)) | @James11222 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AJames11222+updated%3A2022-07-17..2023-03-01&type=Issues)) | @kloczek ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Akloczek+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ksuess ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Aksuess+updated%3A2022-07-17..2023-03-01&type=Issues)) | @martinfleis ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amartinfleis+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mathbunnyru ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amathbunnyru+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mcjulian1107 ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amcjulian1107+updated%3A2022-07-17..2023-03-01&type=Issues)) | @melund ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Amelund+updated%3A2022-07-17..2023-03-01&type=Issues)) | @mmcky ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ammcky+updated%3A2022-07-17..2023-03-01&type=Issues)) | @paugier ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apaugier+updated%3A2022-07-17..2023-03-01&type=Issues)) | @PhilipVinc ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3APhilipVinc+updated%3A2022-07-17..2023-03-01&type=Issues)) | @pradyunsg ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apradyunsg+updated%3A2022-07-17..2023-03-01&type=Issues)) | @pre-commit-ci ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apre-commit-ci+updated%3A2022-07-17..2023-03-01&type=Issues)) | @rkdarst ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Arkdarst+updated%3A2022-07-17..2023-03-01&type=Issues)) | @rossbar ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Arossbar+updated%3A2022-07-17..2023-03-01&type=Issues)) | @scmmmh ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ascmmmh+updated%3A2022-07-17..2023-03-01&type=Issues)) | @sieler ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Asieler+updated%3A2022-07-17..2023-03-01&type=Issues)) | @SilverRainZ ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3ASilverRainZ+updated%3A2022-07-17..2023-03-01&type=Issues)) | @stevepiercy ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Astevepiercy+updated%3A2022-07-17..2023-03-01&type=Issues)) | @trallard ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Atrallard+updated%3A2022-07-17..2023-03-01&type=Issues)) | @whyjz ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Awhyjz+updated%3A2022-07-17..2023-03-01&type=Issues)) | @yuvipanda ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ayuvipanda+updated%3A2022-07-17..2023-03-01&type=Issues)) | @ZedThree ([activity](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AZedThree+updated%3A2022-07-17..2023-03-01&type=Issues))


## v0.3.3 -- 2022-07-17

### Fixes:

- Style edits for last-child zero-margin on dd's [#586](https://github.com/executablebooks/sphinx-book-theme/pull/586) ([@benjaoming](https://github.com/benjaoming))
- Escape colon in JupyterHub link to repo [#556](https://github.com/executablebooks/sphinx-book-theme/pull/556) ([@matthew-brett](https://github.com/matthew-brett))
- Myst-nb pinning to 0.13.2 [#560](https://github.com/executablebooks/sphinx-book-theme/pull/560) ([@choldgraf](https://github.com/choldgraf))
- Stylizing ReadTheDocs in `_readthedocs.scss` as per guidelines [#579](https://github.com/executablebooks/sphinx-book-theme/pull/579) ([@pradyunsg](https://github.com/pradyunsg))
- `templates_path` in config was overriding any value append to `templates_path` in this package. [#566](https://github.com/executablebooks/sphinx-book-theme/pull/566) ([@AakashGfude](https://github.com/AakashGfude))

### Enhancements made:

- Added sidenote and marginnote using footnote syntax [#546](https://github.com/executablebooks/sphinx-book-theme/pull/546) ([@AakashGfude](https://github.com/AakashGfude))

### Docs:

- Added Docs for sphinx-examples [#550](https://github.com/executablebooks/sphinx-book-theme/pull/550) ([@choldgraf](https://github.com/choldgraf))
- Lychee link fixes [#553](https://github.com/executablebooks/sphinx-book-theme/pull/553) ([@choldgraf](https://github.com/choldgraf))
- Beta and lychee link fix [#552](https://github.com/executablebooks/sphinx-book-theme/pull/552) ([@choldgraf](https://github.com/choldgraf))


## v0.3.2 -- 2022-03-28

Two patch releases fixed two bugs for figure content in the margin.

## v0.3.0 - 2022-03-25

This is a significant change in the HTML and CSS of the site, with the goal of making it more standardized and robust. There are several design tweaks that have been made. Here is a short overview:

- The sidebars are now a slightly smaller font, with more padding, to give more attention to the page's content.
- The HTML structure of the site has been re-worked to make `sticky` and other CSS behaviors more dependable.
- The header buttons are now standardized and have an updated look and feel.
- The in-page margin CSS is now more reliable
- Improvements to scrollbar style throughout the site

See the PRs below for where most of these changes occurred.

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.2.0...d9c1abc4197445faab7892291520de448f363274))

### Enhancements made

- ‼️ REFACTOR: HTML and CSS restructuring [#472](https://github.com/executablebooks/sphinx-book-theme/pull/472) ([@choldgraf](https://github.com/choldgraf))
- ENH: Standardize scrollbar behavior [#481](https://github.com/executablebooks/sphinx-book-theme/pull/481) ([@choldgraf](https://github.com/choldgraf))
- ENH: Standardize header buttons [#490](https://github.com/executablebooks/sphinx-book-theme/pull/490) ([@choldgraf](https://github.com/choldgraf))
- ENH: Updating search page style [#491](https://github.com/executablebooks/sphinx-book-theme/pull/491) ([@choldgraf](https://github.com/choldgraf))
- ENH: Add CSS for comments libraries [#524](https://github.com/executablebooks/sphinx-book-theme/pull/524) ([@choldgraf](https://github.com/choldgraf))
- ENH: Add support for ReadTheDocs popup [#518](https://github.com/executablebooks/sphinx-book-theme/pull/518) ([@choldgraf](https://github.com/choldgraf))
- STYLE: Search color highlighting in-line with Jupyter orange [#532](https://github.com/executablebooks/sphinx-book-theme/pull/532) ([@choldgraf](https://github.com/choldgraf))

### ‼️ Breaking changes

This release modifies the HTML structure of some of the major theme sections (in particular, the sidebar and top-bar).
If you had custom CSS or JavaScript that assumed a particular HTML structure, double-check that it still behaves the same way, as you may need to adjust things for the new structure.

## v0.1.10...v0.2.0

This release includes a few under-the-hood and performance improvements to the CSS and HTML of the theme. While there are no major new features, some of these changes have restructured the HTML so double-check your documentation, especially if you had custom CSS rules the sidebar.

Here are a few improvements:

- The right Table of Contents is now hidden using the [Intersection Observer API](https://developer.mozilla.org/en-US/docs/Web/API/Intersection_Observer_API) which will reduce the number of JavaScript calls and improve reliability of this feature. [#448](https://github.com/executablebooks/sphinx-book-theme/pull/448) ([@choldgraf](https://github.com/choldgraf))

- The left sidebar is now toggle-able **only with CSS**, which should make it less prone to failure due to other conflicting javascript on the page. It now includes a "sidebar drawer" on mobile that gives more vertical space for the sidebar. [#454](https://github.com/executablebooks/sphinx-book-theme/pull/454) ([@choldgraf](https://github.com/choldgraf))

- You can now add Deepnote buttons for notebook launch buttons [#385](https://github.com/executablebooks/sphinx-book-theme/pull/385) ([@jakubzitny](https://github.com/jakubzitny))

## v0.1.9 .. v0.1.10

Maintenance release, to remove the unused `click` dependency.

## v0.1.8 .. v0.1.9

This is a minor release to fix a bug that was introduced which broke the right sidebar anchor links.

## v0.1.7 .. v0.1.8

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.7...862632b892f6acd640aa080eb1f50ac6d3de7bc3))

This is a minor release that makes a few bugfixes and small enhancements.

- Printing to PDF from HTML is now formatted more elegantly [#438](https://github.com/executablebooks/sphinx-book-theme/pull/438) ([@AakashGfude](https://github.com/AakashGfude))
- Minor stylistic bugfixes across the theme CSS

## v0.1.6 .. v0.1.7

**Full Changelog**: https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.6...v0.1.7

### Summary

This release primarily updates the pydata theme to bring in a few new theme features and bug-fixes.

### What's Changed
* UPDATE: pydata sphinx theme v0.7.2 by @ocefpaf in https://github.com/executablebooks/sphinx-book-theme/pull/406
* UPDATE: pydata-sphinx-theme 0.7.2 by @kousu in https://github.com/executablebooks/sphinx-book-theme/pull/429
* IMPROVE: translation in the footer for Japanese language by @KengoTODA in https://github.com/executablebooks/sphinx-book-theme/pull/426

## v0.1.5...v0.1.6

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.5...1515334eec40575b0a80c51ce78453ced2ff2484))

### Enhancements made

- Add pst prefix to variables [#413](https://github.com/executablebooks/sphinx-book-theme/pull/413) ([@choldgraf](https://github.com/choldgraf))
- Note TOC level auto-show [#410](https://github.com/executablebooks/sphinx-book-theme/pull/410) ([@choldgraf](https://github.com/choldgraf))
- Add note of margin CSS classes [#405](https://github.com/executablebooks/sphinx-book-theme/pull/405) ([@choldgraf](https://github.com/choldgraf))

## v0.1.5 - 2021-09-23

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.4...c85925c0109a1038994947acb951d1d918a819f8))

### Enhancements made

- Move CSS hash to GET parameter so downstream themes can bust CSS properly [#397](https://github.com/executablebooks/sphinx-book-theme/pull/397) ([@jacobtomlinson](https://github.com/jacobtomlinson))

## v0.1.4 - 2021-09-16

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.3...28358bbc0dc2f1e6e9fff0ac64321685c9edfc00))

### Enhancements made

- ⬆️ UPGRADE: Sphinx v4.0.0 [#364](https://github.com/executablebooks/sphinx-book-theme/pull/364) ([@choldgraf](https://github.com/choldgraf))
- ✨ IMPROVE: Harmonize themes between static and live code [#393](https://github.com/executablebooks/sphinx-book-theme/pull/393) ([@patrickmineault](https://github.com/patrickmineault))
- ✨ IMPROVE: Minor tweaks to footer css [#389](https://github.com/executablebooks/sphinx-book-theme/pull/389) ([@choldgraf](https://github.com/choldgraf))

## v0.1.3 - 2021-08-25

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.2...9a2da30342ace86978ddbd345eb69f5b4479b31c))

### Enhancements made

- ✨ IMPROVE: Add chevrons to prev/next [#386](https://github.com/executablebooks/sphinx-book-theme/pull/386) ([@choldgraf](https://github.com/choldgraf))
- ✨ IMPROVE: Improving accessibility labeling [#375](https://github.com/executablebooks/sphinx-book-theme/pull/375) ([@choldgraf](https://github.com/choldgraf))
- ✨ IMPROVE: improve math styling [#369](https://github.com/executablebooks/sphinx-book-theme/pull/369) ([@akhmerov](https://github.com/akhmerov))

### Bugs fixed

- 🐛 FIX: Fix translation for prev/next [#384](https://github.com/executablebooks/sphinx-book-theme/pull/384) ([@choldgraf](https://github.com/choldgraf))


## v0.1.1...v0.1.2 - 2021-08-06

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.1...v0.1.2))

* 🔧 MAINT: Reduce `full-width` from 136% to 134% [#357](https://github.com/executablebooks/sphinx-book-theme/pull/357):
  This avoid clipping full-width content on certain resolutions
* 🐛 FIX: Dropdown menus on mobile [#367](https://github.com/executablebooks/sphinx-book-theme/pull/367):
  Menus are translated left, so that they are not clipped on small screens

## v0.1.0...v0.1.1

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.1.0...e05def5b9a4fc777f702553a0bcaf7939440dbd3))

### New features added

* Add logo_only theme option [#349](https://github.com/executablebooks/sphinx-book-theme/pull/349) ([@djangoliv](https://github.com/djangoliv))

### Enhancements made

* Add css to highlight searched for phrases [#350](https://github.com/executablebooks/sphinx-book-theme/pull/350) ([@sanjayankur31](https://github.com/sanjayankur31))
* Add logo_only theme option [#349](https://github.com/executablebooks/sphinx-book-theme/pull/349) ([@djangoliv](https://github.com/djangoliv))
* Soften edges in admonitions and remove some ink [#352](https://github.com/executablebooks/sphinx-book-theme/pull/352) ([@choldgraf](https://github.com/choldgraf))

### Bugs fixed

* 🐛 FIX: Path to custom output directory for _sources [#346](https://github.com/executablebooks/sphinx-book-theme/pull/346) ([@dfm](https://github.com/dfm))
* 🐛 FIX: Fixing sidebar animation [#333](https://github.com/executablebooks/sphinx-book-theme/pull/333) ([@choldgraf](https://github.com/choldgraf))

## v0.0.42...v0.1.0

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.42...6320ef6347a77eb91ed67c472b2336fd66d75724))

This updates to the latest PyData Sphinx Theme, which re-works some of the HTML structure (thus, the minor version bump). It also includes some minor fixes to the scrolling and TOC behavior.

### Enhancements made

- ✨ ENH: Adding fullscreen button optional [#328](https://github.com/executablebooks/sphinx-book-theme/pull/328) ([@choldgraf](https://github.com/choldgraf))

### Bugs fixed

- 🐛 FIX: Fixing sidebar scroll [#311](https://github.com/executablebooks/sphinx-book-theme/pull/311) ([@choldgraf](https://github.com/choldgraf))

### API and Breaking Changes

- ⬆ UPGRADE: Pydata Sphinx Theme v0.6.0 [#324](https://github.com/executablebooks/sphinx-book-theme/pull/324) ([@choldgraf](https://github.com/choldgraf))

### Deprecated features

- DEPRECATE: Removing opengraph functionality [#316](https://github.com/executablebooks/sphinx-book-theme/pull/316) ([@choldgraf](https://github.com/choldgraf))

## v0.0.42 2021-03-13

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.41...458fe679ff482a623ec2dd6b13bdd19232069c50))

### Bugs fixed

- 🐛 FIX: hover target bug on right TOC [#300](https://github.com/executablebooks/sphinx-book-theme/pull/300) ([@DrDrij](https://github.com/DrDrij))


## v0.0.41 2021-03-09

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.40...3d9189d889a9be4096ca57859dadf8e11f246a4a))

### Enhancements made

- The Table of Contents titles is now configurable. See [#299](https://github.com/executablebooks/sphinx-book-theme/pull/299) ([@AakashGfude](https://github.com/AakashGfude))
- The left sidebar has a drawer-style layout on mobile. See [#298](https://github.com/executablebooks/sphinx-book-theme/pull/298) ([@DrDrij](https://github.com/DrDrij))

## v0.0.40 - 2021-02-27

([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.39...4ab518e211163a52f01562912ce6e41548a734d1))

### New features added

- Added tag for cell-input [#259](https://github.com/executablebooks/sphinx-book-theme/pull/259) ([@AakashGfude](https://github.com/AakashGfude))
- Add a shadow to header, on scroll [#255](https://github.com/executablebooks/sphinx-book-theme/pull/255) ([@pradyunsg](https://github.com/pradyunsg))
- Add CSS to center align images with class [#292](https://github.com/executablebooks/sphinx-book-theme/pull/292) ([@DrDrij](https://github.com/DrDrij))

### Enhancements made

- Add footnote translations [#274](https://github.com/executablebooks/sphinx-book-theme/pull/274) ([@chrisjsewell](https://github.com/chrisjsewell))

### Bugs fixed

- translation of suggest edit [#284](https://github.com/executablebooks/sphinx-book-theme/pull/284) ([@chrisjsewell](https://github.com/chrisjsewell))
- Pin bs4 and sphinx dependencies [#271](https://github.com/executablebooks/sphinx-book-theme/pull/271) ([@chrisjsewell](https://github.com/chrisjsewell))
- fixing right toc whitespace overlap [#268](https://github.com/executablebooks/sphinx-book-theme/pull/268) ([@choldgraf](https://github.com/choldgraf))
- Fixing linenos style [#263](https://github.com/executablebooks/sphinx-book-theme/pull/263) ([@AakashGfude](https://github.com/AakashGfude))


## v0.0.39 - 2020-11-08
([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.38...v0.0.39))

### New features added
* sphinx sidebars functionality [#233](https://github.com/executablebooks/sphinx-book-theme/pull/233) ([@choldgraf](https://github.com/choldgraf)). You can now use the `html_sidebars` functionality that is native in Sphinx. [See the sidebars documentation](https://sphinx-book-theme.readthedocs.io/en/latest/sections/sidebar-primary.html).
* Collapsible lists in sidebars [#226](https://github.com/executablebooks/sphinx-book-theme/pull/226) ([@AakashGfude](https://github.com/AakashGfude)). Sidebars that have nested sections will now have an arrow that allows you to reveal these sections without changing the current page. You can [control the depth](https://sphinx-book-theme.readthedocs.io/en/latest/sections/sidebar-primary.html#control-the-depth-of-the-left-sidebar-lists-to-expand) of expanded sections with `show_navbar_depth`.

### Enhancements made
* Option for download button [#245](https://github.com/executablebooks/sphinx-book-theme/pull/245) ([@bknaepen](https://github.com/bknaepen)). The "download" button used to be automatically added, but can now be removed. See [the download button configuration](https://sphinx-book-theme.readthedocs.io/en/latest/components/download.html).

## v0.0.38

## Enhancements made
👌 IMPROVE: Add missing aria-label to fullscreen button [#228](https://github.com/executablebooks/sphinx-book-theme/pull/228) ([@foster999](https://github.com/foster999))

👌 IMPROVE: declare parallel read safe [#225](https://github.com/executablebooks/sphinx-book-theme/pull/225) ([@rscohn2](https://github.com/rscohn2))

🐛 FIX: fixing dirhtml builds [#230](https://github.com/executablebooks/sphinx-book-theme/pull/230) ([@choldgraf](https://github.com/choldgraf))

🐛 FIX: fixing margin for code blocks [#229](https://github.com/executablebooks/sphinx-book-theme/pull/229) ([@choldgraf](https://github.com/choldgraf))


## v0.0.37

✨ NEW: Sphinx translations for all buttons and tooltips in major UI elements. See [the Sphinx i18n documentation](https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-language) for how to activate other languages. [#214](https://github.com/executablebooks/sphinx-book-theme/pull/214) ([@chrisjsewell](https://github.com/chrisjsewell))

⬆️  UPGRADE: pydata-sphinx-theme v0.4.0. See [the `pydata-sphinx-theme` changelog](https://github.com/pandas-dev/pydata-sphinx-theme/releases/tag/v0.4.0) for more information.

⬆️ UPGRADE: Use pyScss instead of libsass for scss compilation. This should make the theme more lightweight to install and develop locally. [#200](https://github.com/executablebooks/sphinx-book-theme/pull/200) ([@hason](https://github.com/hason))


### Contributors to this release
([GitHub contributors page for this release](https://github.com/executablebooks/sphinx-book-theme/graphs/contributors?from=2020-08-25&to=2020-09-28&type=c))

[@choldgraf](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Acholdgraf+updated%3A2020-08-25..2020-09-28&type=Issues) | [@chrisjsewell](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Achrisjsewell+updated%3A2020-08-25..2020-09-28&type=Issues) | [@fm75](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Afm75+updated%3A2020-08-25..2020-09-28&type=Issues) | [@hason](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Ahason+updated%3A2020-08-25..2020-09-28&type=Issues) | [@najuzilu](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Anajuzilu+updated%3A2020-08-25..2020-09-28&type=Issues) | [@nathancarter](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Anathancarter+updated%3A2020-08-25..2020-09-28&type=Issues) | [@pauleveritt](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apauleveritt+updated%3A2020-08-25..2020-09-28&type=Issues) | [@pradyunsg](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apradyunsg+updated%3A2020-08-25..2020-09-28&type=Issues) |

## v0.0.36 2020-08-25

👌 IMPROVED: The main theme change in this release, is the addition of CSS styling for definition lists, including those created by [sphinx.ext.autodoc](https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html).
See [Definition and Field Lists](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/lists.html), and the [Python API documentation](https://sphinx-book-theme.readthedocs.io/en/latest/reference/kitchen-sink/api.html).

🔧 MAINTENANCE: Under the hood, there has also been work undertaken to improve the development environment for working with the package. Thanks to [@pradyunsg](https://github.com/pradyunsg).

### Contributors to this release

[@chrisjsewell](https://github.com/chrisjsewell) | [@pradyunsg](https://github.com/pradyunsg)

## v0.0.34...v0.0.35
([full changelog](https://github.com/executablebooks/sphinx-book-theme/compare/v0.0.34...v0.0.35))

### Enhancements 👌

* Change "On this page" -> "Contents" [#159](https://github.com/executablebooks/sphinx-book-theme/pull/159) ([@pradyunsg](https://github.com/pradyunsg))
* Use consistent font size in toc [#157](https://github.com/executablebooks/sphinx-book-theme/pull/157) ([@pradyunsg](https://github.com/pradyunsg))
* Consistent font size in navigation [#156](https://github.com/executablebooks/sphinx-book-theme/pull/156) ([@pradyunsg](https://github.com/pradyunsg))

### Bugs fixed 🐛

* backref superscript [#171](https://github.com/executablebooks/sphinx-book-theme/pull/171) ([@AakashGfude](https://github.com/AakashGfude))
* Fixing sidebar overlap on narrow screens [#167](https://github.com/executablebooks/sphinx-book-theme/pull/167) ([@choldgraf](https://github.com/choldgraf))
* Fixing jupyterhub urls [#166](https://github.com/executablebooks/sphinx-book-theme/pull/166) ([@choldgraf](https://github.com/choldgraf))
* Create parent folders, when adding notebook to sources [#152](https://github.com/executablebooks/sphinx-book-theme/pull/152) ([@pradyunsg](https://github.com/pradyunsg))

### Documentation improvements 📚

* Adding contributing docs [#163](https://github.com/executablebooks/sphinx-book-theme/pull/163) ([@choldgraf](https://github.com/choldgraf))

### Contributors to this release

([GitHub contributors page for this release](https://github.com/executablebooks/sphinx-book-theme/graphs/contributors?from=2020-08-05&to=2020-08-10&type=c))

[@AakashGfude](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3AAakashGfude+updated%3A2020-08-05..2020-08-10&type=Issues) | [@choldgraf](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Acholdgraf+updated%3A2020-08-05..2020-08-10&type=Issues) | [@chrisjsewell](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Achrisjsewell+updated%3A2020-08-05..2020-08-10&type=Issues) | [@pradyunsg](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Apradyunsg+updated%3A2020-08-05..2020-08-10&type=Issues) | [@welcome](https://github.com/search?q=repo%3Aexecutablebooks%2Fsphinx-book-theme+involves%3Awelcome+updated%3A2020-08-05..2020-08-10&type=Issues)
