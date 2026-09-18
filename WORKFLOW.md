# Git Team Sync Workflow

## 1. What did the rejected push error message tell you, and why did it happen?
- The rejected push error message said that updates were rejected because remote contains work I didn't
have locally, which is usually caused by another repository pushing to the same ref. This happened because
both clones A and B had conflicting functions that needed to be resolved.

## 2. What's the actual difference between how you resolved Task 3 (merge) vs Task 4 (rebase)?
- Git merge combined the changes from both remote and local branch into a new merge commit. Meanwhile,
Git rebase replayed the local commit on top of the updated remote branch, which produced a more linear
history instead of a separate merge commit.

## 3. What one habit would have avoided both rejected pushes in this lab?
- One good habit would have been to fetch or pull from the remote repository before starting work or pushing.
This would have kept the local branch updated and aware of any changes made by other team members.

## 4. Which approach - merge or rebase - would you default to on a shared team branch, and why?
- When it comes to shared team branches, I would default to the merge approach because it preserves
existing shared histories and does not rewrite commits other members may have already made or worked on.