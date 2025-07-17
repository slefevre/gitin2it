# TODO
 - UPG use default remote instead of assuming `origin`
 - UPG use default branch instead of assuming `main`
 - DOC define approach to verb tenses, nouns, plurals (e.g. `changes`, `change`, `changed`).
 - FEA add filename argument to `delete`.
 - FEA add filename argument to `undelete`.
 - FEA `ignore`: add a file or directory to .gitignore.
 - FEA some command to show files ignored but still tracked
 - FEA `blamedir`: like blame, but shows who introduced files in a directory.
 - FEA `unmodify`: undo modifications, but keep/ignore new files, deletions, etc.
 - FEA `like`: make the current branch just like the state of another branch
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
 - FEA add cherry pick to git stop
 - FEA `harvest` apply a series of cherry picks
 - FEA `reclone` re-clone a repo
 - FEA `outstanding` -- any uncommitted cahnges, stashes, in-progress cherry pick, merge, etc

---

\* Who decides what is intuitive or idiomatic?

> I do.
