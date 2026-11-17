# Cline Skills Installer

[![PowerShell](https://img.shields.io/badge/PowerShell-5.1%2B%20%7C%207%2B-blue.svg)](https://docs.microsoft.com/powershell/)
[![Platform](https://img.shields.io/badge/Platform-Windows-0078D4.svg)](https://www.microsoft.com/windows)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Automated PowerShell script that installs popular **Agent Skills** packs system-wide for [Cline](https://cline.bot).

Skills are installed into both global locations used by Cline so they are available across **all projects**.

---

## Features

- One-command installation of high-quality skill packs
- Shallow clones for fast downloads
- Automatic discovery of every folder containing a `SKILL.md`
- Installs to both Cline global paths for maximum compatibility
- Safe to re-run (skips existing skills unless forced)
- Optional exclusion of the very large skills catalog

---

## What Gets Installed

| Repository | Description | Size |
|------------|-------------|------|
| [anthropics/skills](https://github.com/anthropics/skills) | Official Anthropic skills collection | Small |
| [obra/superpowers](https://github.com/obra/superpowers) | High-quality coding workflow & methodology | Medium |
| [mattpocock/skills](https://github.com/mattpocock/skills) | Practical engineering skills (`grill-me`, `to-spec`, TDD…) | Small |
| [sickn33/agentic-awesome-skills](https://github.com/sickn33/agentic-awesome-skills) | Large curated catalog of agent skills | **Very Large** |

> **Recommendation:** Start with `-SkipLarge` unless you specifically need the full catalog.

---

## Target Locations

Skills are installed system-wide into: