# Technical Automation Plan for Git Workflows

## [x] 1. Commit Message Formatting (done)
- Enforce or auto-generate commit messages using git hooks (already set up).

## [ ] 2. Pre-commit Checks (high priority)
- Run linters, formatters, or tests before allowing a commit (pre-commit hook or Husky).

## [x] 3. Pre-push Checks (high priority)
- Run tests or checks before pushing to remote to prevent broken code from being pushed. (pre-push hook set up)

## [x] 4. CI/CD Integration (high priority)
- Trigger builds, tests, or deployments automatically on push or PR via GitHub Actions (ci.yml set up)

## [x] 5. Automatic Pull Request Creation (medium priority)
- Use CLI tools or GitHub Actions to open PRs automatically after a push. (auto-pr.yml set up)

## [x] 6. Branch Naming Conventions (medium priority)
- Enforce branch naming rules with hooks. (pre-commit hook set up)

## [x] 7. Issue/PR Templates (medium priority)
- Standardize new issues and PRs with templates. (templates set up)

## [x] 8. Changelog Generation (low priority)
- Automatically generate or update a changelog from commit history. (changelog.yml set up)

## [ ] 9. Dependency Updates (low priority)
- Use bots (like Dependabot) to automa te dependency update PRs.

---

Check off items as you complete them!

---

## AI Doc Suggestions
- Currently using a public OpenAI-powered GitHub Action for doc suggestions on PRs.
- Option: Switch to a custom script with your own OpenAI API key for more control in the future.

---

## Documentation Automation (future options)
- [ ] Auto-generate API docs from code/comments (e.g., Swagger, Sphinx, JSDoc)
- [ ] Auto-lint and format docs (markdownlint, prettier) on PRs and pushes
- [ ] Auto-publish docs to GitHub Pages or static site on merge
- [ ] Doc coverage reports (measure % of codebase documented)
- [ ] Template-driven doc creation for new features/modules
- [ ] Auto-link code and docs (bot checks for code changes not reflected in docs)
