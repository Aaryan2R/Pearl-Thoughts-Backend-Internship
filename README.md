# Pearl Thoughts – Backend Internship

This repository contains daily backend internship assignments completed for **Pearl Thoughts**. Each assignment is placed in a dedicated folder to make review and execution simple for the company team.

---
## Repository structure (what to expect)
- `assignment-1/` — Assignment 1 Hello World API project (NestJS + TypeScript)
- `assignment-2/` — Assignment 2 ER diagram + Loom explanation
- `assignment-3/` — Assignment 3: full backend project (NestJS + TypeORM + PostgreSQL)

Other root files:
- `.gitignore` — prevents `node_modules/`, `dist/`, and other junk from being committed
- `README.md` — this file (overview & quick reviewer guide)

---
## How a reviewer can access the assignments

### Via GitHub UI (easy)
1. Open: `https://github.com/Aaryan2R/Pearl-Thoughts-Backend-Internship`
2. On the repository page, click the folder you want: `assignment-1`, `assignment-2`, or `assignment-3`.
3. Each folder contains a README with instructions for that assignment.

### Via Git (technical)
```bash
git clone https://github.com/Aaryan2R/Pearl-Thoughts-Backend-Internship.git
cd Pearl-Thoughts-Backend-Internship

# Inspect assignment branches if needed:
git branch -r

# Switch to an assignment branch (if requested by reviewer):
git checkout Assignment-3   # or Assignment-1 / Assignment-2
```

> NOTE: The assignment folders contain the artifacts and READMEs. The working backend code to run (NestJS project) is placed in `assignment-3/` so reviewers can open that folder and run the project directly.

---
## Quick-run (to test Hello endpoint)
1. Open `assignment-3/` folder on GitHub or clone and change directory:
```bash
cd assignment-3
npm install
npm run start
```
2. Test the Hello endpoint (after server starts):
```bash
curl http://localhost:3000/hello
# expected JSON: {"message":"Hello World"}
```

---
If you want I can also commit these README files into the repository for you — follow the `git add`, `git commit`, `git push` commands shown in the local instructions inside each assignment README below.
