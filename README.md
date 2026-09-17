# ⚛️ GAMA Engine — Standalone Distribution & MCP Server

Official standalone binary & distribution channel for **GAMA Multi-Dimensional Hyper-Physics Engine v2.0.0** (2D/3D/4D/5D Kinematics, WebGPU Compute, Relativistic Geodesics, Zero-GC Invariants, and Master Model Context Protocol Server).

---

## 📦 Downloads (v1.0.0 Release)

| Asset | Platform | Description |
| :--- | :--- | :--- |
| **[`gama-v1.0.0-dist.zip`](https://github.com/ahmadshady747-create/gama-binaries/releases/download/v1.0.0/gama-v1.0.0-dist.zip)** | Universal (Node.js 20+) | Self-contained bundled MCP server executable, Windows runner (`.cmd`), and Unix runner (`.sh`) |
| **[`SHA256SUMS.txt`](https://github.com/ahmadshady747-create/gama-binaries/releases/download/v1.0.0/SHA256SUMS.txt)** | All | Cryptographic SHA-256 integrity checksums |

### Cryptographic Verification
```bash
sha256sum -c SHA256SUMS.txt
```

---

## 🔌 Model Context Protocol (MCP) Setup Guide

Configure GAMA Engine in your MCP host clients (Claude Desktop, Cursor, Antigravity, Windsurf, Cline) using standard `stdio` transport:

### Claude Desktop Configuration (`claude_desktop_config.json`)
```json
{
  "mcpServers": {
    "gama": {
      "command": "node",
      "args": [
        "C:/path/to/gama-binaries/gama-mcp.cjs"
      ],
      "env": {
        "NODE_ENV": "production"
      }
    }
  }
}
```

*(Or run via the packaged batch script `gama-mcp.cmd` on Windows / `gama-mcp.sh` on macOS/Linux).*

---

## 🛡️ License & Guarantees
- Licensed under **Business Source License 1.1 (BSL 1.1)** with explicit As-Is / Self-Service disclaimer. See [`LICENSE`](LICENSE) for complete terms.
- Strictly verified and governed by the **LOCUS Deterministic Safety & AST Invariant Protocol** (Zero-NaN, Zero-GC in active physics tick loops).
