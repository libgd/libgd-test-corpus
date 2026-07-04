# libgd Test Corpus

Binary conformance and robustness fixtures used by libgd's codec tests.
Test programs and expected-result manifests remain in the main
[`libgd`](https://github.com/libgd/libgd) repository.

## Layout

```text
jpeg/conformance/  JPEG valid, invalid, non-conformant, and crash fixtures
jxl/conformance/   JPEG XL conformance, feature, edge, and invalid fixtures
```

Each codec directory contains its own provenance and licensing documentation.

## Using with libgd

The repository is pinned as the `tests/conformance` submodule in libgd:

```sh
git submodule update --init tests/conformance
```

The corpus is optional for building libgd. It is required only for the full
codec conformance tests.
