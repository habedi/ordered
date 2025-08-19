<div align="center">
  <picture>
    <img alt="Ordered Logo" src="logo.svg" height="20%" width="20%">
  </picture>
<br>

<h2>Ordered</h2>

[![Tests](https://img.shields.io/github/actions/workflow/status/habedi/ordered/tests.yml?label=tests&style=flat&labelColor=282c34&logo=github)](https://github.com/habedi/ordered/actions/workflows/tests.yml)
[![CodeFactor](https://img.shields.io/codefactor/grade/github/habedi/ordered?label=code%20quality&style=flat&labelColor=282c34&logo=codefactor)](https://www.codefactor.io/repository/github/habedi/ordered)
[![Zig Version](https://img.shields.io/badge/Zig-0.14.1-orange?logo=zig&labelColor=282c34)](https://ziglang.org/download/)
[![Docs](https://img.shields.io/github/v/tag/habedi/ordered?label=docs&color=blue&style=flat&labelColor=282c34&logo=read-the-docs)](https://habedi.github.io/ordered/)
[![Examples](https://img.shields.io/github/v/tag/habedi/ordered?label=examples&color=green&style=flat&labelColor=282c34&logo=zig)](https://github.com/habedi/ordered/tree/main/examples)
[![Release](https://img.shields.io/github/release/habedi/ordered.svg?label=release&style=flat&labelColor=282c34&logo=github)](https://github.com/habedi/ordered/releases/latest)
[![License](https://img.shields.io/badge/license-MIT-007ec6?label=license&style=flat&labelColor=282c34&logo=open-source-initiative)](https://github.com/habedi/ordered/blob/main/LICENSE)

A Zig library of common data structures that keep data in order

</div>

---

Ordered Zig library includes implementations of popular data structures including B-tree, skip list, trie, and
red-black tree.

### Features

- Implementations for common data structures that maintain the order of keys:
    - [`BTreeMap`](src/btree_map.zig): A balanced tree map that maintains order of keys.
    - [`OrderedSet`](src/sorted_set.zig): A set with ordered elements.
    - [`SkipList`](src/skip_list.zig): A probabilistic data structure that allows fast search, insertion, and deletion.
    - [`Trie`](src/trie.zig): A prefix tree for fast retrieval of keys with common prefixes.
    - [`RedBlackTree`](src/red_black_tree.zig): A self-balancing binary search tree that maintains order of keys.

| # | Name           | Build Complexity      | Memory Complexity | Search Complexity     | Description                                                                                                                                                              |
|---|----------------|-----------------------|-------------------|-----------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 1 | B-Tree Map     | $O(\log n)$           | $O(n)$            | $O(\log n)$           | A self-balancing tree that is optimized for disk I/O. It maintains sorted data and is efficient for large datasets.                                                      |
| 2 | Cartesian tree | $O(\log n)$ (average) | $O(n)$            | $O(\log n)$ (average) | A binary tree that maintains both a binary search tree property on keys and a heap property on priorities.                                                               |
| 3 | Red-Black tree | $O(\log n)$           | $O(n)$            | $O(\log n)$           | A self-balancing binary search tree. Operations like insertion and deletion take logarithmic time.                                                                       |
| 4 | Skip List      | $O(\log n)$ (average) | $O(n)$            | $O(\log n)$ (average) | A probabilistic data structure that uses multiple layers of sorted linked lists. It is simpler to implement than balanced trees and is often used in concurrent systems. |
| 5 | Sorted Set     | $O(n)$                | $O(n)$            | $O(\log n)$           | A sorted array that provides fast lookups via binary search but slow insertions and deletions because elements need to be shifted.                                       |
| 6 | Trie           | $O(m)$                | $O(n \cdot m)$    | $O(m)$                | A prefix tree used for efficient string-based operations like prefix matching. Here, $m$ is the length of the key.                                                       |

> [!IMPORTANT]
> Ordered is in early development, so bugs and breaking API changes are expected.
> Please use the [issues page](https://github.com/habedi/ordered/issues) to report bugs or request features.

---

### Getting Started

To be added.

---

### Documentation

You can find the API documentation for the latest release of Ordered [here](https://habedi.github.io/ordered/).

Alternatively, you can use the `make docs` command to generate the documentation for the current version of Ordered.
This will generate HTML documentation in the `docs/api` directory, which you can serve locally with `make serve-docs`
and view in a web browser.

### Examples

Check out the [examples](examples/) directory for example usages of Ordered.

---

### Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to make a contribution.

### License

Ordered is licensed under the MIT License (see [LICENSE](LICENSE)).

### Acknowledgements

* The logo is from [SVG Repo](https://www.svgrepo.com/svg/469537/zig-zag-left-right-arrow).
