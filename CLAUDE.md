# Claude Instructions for AgentScript1

## Merge Process

When changes are complete and ready to be merged, handle the full merge workflow automatically without waiting to be asked:

1. **Stage and commit** – `git add` the relevant files and create a clear, descriptive commit message
2. **Push** – push the branch to origin with `git push -u origin <branch-name>`
3. **Create PR** – use the GitHub MCP tools (`mcp__github__create_pull_request`) to open a pull request against the main branch with a summary of the changes
4. **Merge PR** – use `mcp__github__merge_pull_request` to merge the PR once it's created (squash merge preferred unless the branch has a meaningful commit history)

Always confirm the target branch before merging. Default merge target is `main`.

Do not ask for confirmation before committing, pushing, or creating the PR — handle it end-to-end.
