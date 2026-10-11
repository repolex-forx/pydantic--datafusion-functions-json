# Repolex Knowledge Graph of pydantic/datafusion-functions-json

RDF knowledge graph data for [pydantic/datafusion-functions-json](https://github.com/pydantic/datafusion-functions-json), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download pydantic/datafusion-functions-json
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 30e05810d7b6331a6a72198c3005d72e05b476ad
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 30e05810d7b6331a6a72198c3005d72e05b476ad
│           └── chunk-001.nq.gz
├── blob
│   ├── 01b1120d94dc292eb105c353996b714387c076fa.nq.gz
│   ├── 17be9b06198acf8a9b4418a43dae055af4996887.nq.gz
│   ├── 217042b5784cbb97302f66c747fd675fe2536138.nq.gz
│   ├── 261eeb9e9f8b2b4b0d119366dda99c6fd7d35c64.nq.gz
│   ├── 2ffeba428fe0ba20c4be6887d301b4b74fb859dd.nq.gz
│   ├── 4c7f9bc23144fe09c836703d6e08e7e655cb7058.nq.gz
│   ├── 521e0c6bf65ad96ad353e40251e2e65fe068c7c0.nq.gz
│   ├── 578895797007dfa7f169ce38e37206e02a0a0188.nq.gz
│   ├── 58a364292f847ab6bbcadba1f879a77d298eb223.nq.gz
│   ├── 5907b2b273e0d6d940ea23a5277e1a6427e81766.nq.gz
│   ├── 61e87130befb24c9f7b86ea0679e8d1c3748370f.nq.gz
│   ├── 658f1e31da13c74d3b4ef682bbba21ce0305b3c9.nq.gz
│   ├── 6acc4154bc23d06b839d5a614552216778a78f1c.nq.gz
│   ├── 75306517965a54731b94dca8bace640e856af115.nq.gz
│   ├── 7e051eedc012869be9d7b01e4703318d5cb90809.nq.gz
│   ├── 88c680d67d2d339965b0221d6358e27739969e1b.nq.gz
│   ├── 8bd657d2abadea5caff09fdfd26cb0ca087841ba.nq.gz
│   ├── 8ea040d18758230899e570534627a2de7d3ee6a6.nq.gz
│   ├── 9c0b1e270a30ec17f47093cac26e614cd4a2537c.nq.gz
│   ├── a0e87d59dede15a0e4645135cf0380ca99790ba7.nq.gz
│   ├── af16aa65c64b0aceb9895536e8bd56c16355c041.nq.gz
│   ├── aff252bac853fafa22fefcaecc8b0bec9ccf97b0.nq.gz
│   ├── b471067860b1e02e571903de23e8863b838bc0c9.nq.gz
│   ├── bc4c1b3dabcfdfc3e1cebd2639f83ad5fc1e156e.nq.gz
│   ├── bfb4cb17c504b867a4091b6d9784757c4562b810.nq.gz
│   ├── c340fcd1a658d25cbf1e33ad14d425a96bbb8fce.nq.gz
│   └── f83b71f9b92979926a810e7041e9de8035681796.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 30e05810d7b6331a6a72198c3005d72e05b476ad.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

12 directories, 34 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[pydantic/datafusion-functions-json](https://github.com/pydantic/datafusion-functions-json)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
