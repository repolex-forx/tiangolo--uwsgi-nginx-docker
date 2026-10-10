# Repolex Knowledge Graph of tiangolo/uwsgi-nginx-docker

RDF knowledge graph data for [tiangolo/uwsgi-nginx-docker](https://github.com/tiangolo/uwsgi-nginx-docker), parsed by [repolex](https://repolex.ai).

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
rlex download tiangolo/uwsgi-nginx-docker
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 2a3330ace1a83460a613dcfc3977055db888c9a2
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 2a3330ace1a83460a613dcfc3977055db888c9a2
│           └── chunk-001.nq.gz
├── blob
│   ├── 093e1c772ce0ed36bd8bb1d70bd925669af8d260.nq.gz
│   ├── 09f30fd4055ca41cfa9f957252ebc91abc1029e0.nq.gz
│   ├── 15c1060ec4f9e9829bb2862899949d02e75c1dbb.nq.gz
│   ├── 2811ded3331f0482bdee78628f167c7668741729.nq.gz
│   ├── 3af2b8b09377fa7b53d376720610e48ce313b82f.nq.gz
│   ├── 3bb5bfdcc1e30df338692b944c957ba4c9787611.nq.gz
│   ├── 3e3b88c56edb26592a7086b6d1bf2baab9badf94.nq.gz
│   ├── 45d475b319432180076c3b3532657938210305bd.nq.gz
│   ├── 4df28b51950d44648b735e50393f363c57d18ee6.nq.gz
│   ├── 4eab71bc50ec3946260fc2e069de89fa699666aa.nq.gz
│   ├── 55eec6eb458d17b0a36c90625488d8fafbda90d5.nq.gz
│   ├── 59d4301351e60226bb364e1d26183f78bb89bceb.nq.gz
│   ├── 5fc5f542be61a8ec27f104a4685be273a6350ebd.nq.gz
│   ├── 60718f4ca1d979daa03c02d618a5f7a0f250658a.nq.gz
│   ├── 71f71770c6f3d2979972ddef3cc27713ff8fa32f.nq.gz
│   ├── 72d7a762c502b410a9956dc0f3704e22248fd107.nq.gz
│   ├── 8033a67d198b43609fe5050f1d708e95cc81efa4.nq.gz
│   ├── 895bb4cc0862ee8415e083f1240143e9ddb532f0.nq.gz
│   ├── 8a29f73509400236f2bbafc976d5dacaa7dc5093.nq.gz
│   ├── 8f8932f1ac6fcf5729d306ea98b703528224dd69.nq.gz
│   ├── 91365b9dd992ef250c21dd02859315bd31e58c8e.nq.gz
│   ├── 94143827ed065ca0d7d5be1b765d255c5c32cd9a.nq.gz
│   ├── 9ccb1dabcbaf7082ebc12fdefdb7c061d05983e2.nq.gz
│   ├── a037103acad10187ca7d93e0d96996e500180856.nq.gz
│   ├── a666aaab13f6ad3e792f00ffdb7d73e17c7aa79d.nq.gz
│   ├── c87207974b7506aab88361fde06eed9fef5f0c7c.nq.gz
│   ├── c94d562277a586c63f96f5e08e85cef15d9b1a4f.nq.gz
│   ├── cb4a893e0f31e79bff652190b8ef52e85737b5eb.nq.gz
│   ├── cba4c0f687cbd1ff851cb5c888adf4e4092cf7cd.nq.gz
│   ├── cbe8b6e03be1e1168901d8bef53bf024b07539bd.nq.gz
│   ├── d092edbd34c6c9da84aa3ee3c733d430a54d3b8a.nq.gz
│   ├── d1002512712a0d54d3e7c7d501b3c85bae052949.nq.gz
│   ├── d151b3511f957e365b6aaf634f28abdfd59c5d9e.nq.gz
│   ├── da82b3c0b63d55cf25b1b80a7e6813ec42ce023a.nq.gz
│   ├── e311a789f21ccc0908071596f3ffae60ecc2b7c6.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ea050d7be5487f2e86d9f01006c172500d787312.nq.gz
│   ├── f4bac1a1c1885eb6b303f59e963c8d5bf7878e92.nq.gz
│   ├── fd7eb9d7f4e76dcf832907bd3282cbbdfe8f95f1.nq.gz
│   └── ffb4e568394dc94a17f7851dbc7f8ca0d252b40c.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 2a3330ace1a83460a613dcfc3977055db888c9a2.nq.gz
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

[tiangolo/uwsgi-nginx-docker](https://github.com/tiangolo/uwsgi-nginx-docker)

---
*Parsed on 2026-10-10 by [repolex](https://repolex.ai)*
