# Contributing

Thanks for helping improve this introductory GenAI and LLM workshop.

## Propose a change

1. Open an issue to discuss substantial changes or report a problem. Include the
   notebook section, expected behavior, and actual behavior when relevant.
2. Fork the repository if you do not have write access, and create a topic branch.
3. Keep changes focused and use beginner-friendly explanations.
4. Open a pull request targeting `main`, explaining the change and how you checked it.

## Check your changes

- For notebook changes, restart the kernel and run all cells in order in JupyterLab.
  Check the results and confirm that images still display.
- Keep notebook outputs useful for learners; remove personal information, credentials,
  and machine-specific output before committing.
- For documentation changes, check the instructions, links, and Markdown formatting.
- Never commit API keys, access tokens, `.env` files, or virtual environments.

## Review and branch protection

`@vinays75-coder` owns all files through `.github/CODEOWNERS`.
The active GitHub ruleset for `main` requires pull requests, one approving review,
code-owner approval, and resolution of review conversations. New reviewable commits
dismiss stale approvals. Force pushes and branch deletion are blocked.

Repository administrators may bypass review requirements **through a pull request
only**, which lets the sole maintainer merge their own changes. Direct pushes to
`main` remain blocked. No automated status checks are currently required.

The ruleset configuration is recorded in `.github/rulesets/main-protection.json`.
Editing that file does not update GitHub settings automatically; an administrator
must also update the live ruleset in the repository's **Settings → Rules → Rulesets**.
