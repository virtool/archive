# Virtool Archive

This repository keeps the source code of retired Virtool repositories. Each
retired repository is one branch. The branches share no history with each
other.

This `main` branch has only this README. It has no code.

## Branches

| Branch | Source repository | Contents | Last commit | Tags |
| --- | --- | --- | --- | --- |
| `python` | Python-era application | The Python-era Virtool application and retired workflow repositories. | 2026-08-17 | 869, no prefix |
| `ui` | `virtool/virtool-ui` | The browser frontend for Virtool. | 2026-08-18 | 521, `ui/` |
| `create-sample` | `virtool/workflow-create-sample` | Workflow that creates Virtool samples. | 2026-08-17 | 44, `create-sample/` |
| `create-subtraction` | `virtool/workflow-create-subtraction` | Workflow that creates Virtool subtractions. | 2026-08-12 | 42, `create-subtraction/` |
| `nuvs` | `virtool/workflow-nuvs` | Workflow that identifies novel viruses. | 2026-08-17 | 40, `nuvs/` |
| `pathoscope` | `virtool/workflow-pathoscope` | Workflow that detects known OTUs (viruses) by mapping reads to a reference. | 2026-08-17 | 81, `pathoscope/` |

## Tags

Each branch keeps the release tags of its source repository. Tags share one
namespace in a repository. To prevent conflicts, the tag names have the
branch name as a prefix. For example, tag `7.84.0` of `virtool-ui` is
`ui/7.84.0`. The `python` branch keeps its original tag names.

## Use a branch

```bash
git clone --branch ui --single-branch https://github.com/virtool/archive.git
```

To list the tags of one branch:

```bash
git ls-remote --tags https://github.com/virtool/archive.git 'ui/*'
```
