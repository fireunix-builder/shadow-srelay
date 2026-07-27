# SRelay Builder

Public build and release automation for the private
`fireunix-app/shadow-srelay` repository.

The private source is checked out only on an ephemeral GitHub-hosted runner
using a repository-scoped, read-only PAT. Source files and project build output
are not committed, uploaded, or cached. Release archives contain compiled
binaries and explicitly published runtime templates only.

GitHub Releases are written back to the private SRelay repository through a
separate single-repository write token. This public repository never hosts
Releases; R2 receives only the reviewed binary archives and checksums.
