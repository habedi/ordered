## Ordered

<div align="center">
  <picture>
    <img alt="Ordered Logo" src="logo.svg" height="25%" width="25%">
  </picture>
</div>
<br>

[![Tests](https://img.shields.io/github/actions/workflow/status/habedi/ordered/tests.yml?label=tests&style=flat&labelColor=282c34&logo=github)](https://github.com/habedi/ordered/actions/workflows/tests.yml)
[![Code Coverage](https://img.shields.io/codecov/c/github/habedi/ordered?label=coverage&style=flat&labelColor=282c34&logo=codecov)](https://codecov.io/gh/habedi/ordered)
[![CodeFactor](https://img.shields.io/codefactor/grade/github/habedi/ordered?label=code%20quality&style=flat&labelColor=282c34&logo=codefactor)](https://www.codefactor.io/repository/github/habedi/ordered)
[![License](https://img.shields.io/badge/license-MIT-007ec6?label=license&style=flat&labelColor=282c34&logo=open-source-initiative)](https://github.com/habedi/ordered/blob/main/LICENSE)
[![Zig Version](https://img.shields.io/badge/Zig-0.14.1-orange?logo=zig&labelColor=282c34)](https://ziglang.org/download/)
[![Release](https://img.shields.io/github/release/habedi/ordered.svg?label=release&style=flat&labelColor=282c34&logo=github)](https://github.com/habedi/ordered/releases/latest)

---

Ordered Zig library includes implementations of popular data structures including B-tree, skip lists, tries, and
red-black tree.

> [!IMPORTANT]
> This library is in very early stages of development and is not yet ready for serious use.
> The API is not stable and may change frequently.
> Additionally, it's not thoroughly tested or optimized so use it at your own risk.

### Features

- Implementations for common data structures that maintain the order of keys:
    - [`BTreeMap`](src/btree_map.zig): A balanced tree map that maintains order of keys.
    - [`OrderedSet`](src/sorted_set.zig): A set with ordered elements.
    - [`SkipList`](src/skip_list.zig): A probabilistic data structure that allows fast search, insertion, and deletion.
    - [`Trie`](src/trie.zig): A prefix tree for fast retrieval of keys with common prefixes.
    - [`RedBlackTree`](src/red_black_tree.zig): A self-balancing binary search tree that maintains order of keys.

---

### Getting Started

To be added.

### Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to make a contribution.

### Logo

The logo is from [SVG Repo](https://www.svgrepo.com/svg/469537/zig-zag-left-right-arrow).

### License

This project is licensed under the MIT License ([LICENSE](LICENSE)).
