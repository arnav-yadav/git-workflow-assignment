# Git Workflow Assignment

This local project contains two HTML pages and demonstrates the assignment's
initial commit, second commit, feature branch, explicit merge, ignore rules,
additional commit, and history-preserving revert.

## Files

- `index.html`, `about.html`: the two-page project.
- `.gitignore`: ignores `*.log` files and `temp/` folders.
- `git_commands.txt`: commands with explanations; prepared GitHub commands are marked pending.
- `evidence/git_workflow.txt`: actual command output for the workflow and undo demonstration.
- `login_test_cases.csv`: 12 test cases with the four required table columns.

The login test cases specify expected behavior derived from the requirements.
The examples use `user1` / `pass123`
and `boundary_user` / `abc123` as registered test accounts.

## View the history

```sh
git log --oneline --graph --all --decorate
```

`feature` is retained. The merge uses `--no-ff` to make branch activity explicit.
The undo uses `git revert --no-edit HEAD`, so both the change and its reversal
remain available to an instructor reviewing the history.

## GitHub status

Public repository: https://github.com/arnav-yadav/git-workflow-assignment-20261115

Public visibility, default branch main, and matching remote main and feature hashes
were verified. Initial publishing output is in evidence/github_integration.txt.
