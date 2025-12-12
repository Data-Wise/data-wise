# Finding Projects Permission in Fine-Grained Token

## Where to Look

Fine-grained tokens have **3 permission sections**. Projects can be in different places depending on your setup:

### 1. Repository Permissions (Common)

Scroll down to **"Repository permissions"** section and look for:

- **Projects** (for repository-level project boards)

### 2. Account Permissions (For User Projects)

Scroll further to **"Account permissions"** and look for:

- **Projects** (for your personal project boards)

### 3. Organization Permissions (If Data-Wise is an Org)

If you see **"Organization permissions"**, check:

- **Projects** (for organization-level boards)

---

## Screenshot Guide

When editing your token, you should see sections like this:

```
Repository permissions
├── Actions (Read-only / Read and write / Admin)
├── Contents (Read-only / Read and write)
├── Metadata (Read-only) [MANDATORY]
├── Projects ← LOOK HERE FIRST
└── ...

Account permissions
├── Followers (Read-only / Read and write)
├── Projects ← OR HERE
└── ...
```

---

## Can't Find It At All?

If "Projects" doesn't appear anywhere, it might mean:

**Option A**: The token type doesn't support it

- Try: Create a new token instead of editing
- Go to: Settings → Developer settings → Personal access tokens → Fine-grained tokens → "Generate new token"
- When creating, you'll see all available permissions

**Option B**: Your account doesn't have projects enabled

- Check if you actually have projects at: <https://github.com/Data-Wise?tab=projects>
- Or your user projects at: <https://github.com/users/DATA-WISE-USERNAME/projects>

---

## Alternative: Try This Command

Instead of editing the token, try refreshing your gh CLI auth:

```bash
gh auth refresh -h github.com -s project
```

This might prompt you to re-authorize with project scope.

---

## What's Your Project URL?

Can you share the URL of your GitHub Projects board? It will look like:

- `https://github.com/users/USERNAME/projects/1` (user project)
- `https://github.com/orgs/Data-Wise/projects/1` (org project)

This will help me understand which permission type you need!
