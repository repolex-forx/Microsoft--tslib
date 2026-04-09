# Repolex Knowledge Graph of Microsoft/tslib

RDF knowledge graph data for [Microsoft/tslib](https://github.com/Microsoft/tslib), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [lexq](https://github.com/repolex-ai/lexq) query tool using [uv](https://docs.astral.sh/uv/getting-started/installation/).

If you have uv installed, just copy/paste this into your terminal:

```bash
uv tool install git+https://github.com/repolex-ai/lexq
```

This installs lexq onto your system, in your user context. Verify the install:

```bash
lexq --help
```

**lexq is designed to be used primarily by LLMs in a terminal.** Start up your favorite LLM and ask it to use the lexq tool. It's that easy!

To load this repo's data:

```bash
lexq download Microsoft/tslib
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── ca5f7fb791f85ebf17c0102cdc632e9577b3e483
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── ca5f7fb791f85ebf17c0102cdc632e9577b3e483.nq.gz
│   └── repolex
│       └── ca5f7fb791f85ebf17c0102cdc632e9577b3e483
│           └── chunk-001.nq.gz
├── blob
│   ├── 00d2841124378dd659fc38064763f1e88037976f.nq.gz
│   ├── 04c09f4dbeb60aef902d0dc0814615353f7d5666.nq.gz
│   ├── 0769d234b3fd58c994c476abbdef8bdb57d1bd40.nq.gz
│   ├── 0e42542369729ec05635e54491d177e86ccea100.nq.gz
│   ├── 0f56d34c47fb55b65d7170d999d5de764e56f0ce.nq.gz
│   ├── 136ad0088c30380776636ccdedc162b1e2b1aced.nq.gz
│   ├── 23992f6df8b85528158fbf3d533ab57fde58ca5c.nq.gz
│   ├── 290cc618fba09dc5e93cb6c6b2364835d474f205.nq.gz
│   ├── 2fdb77accff9af2476a51b99e5f4d33972861c0f.nq.gz
│   ├── 3244fabeec060d55c47f0a981adb9d629fd0678f.nq.gz
│   ├── 3609e6b06801c3ec6340f28272e6a8b7ac69f8d6.nq.gz
│   ├── 3ac4a8f915c12ec98f27abb1e1029d517f1b2aef.nq.gz
│   ├── 43c97e719a5a824700932f72e6e7e6748ce45d01.nq.gz
│   ├── 47956e1e0f62fde578a7967235ea49b6a7ed36a8.nq.gz
│   ├── 4875eede59c4ba8bccefb6077a070fa849d90a2c.nq.gz
│   ├── 66f4b38590620f97a7a308cee895760e906f37ab.nq.gz
│   ├── 6eb83d59ee461e8be6c9ed25f4f6d60ceb52d553.nq.gz
│   ├── 731dab48315d4d3eab7f6622a833f87fff96ce28.nq.gz
│   ├── 74f5f4a6409487aa0154c278e7c1ec6c6e72fd57.nq.gz
│   ├── 7a9215a9e7b6ab772fdfd05ce41c315012df82c1.nq.gz
│   ├── 7b3f22814032904946929891071de3b7f70e558e.nq.gz
│   ├── 7ce57f9af6ba9f1153bffd02149fc97018b08e80.nq.gz
│   ├── 8697e6ef638dbba68091177d2ccb262400f1d049.nq.gz
│   ├── 869fdfe2b246991a053fab9cfec1bed3ab532ab1.nq.gz
│   ├── 95beb9179490936cf692dbd15e750dd243204375.nq.gz
│   ├── a14735260705edafbe329f78d48c10262103c6ee.nq.gz
│   ├── a1d9ef56b262b392240b63768db084bdc620d037.nq.gz
│   ├── a26e3e508ecee987effd53d76fb0a07e44072c01.nq.gz
│   ├── a2ce16102e4a64de5f0d0f8c883b8c5d587cf994.nq.gz
│   ├── aafa0e4b45ab8f65ed28c0d0b389ae9587aa3d80.nq.gz
│   ├── aafc1dc61d5795fc626eed67f23ce1b0751fa27f.nq.gz
│   ├── ab4829e440219f6992526b203fc1e218c927d718.nq.gz
│   ├── bca51b352e768f4c537189c215af810d65135580.nq.gz
│   ├── bfe6430cb0d83f34f5ed859d118dd3dc8ec1f7e8.nq.gz
│   ├── c91f61864fead99b3085eed82ae0aa8a098d83a8.nq.gz
│   ├── d892fe0759407813320869b4572b1422bc2b3583.nq.gz
│   ├── ddd87f6bd630263a2879a3bb87837af04aa05926.nq.gz
│   ├── f23df5596e4c82c702ef1fcf8f8be68d650e3988.nq.gz
│   ├── f25ede676f3e4ff8639d209c5d71d5ee50626a83.nq.gz
│   └── f6a69d5fda62ea7894654b34d644a85ecd533dee.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── ca5f7fb791f85ebf17c0102cdc632e9577b3e483.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 49 files
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

## Source repository

[Microsoft/tslib](https://github.com/Microsoft/tslib)

---
*Parsed on 2026-04-09 by [repolex](https://repolex.ai)*
