# AI-skills-installer-windows-for-cline-
System wide installer for all skills needed

# How to use
1.  Save the script as skillsinstaller.ps1.
2.  Open PowerShell as your normal user (not necessarily admin).
3.  Run:

# Full install (includes the large repo – can take time + disk space)
.\skillsinstaller.ps1

# Recommended first run (skip the huge catalog)
.\skillsinstaller.ps1 -SkipLarge

# Force re-download everything
.\skillsinstaller.ps1 -Force -SkipLarge


Notes
•  Size warning: sickn33/agentic-awesome-skills contains thousands of skills. The -SkipLarge switch is recommended unless you really want everything.
•  The script uses shallow clones (--depth 1) to keep downloads fast.
•  Skills are copied (not symlinked) so they work reliably on Windows without Developer Mode.
•  After installation, restart Cline / VS Code (or start a completely new Cline task) so it re-scans the global skill directories.
•  Both ~/.cline/skills and ~/.agents/skills are populated for maximum compatibility with current and future Cline versions + the skills CLI.