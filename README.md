# 🤖 demo-mcp

> A demonstration project for the **Model Context Protocol (MCP)** — a standard that connects AI systems with external tools and data sources.

---

## 📋 Table of Contents

- [About](#about)
- [Features](#features)
- [Getting Started](#getting-started)
- [Project Structure](#project-structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

---

## 🧠 About

**demo-mcp** is a hands-on demo that showcases how to build and connect an MCP server using the [`@modelcontextprotocol/sdk`](https://github.com/modelcontextprotocol/typescript-sdk). It serves as a learning resource for developers who want to understand how AI agents communicate with external services through a standardized protocol.

---

## ✨ Features

- ✅ MCP Server setup with `@modelcontextprotocol/sdk`
- ✅ Custom tool definitions exposed to AI clients
- ✅ TypeScript support
- ✅ Clean project structure ready to extend
- ✅ Easy local development

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18 or higher
- [npm](https://www.npmjs.com/) or [pnpm](https://pnpm.io/)

### Installation

```bash
# Clone the repository
git clone https://github.com/valen-ruggieri/demo-mcp.git
cd demo-mcp

# Install dependencies
npm install
```

### Run the server

```bash
npm run dev
```

---

## 📁 Project Structure

```
demo-mcp/
├── src/
│   ├── index.ts        # Entry point — MCP Server initialization
│   └── tools/          # Custom tool definitions
├── package.json
├── tsconfig.json
└── README.md
```

---

## 🛠️ Usage

Once running, the MCP server exposes tools that can be consumed by any MCP-compatible AI client (e.g., Claude, Antigravity, etc.).

Example tool registration:

```typescript
import { Server } from "@modelcontextprotocol/sdk/server/index.js";

const server = new Server(
  { name: "demo-mcp", version: "1.0.0" },
  { capabilities: { tools: {} } }
);
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

1. Fork the repo
2. Create a feature branch: `git checkout -b feat/my-feature`
3. Commit your changes: `git commit -m 'feat: add my feature'`
4. Push to the branch: `git push origin feat/my-feature`
5. Open a Pull Request against `dev`

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">Made with ❤️ by <a href="https://github.com/valen-ruggieri">Valentin Ruggieri</a></p>
