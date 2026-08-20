# Assignment

<!-- repository-summary -->
A Jenkins CI/CD practice repository for declarative pipelines, Git branches, builds, tests, and post-build actions.
<!-- /repository-summary -->

A small Jenkins CI/CD practice repository used to experiment with declarative
pipelines and Git branching/merging workflows.

## What's here

- **`Jenkinsfile`** — a declarative Jenkins pipeline with `Checkout`, `Build`,
  and `Test` stages, plus `post { success / failure }` hooks. The checkout
  step is wired to pull from the `develop` branch. The build/test steps are
  left as placeholders (`// Your build/test steps here`) for filling in
  project-specific commands.
- **`code.txt`, `log.txt`, `master.txt`, `output.txt`, `public1.txt`,
  `urgent.txt`** — empty placeholder text files. These exist to exercise
  branching/merging behavior across the repo's several branches (`master`,
  `Develop`, `feature/my-feature`, `private`, `public1`, `public2`) rather
  than to hold real content.

## Purpose

This repo isn't an application — it's a sandbox for practicing Jenkins
pipeline syntax and Git branch/merge workflows (multiple long-lived and
feature branches exist in the remote for that purpose).

## Usage

To try the pipeline, point a Jenkins job at this repository and let it pick
up the `Jenkinsfile` from the branch you're testing.
