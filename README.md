# gitin2it
set of aliases to make git actions more intuitive

# Installation
I recommend that you clone this repo into your home dir, then add this to your user's `.gitconfig`

```
[include]
path = ./gitin2it/gitin2it
```

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

 - `ignore` command

\* Who decides what is intuitive or idiomatic?

> I do. 
