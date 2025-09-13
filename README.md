## Fork

### Merged patches

- **Bookmarks** (Aug 6, CLOSED)  
  [PR](https://github.com/helix-editor/helix/pull/10905) | [Remote](https://github.com/savente93/helix/tree/master)
- **Go to file position** (Jul 2024, maybe superseded by [PR#8521](https://github.com/helix-editor/helix/pull/8521) ?)  
  [PR](https://github.com/helix-editor/helix/pull/5260) | [Remote](https://github.com/xJonathanLEI/helix/tree/dev/goto_file_pos)
- **Expand selection to whole word when pressing `*`** (Feb 2024, pascalkuthe&mikedavis👍)  
  [PR](https://github.com/helix-editor/helix/pull/6046) | [Remote](https://github.com/magopian/helix/tree/6045-expand-word-boundary-on-search)
- **Selection history (simple)** (Nov 2023)  
  [Issue](https://github.com/helix-editor/helix/issues/1596) | [Commit](https://github.com/helix-editor/helix/compare/master...gertqin:helix:undo-redo-selections)
- **Filter out irrelevant overlays on `gw`** (Apr 2024, maintainers ❌)  
  [PR](https://github.com/helix-editor/helix/pull/10082) | [Remote](https://github.com/perehonchuk/helix/tree/master)
- **Clickable Bufferline** (rebased May 2025, maintainers ∅)  
  [PR](https://github.com/helix-editor/helix/pull/12173) | [Remote](https://github.com/irh/helix/tree/clickable-bufferline)
- **Inline Git Blame** (rebased Aug 2025, mikedavis👍, HUGE)  
  [Issue](https://github.com/helix-editor/helix/pull/13133) | [PR](https://github.com/helix-editor/helix/pull/13133) | [Remote](https://github.com/nik-contrib/helix/tree/gix-blame)
- **Zellij navigation** (Jun 2025)  
  [Remote](https://github.com/g1ibby/helix-zellij-nav)

### Cool stuff
- **Unix Socket support** (Jul 2025, maintainers ∅)  
  [Issue](https://github.com/helix-editor/helix/issues/387) | [PR](https://github.com/helix-editor/helix/pull/13896) | [Remote](https://github.com/shitohana/helix/tree/master)
- **Vim/Neovim Style Tabs** (Apr 2024, maintainers 😐)  
  [Issue](https://github.com/helix-editor/helix/issues/2295) | [PR](https://github.com/helix-editor/helix/pull/7109) | [Remote](https://github.com/nrabulinski/helix/tree/tabs)
- **Sticky Context** (Sep 2024, mikedavis👍, HUGE)  
  [PR](https://github.com/helix-editor/helix/pull/6118) | [Remote](https://github.com/SoraTenshi/helix/tree/sticky-context)
- **View-based Refactoring** (Jul 2025, WIP)  
  [PR](https://github.com/helix-editor/helix/pull/13870) | [Remote](https://github.com/gerblesh/helix/tree/refactor)
- **Icons** (Jul 2025, HUGE)  
  [PR](https://github.com/helix-editor/helix/pull/12369) | [Remote](https://github.com/RoloEdits/helix/tree/icons-v2)
- **Persistent state** (rebased Dec 2024, maintainers ∅, HUGE, CLOSED)  
  [Issue](https://github.com/helix-editor/helix/issues/401) | [PR](https://github.com/helix-editor/helix/pull/9143) | [Remote](https://github.com/intarga/helix/tree/persistent_state)
- **Persistent undo** (Apr 2024, HUGE)  
  [PR](https://github.com/helix-editor/helix/pull/9154) | [Remote](https://github.com/kirawi/helix/tree/undo)
- **Spellcheck**  (mikedavis👍)  
  [Issue](https://github.com/helix-editor/helix/issues/5167)
- **Code folding** (pascalkuthe🤞)  
  [Issue](https://github.com/helix-editor/helix/issues/11660)
- **Harpoon**  
  [Issue](https://github.com/helix-editor/helix/issues/1840)
- **Side-by-side diff**  
  [Issue](https://github.com/helix-editor/helix/issues/405)
- **Resolution of merge conflits**  
  [Issue](https://github.com/helix-editor/helix/issues/5132)

- [**Wezterm IDE**](https://github.com/quantonganh/helix-wezterm)

<div align="center">

<h1>
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="logo_dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="logo_light.svg">
  <img alt="Helix" height="128" src="logo_light.svg">
</picture>
</h1>

[![Build status](https://github.com/helix-editor/helix/actions/workflows/build.yml/badge.svg)](https://github.com/helix-editor/helix/actions)
[![GitHub Release](https://img.shields.io/github/v/release/helix-editor/helix)](https://github.com/helix-editor/helix/releases/latest)
[![Documentation](https://shields.io/badge/-documentation-452859)](https://docs.helix-editor.com/)
[![GitHub contributors](https://img.shields.io/github/contributors/helix-editor/helix)](https://github.com/helix-editor/helix/graphs/contributors)
[![Matrix Space](https://img.shields.io/matrix/helix-community:matrix.org)](https://matrix.to/#/#helix-community:matrix.org)

</div>

![Screenshot](./screenshot.png)

A [Kakoune](https://github.com/mawww/kakoune) / [Neovim](https://github.com/neovim/neovim) inspired editor, written in Rust.

The editing model is very heavily based on Kakoune; during development I found
myself agreeing with most of Kakoune's design decisions.

For more information, see the [website](https://helix-editor.com) or
[documentation](https://docs.helix-editor.com/).

All shortcuts/keymaps can be found [in the documentation on the website](https://docs.helix-editor.com/keymap.html).

[Troubleshooting](https://github.com/helix-editor/helix/wiki/Troubleshooting)

# Features

- Vim-like modal editing
- Multiple selections
- Built-in language server support
- Smart, incremental syntax highlighting and code editing via tree-sitter

Although it's primarily a terminal-based editor, I am interested in exploring
a custom renderer (similar to Emacs) using wgpu or skulpin.

Note: Only certain languages have indentation definitions at the moment. Check
`runtime/queries/<lang>/` for `indents.scm`.

# Installation

[Installation documentation](https://docs.helix-editor.com/install.html).

[![Packaging status](https://repology.org/badge/vertical-allrepos/helix-editor.svg?exclude_unsupported=1)](https://repology.org/project/helix-editor/versions)

# Contributing

Contributing guidelines can be found [here](./docs/CONTRIBUTING.md).

# Getting help

Your question might already be answered on the [FAQ](https://github.com/helix-editor/helix/wiki/FAQ).

Discuss the project on the community [Matrix Space](https://matrix.to/#/#helix-community:matrix.org) (make sure to join `#helix-editor:matrix.org` if you're on a client that doesn't support Matrix Spaces yet).

# Credits

Thanks to [@jakenvac](https://github.com/jakenvac) for designing the logo!
