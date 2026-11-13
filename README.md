# Atlas downloads

Atlas indexes your SAP Commerce workspace locally and gives coding agents read-only access to the index through MCP.

**Requirements:** macOS, Java 21 or later, and network access to download the release. Docker must be running for indexing and serving the index. The first index may need to download the Neo4j image.

```sh
curl -fsSL https://github.com/guillem-matias/atlas-releases/releases/download/v0.1.0/install-atlas.sh | bash -s -- --version v0.1.0
export PATH="$HOME/.local/bin:$PATH"
atlas --version
```

From your SAP Commerce project root, run `atlas index` to build the index and `atlas install` to register Atlas with Codex and Claude Code.
