# typescript-productivity-setup

Configuration files to boost your productivity with TypeScript.

---

## 🚀 Node.js Installation

If you're using **Linux**, install Node.js using `nvm`:

```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.40.2/install.sh | bash
\. "$HOME/.nvm/nvm.sh"
nvm install 22
node -v
nvm current
npm -v
```

Or download it manually from:  
🔗 https://nodejs.org/en/download

---

## 📦 Optional: Install Yarn

This setup uses **Yarn** (optional).  
To install globally:

```bash
npm install --global yarn
```

> Prefer **npm**? No problem — all commands work with either.

---

## 📁 Example Folder Structure

```
project-root/
│
├── src/                # Source code
│   ├── routes/         # Route handlers
│   ├── controllers/    # Business logic
│   ├── schemas/        # Zod validation schemas
│   ├── utils/          # Utility functions
│   └── server.ts       # Application entry point
│
├── tests/              # Vitest test files
│
├── tsconfig.json       # TypeScript configuration
├── package.json
└── README.md
```

---

## ⚙️ Initialize TypeScript

After installing dependencies, run:

```bash
npx tsc --init
```

Then update `tsconfig.json` with recommended options:

```json
{
  "compilerOptions": {
    "target": "ES2022",
    "module": "ESNext",
    "moduleResolution": "Node",
    "esModuleInterop": true,
    "strict": true,
    "skipLibCheck": true,
    "forceConsistentCasingInFileNames": true,
    "outDir": "./dist"
  },
  "include": ["src"],
  "exclude": ["node_modules", "dist"]
}
```

---

## 📥 Install Dependencies

### Development

```bash
yarn add -D typescript tsx tsup vitest
```

### Production

```bash
yarn add fastify zod
```

---

All set! You now have a lightweight, organized, and productivity-ready TypeScript setup. 🚀
