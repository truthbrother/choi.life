žée

## Syncing docs to the master vault
This repo's Markdown mirrors into `master_markdowns` at `_SOURCE REPO DOCS/choi.life/`
(markdown only, paths preserved). This repo is the source of truth for its `.md` â€”
never hand-edit its vault snapshot. After changing `.md`, run the canonical script
(don't copy/flatten/rename by hand):
    ~/Documents/master_markdowns/tools/sync-repo-docs.sh "$(git rev-parse --show-toplevel)"
An hourly sweep also re-syncs automatically; the script is just for immediacy.