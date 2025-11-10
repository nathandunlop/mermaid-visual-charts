# Project Setup Instructions

Follow these steps to use this template for a new project.

## 1. Copy This Template

```bash
cd "General Projects"
cp -r _project-template your-new-project-name
cd your-new-project-name
```

**Or manually:**
- Copy the `_project-template` folder
- Rename it to your project name (use kebab-case: `my-project-name`)

## 2. Customize Files

### Update README.md
- Replace `[Project Name]` with your actual project name
- Fill in tech stack details
- Update installation and usage instructions
- Add your features list

### Review .gitignore
- The template includes common ignores for Node.js, Python, databases, etc.
- Add any additional files/folders specific to your tech stack

## 3. Initialize Git

```bash
git init
git add .
git commit -m "Initial commit: [Project Name] setup

Brief description of what this project does.

🤖 Generated with [Claude Code](https://claude.com/claude-code)

Co-Authored-By: Claude <noreply@anthropic.com>"
```

## 4. Verify .gitignore is Working

```bash
git status --ignored
```

Confirm that `node_modules/`, `dist/`, `.env`, etc. appear under "Ignored files".

## 5. Create GitHub Repository

```bash
gh repo create your-project-name \
  --public \
  --source=. \
  --description="Brief description of your project" \
  --remote=origin

git branch -M main
git push -u origin main
```

## 6. Add to General Projects README

Update `General Projects/README.md` to include your new project:

```markdown
### Your Project Name
**Location:** `your-project-name/`
**Type:** [Full-stack web app / CLI tool / API / etc.]
**Tech:** [React, Node.js, PostgreSQL]
**Description:** Brief description
```

## 7. Start Building!

You're all set. Start adding your code and commit regularly.

---

## Quick Checklist

- [ ] Copied template to new folder with kebab-case name
- [ ] Updated README.md with project details
- [ ] Reviewed/customized .gitignore
- [ ] Ran `git init`
- [ ] Made initial commit
- [ ] Created GitHub repo with `gh repo create`
- [ ] Pushed to GitHub
- [ ] Updated General Projects README.md
- [ ] Started coding!

---

**Template Version:** 1.0
**Last Updated:** November 2025
