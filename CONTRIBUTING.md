# Contributing Yen Project

Before creating any pull requests, please check if all requirements are satisfied.

## Version control & PR

### Fowrkflow

The project is driven by git flow workflow.

> Read more at [atlassian.com](https://www.atlassian.com/git/tutorials/comparing-workflows/gitflow-workflow)

### Commit description

All commits should be signed with GPG signature & have a properly formatted message.
Each commit should contain atomic changes.

A PR should not contain more than 1000 LOC for addition or removal in total.

There are following commit types:

- FEATURE - for all new functionality;
- FIX - for all bug fixes;
- DOC - update of the documentation;
- MISC - mostly for any changes in configurations, pipelines, packaging, etc. (if FEATURE or FIX types are not acceptable);
- CHORE - for changes in read-me files, etc.

### PR with a bug fix

If the PR contains a fix for a bug and the bug ticket exists, it should be linked in the PR description.

## Source code

All code in the commit should be formatted with the clang & CMake format tools.

> Code should be compiled without errors.

## Tests

All tests should be passed.

## Enviroment

The project is aimed in first place to be developed in Alpine Linux environment, with following porting to other distributive.

