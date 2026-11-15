# Together document formats

Definitions and test vectors of the document formats that Together-Pad writes, for anyone who wants to read
and write them in a program of their own. Each format is a document profile (or a layer) of
[TDSP](https://github.com/wappensc/tdsp), the Together Document Sync Protocol, and its name lies in the
namespace `de.wappensc.together.format.*`.

| Format | Definition | Test vectors | Status |
|---|---|---|---|
| `de.wappensc.together.format.richtext/1` | [richtext-1/index.html](richtext-1/index.html), published at <https://together-pad.com/formats/richtext-1/> | [richtext-1/vectors.json](richtext-1/vectors.json) | final (15 November 2026) |

The published page is the definition that holds. This repository keeps the same text and the vectors that go
with it, so that every tag shows which text belongs to which vectors.

## Using the vectors

Each vector lists Yjs updates and what they must yield: the state, its projection to plain text, the state
vector, the canonical encoding of what was deleted and what a reader shows. The fields are described at the top
of `vectors.json` and in section 11 of the definition.

## Terms

Anyone may implement these formats, without asking and without fee. Text and test vectors are under the
[MIT licence](LICENSE).

## Changes

A format changes only through its definition: only the definition adds keys, values, formats or embed types,
and once a version is final it changes only compatibly; an incompatible change gets a new name with a new major
version. Questions, unclear passages and mistakes are welcome as issues. A pull request is read as a suggestion;
an accepted change comes into the definition by its maintainer.

Maintained by WappenSC, the maker of Together-Pad.
