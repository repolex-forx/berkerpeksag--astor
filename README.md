# Repolex Knowledge Graph of berkerpeksag/astor

RDF knowledge graph data for [berkerpeksag/astor](https://github.com/berkerpeksag/astor), parsed by [repolex](https://repolex.ai).

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
lexq download berkerpeksag/astor
```

This will automatically download essential data files from the last parsed commit. Consult `lexq --moreinfo` for other options, including downloading multiple commits, blobs, etc.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c7553c79f9222e20783fe9bd8a553f932e918072
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── c7553c79f9222e20783fe9bd8a553f932e918072.nq.gz
│   └── repolex
│       └── c7553c79f9222e20783fe9bd8a553f932e918072
│           └── chunk-001.nq.gz
├── blob
│   ├── 0c5ddcdb1da2ea6a901884b478720797956f8e75.nq.gz
│   ├── 19463fb7f65afcd737f9184c5c4c3bbeb4b15c51.nq.gz
│   ├── 2f716ad837015cff29acee15b479ad3b9c963d4c.nq.gz
│   ├── 359242b1edac72b5159ecad57aab94f5e78054af.nq.gz
│   ├── 398552383f7fed2f7d031f77505fb5682fea5df2.nq.gz
│   ├── 3d85b79abb6b461758658083f6e62d4d936738f8.nq.gz
│   ├── 43e62286d2e198a06bba81ef09e3bad80bb0d843.nq.gz
│   ├── 45df8c05f987b38df2ed5bf3f5606da980b74a76.nq.gz
│   ├── 606849326a4002007fd42060b51e69a19c18675c.nq.gz
│   ├── 65c590c575cbb254fb2a9e6cfec86fc974a52c27.nq.gz
│   ├── 662b9f2731c0ce4535526b06e0b4e39d97ed2c3a.nq.gz
│   ├── 6dce9ccd202ab583718772dbfcfba395ef9b9577.nq.gz
│   ├── 6f4eebdf6f68fc72411793cdb19e3f1715b117f3.nq.gz
│   ├── 7ce55d9314a6c9b060163bee336257ed1779e3e2.nq.gz
│   ├── 81e72d5db67b1abefd9d476ff9edb12b420e3bdf.nq.gz
│   ├── 894fa6dc1ab492f4831f3f1c5554b86484962d45.nq.gz
│   ├── 8b108e72a981c911f4a296003a1b15790682a7ed.nq.gz
│   ├── 8f4e8166e555017501deba62822080a0da87e330.nq.gz
│   ├── a04940c7300f852ff86c818ce19910c059f94e7f.nq.gz
│   ├── af08977c11a663b553b54a0f4c092d9be34a73f0.nq.gz
│   ├── bdedaeffd7cc30a2938f7688cd8efc33f2fc744b.nq.gz
│   ├── c0391b9a58771a01259af37cce7af2ecf99f2612.nq.gz
│   ├── c5ff51d6be84c5fa32ad5a00198d3ed9b21c327d.nq.gz
│   ├── c61f980b4bb7e0b6f41440c4411d083fb85c2e50.nq.gz
│   ├── c80a6601f95a5c88a875a4c8e34cd516a851fcc8.nq.gz
│   ├── c8dc4eeb07696ea9dff123b1aed571a77826d5c4.nq.gz
│   ├── d685597e8f47b4ab77c94f2cbf77f2593b596124.nq.gz
│   ├── da71759208405943c41c8e7add3c53cba4217a27.nq.gz
│   ├── db8c4eabcc67e0bff76bc2e312dad37590a1d4d1.nq.gz
│   ├── df658a86e876931b8fc7842b1bd4352bf5cd020c.nq.gz
│   ├── e0048072e5e8e220ccdd13b01820a0586b67bd64.nq.gz
│   ├── e3c940f0f61f75255ddd31cc57907a1922aab97a.nq.gz
│   ├── e54e88b6884d14a4f0a7c9b7f8088901b55afd40.nq.gz
│   ├── e69de29bb2d1d6434b8b29ae775ad8c2e48c5391.nq.gz
│   ├── ec52114c9811fdf251548575ecf78dc736a29177.nq.gz
│   ├── f4d06d5b23c3d71f490ec82884570426ae21f8d0.nq.gz
│   ├── fc26bc48c5b2a1e1f92f11c7b8857b037bb06740.nq.gz
│   └── fd715381c94330321d94a87db319ca448d36ceb3.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── c7553c79f9222e20783fe9bd8a553f932e918072.nq.gz
├── filetree
│   └── c7553c79f9222e20783fe9bd8a553f932e918072.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

15 directories, 48 files
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

[berkerpeksag/astor](https://github.com/berkerpeksag/astor)

---
*Parsed on 2026-04-13 by [repolex](https://repolex.ai)*
