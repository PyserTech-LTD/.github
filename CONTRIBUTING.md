# Contributing Guide

## Flow

```
/<short-name>  →  dev  →  main
```

PRs always target `dev`. Only `dev` merges into `main`.

---

## 1. Create an Issue

- Open a task from the GitHub Project board — this creates the issue automatically.
- Assign it to self.

---

## 2. Create a Branch

Always pull latest `dev` first:

```bash
git checkout dev
git pull origin dev
git checkout -b /seeworld-gateway
```

Branch naming:

```
/seeworld-gateway
/sensor-analytics
/gps-null-crash
/auth-token-expired
/update-dependencies
/location-service
```

---

## 3. Commit

```
feat: add seeworld gateway layer
fix: resolve gps null crash
chore: update dependencies
refactor: extract location service
hotfix: fix auth token expiry
```

---

## 4. Open a Pull Request

- Target branch: `dev`
- Title: same format as commit message
- Description must include desribe task `xxxx ingtegration completed.`
- Fill in the PR template completely

---

## 5. Merge to Main

Only `dev` → `main`, after testing is complete.  
Never merge a feature branch directly to `main`.
