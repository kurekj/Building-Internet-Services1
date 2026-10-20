# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repository is

A freshly initialised git repository (`main`, remote `origin` =
`https://github.com/kurekj/Building-Internet-Services1.git`) for the **Building Internet
Services** course at SGGW, winter semester 2026/27. It is the only git repo in the teaching
folder; everything around it (`../raport.csv`, rosters, timetables) is plain files governed by
the parent `CLAUDE.md` files — read those before touching any roster data.

There is **no source code, build system, lint or tests** yet. Nothing to build or run.

## Current contents

- `git.txt` — the GitHub "create a new repository" bootstrap commands, committed as the first
  file. Note it references a `README.md` that was never actually created.
- `Jaroslaw_Kurek_SGGW_profile.docx` — **untracked**, a researcher-profile summary compiled from
  the SGGW Knowledge Base. It contains personal contact details (phone, e-mail, room number),
  so do not commit or push it unless the user explicitly asks.

## Environment notes

- `core.autocrlf=true` is set, so files are checked out with CRLF on Windows; write new text
  files with LF and let git normalise.
- The default `python` has no `python-docx`/`openpyxl`/`pandas`. Read `.docx`/`.xlsx` via
  `zipfile` + the XML inside, or install the package first. Run such scripts with `python -I`.
- Shell is PowerShell; the parent path contains `!`, so quote paths in Bash.
- Commits so far were authored as `unknown <j.kurek@rynekpierwotny.pl>`; the repo has no local
  `user.name`/`user.email` override, so check `git config` before committing on the user's behalf.
