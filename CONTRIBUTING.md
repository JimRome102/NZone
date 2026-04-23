# Contributing to NZone

This document outlines the workflow for contributing to the NZone project.

## Git Workflow

### Branches

- **main** - Production-ready code and finalized research
- **kindercare-research** - Active research branch for Kindercare partnership
- **feature/*** - Feature branches for specific tasks
- **hotfix/*** - Quick fixes to main

### Creating a Feature Branch

```bash
git checkout main
git pull origin main
git checkout -b kindercare-research
```

Or for specific features:

```bash
git checkout -b feature/collect-contacts
git checkout -b feature/outreach-templates
```

### Making Changes

1. Make your changes on the branch
2. Commit with clear messages:
   ```bash
   git add .
   git commit -m "Add contacts for Boston area locations"
   ```

3. Push your branch:
   ```bash
   git push origin kindercare-research
   ```

### Creating a Pull Request (PR)

1. Go to https://github.com/JimRome102/NZone
2. Click "Pull Requests" → "New Pull Request"
3. Compare `kindercare-research` (or your branch) to `main`
4. Add a title and description:
   - **Title:** Brief summary (e.g., "Add Kindercare Boston region contacts")
   - **Description:** What was added/changed, how many contacts, any notes

5. Click "Create Pull Request"

### Reviewing & Merging

1. Review the changes
2. If ready to merge, click "Merge Pull Request"
3. Delete the branch after merging

### Pulling Latest Changes

Always pull before starting new work:

```bash
git checkout main
git pull origin main
git checkout -b your-branch-name
```

## File Conventions

- **Data files:** `kindercare_contacts.csv`, `kindercare_templates.md`
- **Documentation:** In `docs/` folder or root as `.md`
- **Commits:** Use present tense ("Add contacts" not "Added contacts")

## Research Workflow

1. **Branch:** Create `kindercare-research` branch
2. **Work:** Add contacts, templates, notes
3. **Commit:** Push updates regularly with clear commit messages
4. **PR:** When phase is complete, create PR to main
5. **Merge:** Review and merge to main

## Example Session

```bash
# Start research
git checkout -b kindercare-research
git pull origin main

# Do research work
# ... add contacts to kindercare_contacts.csv ...

# Commit progress
git add kindercare_contacts.csv
git commit -m "Add 50 Boston area Kindercare locations"
git push origin kindercare-research

# More work
# ... add outreach templates ...

git add docs/outreach_templates.md
git commit -m "Add email templates for director outreach"
git push origin kindercare-research

# When phase is done, create PR on GitHub
# Merge to main
```
