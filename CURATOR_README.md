# Mudit Dholakia's curated copilot learning fork

Source: [microsoft/agent-academy](https://github.com/microsoft/agent-academy). This is an upstream fork, not original authorship.
Purpose: Structured Copilot Studio lessons with progressive exercises.
License: upstream MIT. Preserve LICENSE, copyright notices, and any asset-specific terms.
Snapshot before curator additions: `c219c2591c9f3c6e40d7af2b2b5e2bca89da7bbd`.

## Start here

Recommended starting point: **Recruit beginner course**.
Prerequisites: Copilot Studio trial/license and development environment.
Read the upstream README and selected sample's instructions before installing dependencies.
Never use real customer data or commit tenant configuration. Cloud setup and live execution
have not been performed by this curation process.

## Local checkout

This is a shallow, blob-filtered sparse checkout to limit downloads. Included directories:
`["docs/recruit"]` plus `.github` and root files. Excluded files remain
available in the complete GitHub fork. To include another learning directory:

```sh
git sparse-checkout add <PATH>
```

To materialize everything, run `git sparse-checkout disable`; large courses can download
substantial assets. Sparse checkout does not remove upstream history or content on GitHub.

## Your learning plan

1. Explain the selected example's inputs, agent instructions, tools, identity, and output.
2. Create a dedicated development environment with synthetic inputs and least privilege.
3. Record the exact SDK/runtime version, prerequisites, and setup evidence.
4. Run one happy-path prompt and negative tests for grounding, permissions, and injection.
5. Document a failure and a mitigation. Do not equate a successful demo with production readiness.
6. Implement your own variation in the original portfolio lab; cite this source if adapted.

## Upstream updates

```sh
git fetch --unshallow upstream  # once, only while shallow
git fetch upstream
git switch main
git merge upstream/main
git push origin main
```

Review licensing, dependencies, API migrations, and conflicts before executing upstream
code. Curator files and the README banner are additive; upstream notices are retained.
See CURATOR_SECURITY.md for audit results and adoption boundaries.

## Troubleshooting

Missing files: add the relevant sparse path. Merge history errors: unshallow first.
Authentication errors: check `gh auth status`. Cloud authorization errors: check the
specific sample's identity, consent, and licensing requirements rather than elevating
permissions broadly. Do not enable upstream Actions until reviewing each workflow.
