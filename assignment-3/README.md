# Assignment 3 — Backend (NestJS) + PostgreSQL (TypeORM)

## Objective
Provide a working NestJS backend and configure a PostgreSQL connection using TypeORM.  
This folder contains an independent, runnable backend project created specifically for Assignment 3.

---

## Tech Stack
- NestJS (TypeScript)
- PostgreSQL
- TypeORM
- Node.js + npm

---

## Folder Contents
- `src/` — application source code (controllers, modules, services)
- `test/` — basic test setup
- `package.json` — scripts and dependencies
- `package-lock.json` — dependency lock file
- `nest-cli.json` — NestJS CLI configuration
- `tsconfig.json`, `tsconfig.build.json` — TypeScript configuration
- `.prettierrc`, `eslint.config.mjs` — code formatting and linting
- `README.md` — this documentation

> Note: `node_modules/` and `dist/` are intentionally excluded from GitHub using `.gitignore`.

---

## Prerequisites (for reviewer)
- Node.js (v18 or higher recommended)
- npm (comes with Node.js)
- PostgreSQL (optional, only required to test DB connectivity)

---

## How to Run the Project (without database)
This verifies that the NestJS application starts correctly.

```bash
cd assignment-3
npm install
npm run start
```

- Server runs on **http://localhost:3000**
- Application should start successfully even if PostgreSQL is not running

---

## Hello World Endpoint Test
```bash
curl http://localhost:3000/hello
```

Expected response:
```json
{ "message": "Hello World" }
```

---

## PostgreSQL Configuration (Optional Test)

### Step 1: Create `.env` file
Create a file named `.env` inside `assignment-3/`:

```
DB_HOST=localhost
DB_PORT=5432
DB_USERNAME=postgres
DB_PASSWORD=postgres
DB_NAME=assignment3_db
```

### Step 2: Start application
```bash
npm run start
```

- If PostgreSQL is running, TypeORM will connect successfully
- If PostgreSQL is not running, a connection error will appear (acceptable for evaluation)

---

## TypeORM Notes
- `autoLoadEntities: true` is enabled
- `synchronize: true` is used for development convenience
- These settings are **not recommended for production**, but are acceptable for internship evaluation

---

## Troubleshooting
- `ECONNREFUSED` → PostgreSQL is not running or credentials are incorrect
- Run `npm install` if dependencies are missing
- Check `src/app.module.ts` for TypeORM configuration

---

## Assignment Status
✅ Independent backend project  
✅ PostgreSQL connection configured  
✅ Clean Git history (no node_modules, no secrets)

This completes **Assignment 3**.
