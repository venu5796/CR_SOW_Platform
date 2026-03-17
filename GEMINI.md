# CR_SOW_Platform Environment System

This project uses a Git-based environment system to separate Development, Staging, and Production.

## Branches
- **`prod`**: Production code. Deployed to GitHub Pages.
- **`stage`**: Pre-release environment for final validation.
- **`dev`**: Active development environment.

## Workflow
1. **Feature Implementation**: Work is performed on the `dev` branch.
2. **Validation**: Test features locally on `dev`.
3. **Promotion to Stage**: `git merge dev` into `stage`.
4. **Promotion to Production**: `git merge stage` into `prod`.

## Managing Branches (Gemini CLI)
Ask me to:
- "Merge Dev to Stage"
- "Merge Stage to Prod"
- "Sync all branches"
- "Set GitHub remote URL" (e.g., `git remote add origin <url>`)
