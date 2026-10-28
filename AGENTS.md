# AGENTS.md - AiFinPay .github Directory

## High-signal context for OpenCode agents in this repo

### Purpose
This repository is the AiFinPay organization's GitHub `.github` directory containing organizational configuration, OpenCode skills, and documentation assets.

### What this repo contains

**Primary files to inspect first:**
- `profile/README.md` - Main organizational README with AiFinPay project overview and integration guides
- `.opencode/skills/seo-optimization/SKILL.md` - SEO optimization skill for website auditing and improvement
- Assets in `assets/` - Chain network logos for documentation

**OpenCode-specific files:**
- `.opencode/skills/seo-optimization/SKILL.md` - Installable OpenCode skill for SEO optimization
- `.gitignore` - Git ignore rules for the .github directory

### Key conventions and constraints

**Profile README structure:**
- Contains comprehensive AiFinPay documentation and integration guides
- Maintained as a marketing/documentation file, not code documentation
- Updated frequently with network/chain additions (14 networks tracked)
- Serves as the primary user-facing documentation source

**OpenCode skills:**
- SEO optimization skill is an organization-specific addition
- Skills are installed via `npx skills add` command
- Must respect skill's operating rules, especially inspection-before-prescription

**Asset management:**
- Chain logos stored in `assets/chains/` for documentation use
- Binary PNG files (robinhoood.png) and SVG files
- Updated when new networks are added to supported chains

### Command patterns

**For SEO analysis:**
```bash
# Use the organization's SEO skill for website optimization
npx skills add AiFinPay/skill
```

**For documentation:**
```bash
# Reference AiFinPay's main documentation and integration guides
cat profile/README.md
```

### Investigation approach

1. **Start with `profile/README.md`** - This is the executable source of truth for the organization
2. **Check OpenCode skills** - The SEO optimization skill is the only installable skill available
3. **Review recent changes** - Git log shows frequent updates to supported networks and documentation

### Important constraints to preserve

- Profile README changes propagate to organization documentation
- Chain logos must be updated when new networks are added
- SEO skill must follow its 10 operating rules, especially "inspect before prescribing"
- Network coverage changes require both documentation and logo updates

### When this matters

Agents working in this repo need this guidance to:
- Avoid treating profile/README.md as code documentation
- Understand why SEO skills need inspection of multiple factors before recommendations
- Know when to update chain assets alongside network additions
- Respect the organization's focus on developer-first, secure documentation practices