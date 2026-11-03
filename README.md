# Virtool Archive

This repository keeps the source code of retired Virtool repositories. Each
retired repository is one branch. The branches share no history with each
other.

This `main` branch has only this README. It has no code.

## Branches

| Branch | Source repository | Contents | Last commit |
| --- | --- | --- | --- |
| `python` | Python-era application | The Python-era Virtool application and retired workflow repositories. | |
| `ui` | `virtool/virtool-ui` | The browser frontend for Virtool. | 2026-08-18 |
| `create-sample` | `virtool/workflow-create-sample` | Workflow that creates Virtool samples. | 2026-08-17 |
| `create-subtraction` | `virtool/workflow-create-subtraction` | Workflow that creates Virtool subtractions. | 2026-08-12 |
| `nuvs` | `virtool/workflow-nuvs` | Workflow that identifies novel viruses. | 2026-08-17 |
| `pathoscope` | `virtool/workflow-pathoscope` | Workflow that detects known OTUs (viruses) by mapping reads to a reference. | 2026-08-17 |

## Tags

Each branch keeps the release tags of its source repository. The tag names
have the branch name as a prefix. This prevents conflicts, because tags share
one namespace in a repository.

| Source tag | Tag here |
| --- | --- |
| `7.84.0` (`virtool-ui`) | `ui/7.84.0` |
| `5.15.0` (`workflow-nuvs`) | `nuvs/5.15.0` |

## Use a branch

```bash
git clone --branch ui --single-branch https://github.com/virtool/archive.git
```

To list the tags of one branch:

```bash
git ls-remote --tags https://github.com/virtool/archive.git 'ui/*'
```
