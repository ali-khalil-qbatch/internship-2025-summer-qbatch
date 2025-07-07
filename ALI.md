# Task 1: Git Rebasing vs Merging

## What is "Merging"?
Merging is the process of taking the changes from one branch (e.g., a feature branch) and integrating them into another branch (e.g., main). When you merge, Git creates a new "merge commit" that combines the histories of both branches. This preserves the complete history and shows that a branch was merged.

**Example:**
```
git checkout main
git merge feature-branch
```

**Key Points:**
- Preserves the full history of both branches.
- Creates a merge commit if there are new commits on both branches.
- Good for keeping context and showing when branches diverged and came together.

## What is "Rebasing"?
Rebasing is the process of moving or combining a sequence of commits to a new base commit. Instead of creating a merge commit, rebasing rewrites the commit history so that your changes appear as if they were made on top of the latest commit from the target branch. This results in a linear history.

**Example:**
```
git checkout feature-branch
git rebase main
```

**Key Points:**
- Rewrites commit history for a cleaner, linear project history.
- Does not create a merge commit.
- Can make history easier to read, but should be used with caution (especially on shared branches). 

### Summary Table
|            | Merging                        | Rebasing                          |
|------------|-------------------------------|-----------------------------------|
| History    | Preserves branch structure     | Linearizes history                |
| Commit     | Creates a merge commit         | Rewrites commits, no merge commit |
| Use case   | When you want to keep context  | When you want a clean history     |
| Command    | git merge branch               | git rebase branch                 |

**In short:**
- Use merge to combine branches and keep the full history.
- Use rebase to make your history linear and tidy, as if your work was done on top of the latest changes.

---

# Task 2: Git Command Explanations

For detailed explanations of various Git commands, please refer to the following Google Docs link:
[Click here](https://docs.google.com/document/d/12qufZhKjhnJHmoMq0SB_KvLSYVy30wgnz5-Ev0e2Fjs/edit?usp=sharing)