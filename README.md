# Intro

# Subtrees

This repository uses subtrees.
If you want to modify the following subtree "repos" please read the following chapters.

## Adding remotes for our subtrees

    git remote add ansible-roles https://github.com/rattermeyer/ansible-roles.git

## Updating roles subtree

    git subtree pull --prefix=roles --squash ansible-roles master

## Backporting changes to common codebase (these should be applicable to all container repos that use roles as a subtree)

    git subtree push -P roles ansible-roles master

