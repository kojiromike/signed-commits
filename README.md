# Git Signed Commits

I'm curious about the tradeoffs between signed commits and usability.

## How it works

This is pretty much a TL;DR of the [git documentation](http://git-scm.com/book/en/v2/Git-Tools-Signing-Your-Work).

1. Create a GPG key if you don't already have one.
2. Sign commits using git (1.7.1 or greater) and the `-S` flag.
3. Look at signatures in `git log` using `--show-signature`.
4. Merge using `--verify-signatures` will fail if a signature is missing from a commit.

