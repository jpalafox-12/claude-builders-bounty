# Generate Changelog

A Claude Code skill and bash script that generates a structured CHANGELOG.md from git history.

## Setup (3 steps)

1. Clone this repo or copy `changelog.sh` and `SKILL.md` to your project
2. Make the script executable: `chmod +x changelog.sh`
3. Run: `bash changelog.sh`

## Features

- Auto-categorizes commits into Added / Fixed / Changed / Removed
- Supports conventional commit prefixes (feat:, fix:, chore:, etc.)
- Works with or without git tags
- Generates clean, formatted Markdown output

## Usage

### As a bash script
```bash
bash changelog.sh
```

### As a Claude Code skill
Use the `/generate-changelog` command in Claude Code.

### Custom output file
```bash
bash changelog.sh CHANGES.md
```

## Example Output

```markdown
# Changelog

All notable changes to my-project will be documented in this file.

## [v1.2.0] - 2026-07-17

### Added
- feat: add user authentication
- feat: add dark mode support

### Fixed
- fix: resolve login timeout issue
- fix: correct date formatting

### Changed
- update: improve performance
- refactor: simplify error handling
```
