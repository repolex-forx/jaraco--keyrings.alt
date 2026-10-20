# Repolex Knowledge Graph of jaraco/keyrings.alt

RDF knowledge graph data for [jaraco/keyrings.alt](https://github.com/jaraco/keyrings.alt), parsed by [repolex](https://repolex.ai).

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
rlex download jaraco/keyrings.alt
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 2189879d8b6c2df8450162194404b47a1b76e2bd
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 2189879d8b6c2df8450162194404b47a1b76e2bd
│           └── chunk-001.nq.gz
├── blob
│   ├── 07e5e9a2c54560252320a62c42159be4283bc11c.nq.gz
│   ├── 0d1f7edf5dc6343538563a8caa7de6829752c4f9.nq.gz
│   ├── 107cc665bff04c49fa416a97a4eb1973c15dc0b5.nq.gz
│   ├── 18c17cf9c362686dcb0d44ab169ba9bfedd0c6f7.nq.gz
│   ├── 19e67ae811db0386b1bc1b42337bd355f1768872.nq.gz
│   ├── 1ab59005b8177ff1a3953714936eb12626f451bd.nq.gz
│   ├── 2e3f4dd791a6372b427d618eb0baa8c4dc58e5f0.nq.gz
│   ├── 304196f81e11a168c9894f966e4a617ebf4ed53c.nq.gz
│   ├── 349523efe59a085d933263fdca013c0726363111.nq.gz
│   ├── 37082e4b113c6139900c8f447b365d40b19d730c.nq.gz
│   ├── 39c66a83ea853cbc91770d394ab0144d9f93a577.nq.gz
│   ├── 3cf978b3c17c7c28cd7a8ace353db254b0ff6bef.nq.gz
│   ├── 42136fcb7470b38a511a34ef766a94d6a677ab6b.nq.gz
│   ├── 452efae8d76d33b50da971e777e297f2ce835a6b.nq.gz
│   ├── 54c9000ec94341dd65c2053251b85b124017b9b5.nq.gz
│   ├── 54cc8303b22089e12053e552d4e6cb852a865b8a.nq.gz
│   ├── 54f99acbfac68c2be8283174ea64f1730a795e49.nq.gz
│   ├── 577e87a793a20e413f7321f4f17ec1eba2ea1962.nq.gz
│   ├── 5bdc232005af9be104a00437ae9bc64417a4c1cc.nq.gz
│   ├── 5c05f9e27d57a4b7a3c3a9fdfecf8cddb8be499f.nq.gz
│   ├── 5f0b87446c672c54fb4c2342fc57685f7cdd26e4.nq.gz
│   ├── 6188b60658753d7567837a9345b25f17e9ee1a8e.nq.gz
│   ├── 6d02c7e00b81b7079b96a6c64591af9471160a7a.nq.gz
│   ├── 700235be57c1b2872455c0be5333f59cf568e252.nq.gz
│   ├── 724370638fc188317bbc7dc868f1a571995fd796.nq.gz
│   ├── 72ca2410e2e05a744fe98768b7a485d164006561.nq.gz
│   ├── 75d53bc901137a7a2b64fcc0ab2911e411b68245.nq.gz
│   ├── 7af63bfa56fb5e5410139c3657e42af89f2cc0b2.nq.gz
│   ├── 9a0f3bce1395ae3819030b822e5d9076c85068ea.nq.gz
│   ├── b3da1e1b803d066a8e97aea4760e58a51b471a31.nq.gz
│   ├── b98ee451c6d8e2082c7338262da167711d82dd32.nq.gz
│   ├── baeeaf7c398475c435c856b176a287cc0baa6d12.nq.gz
│   ├── c08a0385cd850258ba103c675ebfb0c705b4c107.nq.gz
│   ├── c54bbdcf8e54daf1223e6c2c277032ee7a47a2f3.nq.gz
│   ├── e05a3d4a2ab888e32952006d8cd380864368db5f.nq.gz
│   ├── e2e29c9db43fe09edc5ff3692f4b331d14f9de4f.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── f89fb3545369981d9f6c9e2a5816e2bebbaac778.nq.gz
│   ├── fa017c68ac0aa323f5d691bf971daf9be010d220.nq.gz
│   └── fa66a689231f157518fde5e0ebeeffcec17339b0.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 2189879d8b6c2df8450162194404b47a1b76e2bd.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 48 files
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

[jaraco/keyrings.alt](https://github.com/jaraco/keyrings.alt)

---
*Parsed on 2026-10-20 by [repolex](https://repolex.ai)*
