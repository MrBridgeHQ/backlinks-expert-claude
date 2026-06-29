# Installation — Backlinks Expert skill

This skill is designed to be installed at the **user level** in Claude Code, so it's available across all your projects without copying it into each repo. It is pure doctrine (Markdown only) — there are no scripts and no dependencies to install.

## Prerequisites

- Claude Code installed and working.
- A terminal with `unzip` (macOS, Linux) or PowerShell with `Expand-Archive` (Windows).

## Installation

### macOS / Linux

```bash
# 1. Create the user-level skills directory if it doesn't exist
mkdir -p ~/.claude/skills

# 2. Unzip the skill into that directory
unzip backlinks-expert.zip -d ~/.claude/skills/

# 3. Verify the structure
ls ~/.claude/skills/backlinks-expert/
# Expected: SKILL.md  README.md  INSTALL.md  references/
```

### Windows (PowerShell)

```powershell
# 1. Create the user-level skills directory if it doesn't exist
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills"

# 2. Unzip the skill into that directory
Expand-Archive -Path .\backlinks-expert.zip -DestinationPath "$env:USERPROFILE\.claude\skills\"

# 3. Verify the structure
Get-ChildItem "$env:USERPROFILE\.claude\skills\backlinks-expert\"
# Expected: SKILL.md  README.md  INSTALL.md  references/
```

You can also install it per-project by placing the `backlinks-expert/` directory under a project's `.claude/skills/` instead of the user-level one.

## Verification

Open Claude Code and ask:

> "What skills do you have access to?"

You should see `backlinks-expert` in the list. If not, check that the SKILL.md file is at the path:

- macOS / Linux: `~/.claude/skills/backlinks-expert/SKILL.md`
- Windows: `%USERPROFILE%\.claude\skills\backlinks-expert\SKILL.md`

## First test

In any Claude Code session, ask:

> "Plan a link-building campaign for a brand-new SaaS landing page — give me the tactic mix, anchor distribution, and velocity."

The skill should activate, route to STRATEGIZE mode, and produce a per-property campaign brief (posture → tier ratio → anchor mix → velocity → sequence → KPIs), pulling from `references/campaign-planning.md` and `references/property-profiles.md`.

To test the qualification gate:

> "Here's a 'top 50 dofollow forums' list — which of these are actually worth using?"

The skill should route to DISCOVER/QUALIFY, treat every entry as UNVERIFIED, and walk the `references/qualification.md` checklist (relevance → live dofollow → indexation → metric → spam → traffic → OBL → penalty/PBN → activity) rather than trusting the list's claims.

## Updating the skill

To install a newer version, just replace the directory:

```bash
# macOS / Linux
rm -rf ~/.claude/skills/backlinks-expert
unzip backlinks-expert.zip -d ~/.claude/skills/
```

## Uninstalling

```bash
# macOS / Linux
rm -rf ~/.claude/skills/backlinks-expert

# Windows (PowerShell)
Remove-Item -Recurse -Force "$env:USERPROFILE\.claude\skills\backlinks-expert"
```

## Troubleshooting

**Skill doesn't activate when expected.**
Auto-activation depends on the `description` in `SKILL.md`'s frontmatter. Triggers include: "build backlinks", "link building", "off-page SEO", "dofollow forums", "guest posts", "niche edits", "anchor text strategy", "find link opportunities", EN or FR. If your phrasing doesn't match, force activation: "Use the `backlinks-expert` skill to..."

## Support

This skill is link-building doctrine. To improve it (new opportunity types, refreshed seed targets, updated policy notes), edit the relevant `references/*.md` file directly — the reference files are the authoritative surface and `SKILL.md` routes to them.
