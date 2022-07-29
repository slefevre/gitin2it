# gitin2it
a set of aliases to make complex or rare git actions more intuitive

# Installation
Add the following lines to your ~/.gitconfig
```
[include]
path = path/to/gitin2it/aliases
```
where `path/to/gitin2it/aliases` is the path, relative from the location of your `.gitconfig` file, to the `aliases` file in this repo.

# Documentation Syntax

alias-name required-argument [optional-argument|'default-value'] [optional-argument]

# What belongs here?
Git aliases that 
 - are intuitively, idiomatically named *
 - replace commands that have switches...
   - `git ignored` vs. `git ls-files --others --exclude-standard --ignored`

     *show ignored files in repository*
 - ... or syntax
   - `git back` vs. `git checkout HEAD~1` 
 - are named after google searches or stack overflow questions
   - "How do I unstage changes that I've commited?"
     `git unstage` vs. `git reset`
 - Implement as-of-yet-unimplemented features
   - `git diff-stat` automatically sizes `stat` output to terminal width
 - Wield the power of shell commands
   - two sequential commands: `git scrub` vs. `git reset --hard; git clean -f -f -d;` to remove all changes and new files
   - optional common defaults: 
     - `git set-upstream` // defaults to `origin` 
     - `git set-upstream remote-other-than-origin` // sets the upstream remote to (an existing) one other than origin

# What doesn't belong here?
  - abbrevations
    - `git co` for `git checkout`
  - personalizations or niceities, such as a custom log format with certain fields, colors, etc.

# TODO
 - DOC define approach to verb tenses, nouns, plurals (e.g. `changes`, `change`, `changed`).
 - FEA add filename argument to `delete`.
 - FEA add filename argument to `undelete`.
 - FEA `ignore`: add a file or directory to .gitignore.
 - FEA some command to show files ignored but still tracked
 - FEA `blamedir`: like blame, but shows who introduced files in a directory.
 - FEA `unmodify`: undo modifications, but keep/ignore new files, deletions, etc.
 - BUG `copy` throws error when asked to copy a file from another branch which doesn't exist on the current branch.
    "fatal: Path 'resources/assets/js/ckeditor.js' exists on disk, but not in the index." 
 - BUG make `resolve` use repo root for commit message
 - FEA `is-staged` are there changes staged?
 - FEA `is-modified` are there local modifications?
 - FEA `is-changed` are there changes?
 - FEA `is-stashed` are there items in the stash?
 - FEA `is-deleted` are there uncommitted deletes?
 - FEA `is-new` are there new uncommited files?
 - FEA `is-untracked` are there files that are not being tracked?
 - FEA `is-dirty` are there any unsaved, uncommitted changes?
 - FEA `ignore`
 - FEA `forget`
 - FEA `is-`
 - FEA `tracking/tracked`
 - FEA `remote mv`
 - FEA `chmod`
 - FEA `wipe` delete the repo with --mirror --force
---

\* Who decides what is intuitive or idiomatic?

> I do. 
