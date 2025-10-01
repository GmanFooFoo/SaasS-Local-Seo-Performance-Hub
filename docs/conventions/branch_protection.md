# Branch Protection Guidelines

## Why Protect the Main Branch?
Protecting the `main` branch ensures your production code is always stable, prevents accidental loss of work, and enforces code quality through automated checks and reviews.

## Recommended Settings
- **Protect against force pushes and deletion**
  - Prevents accidental or malicious overwrites or branch removal.
- **Require status checks to pass before merging**
  - Only allow merging PRs if CI, lint, and other checks pass.
- **Require pull request reviews before merging** (optional, but recommended)
  - Ensures at least one other person reviews changes before they are merged.
- **Require branches to be up to date before merging**
  - Prevents merging stale code.
- **Include administrators** (optional)
  - Ensures even admins follow the same rules for extra safety.

## How to Set Up on GitHub
1. Go to your repository on GitHub.
2. Click on `Settings` > `Branches`.
3. Under `Branch protection rules`, click `Add rule`.
4. Set the branch name pattern to `main`.
5. Select the recommended settings above.
6. Click `Create` or `Save changes`.

## Additional Notes
- You can further restrict who can push to the branch if needed.
- Adjust rules as your team or workflow evolves.

---

For more details, see the [GitHub Docs on Branch Protection](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-a-branch-protection-rule).
