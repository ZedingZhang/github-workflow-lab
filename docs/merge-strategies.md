# Merge Strategies

GitHub supports three common pull request merge strategies. The right choice
depends on how much branch history the project wants to preserve.

## Merge commit

Creates a merge commit with both histories intact. This makes the branch boundary
and the pull request integration explicit.

## Squash and merge

Combines the pull request commits into one commit on the base branch. This is useful
when intermediate commits are mostly work in progress.

## Rebase and merge

Replays the pull request commits onto the base branch without a merge commit. This
keeps history linear while preserving individual commits.

## Practice note

Review requirements and branch protection should reflect the risk of the project.
This repository is a low-risk workflow lab; production repositories should normally
require review before merging changes.
