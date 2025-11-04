# btrfs snapshot utilities

*_pre-release: future updates might introduce breaking changes_*

# Usage

These tools are written with a sysadmin use-case in mind and many require sudo
privileges. They're generally written to be run by a cron job but should work
if invoked by a user.

Executable scripts in `./bin/` should by symlinked to somewhere in your path,
or you can add `./bin/` to your path.

## `increment_snapshot`

Creates a snapshot and sends an incremental backup. Requires a parent snapshot.