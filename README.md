# Auto Design Scout

A Claude skill for automotive HMI and cockpit design students seeking internships and graduate roles. It connects career direction with current openings at automakers and suppliers, then helps set up reminders for new roles and approaching deadlines.

## Why it exists

Automotive design internships and graduate programmes open on different schedules. A student may have a portfolio ready and still discover a suitable role shortly before applications close. Searching also takes time when the student is unsure which job titles, company types or recruitment windows fit their background.

This workflow combines those tasks. It uses a CV or a short profile to identify relevant design directions, checks official recruitment channels for current opportunities, and explains why each recommendation fits. The channel list and recruitment-window guidance focus on China's automotive hiring market.

## How it works

Share your CV, or describe your education, graduation year, portfolio focus and experience. The skill suggests a primary direction and, where useful, one adjacent direction, with job titles you can search for and an assessment of the current internship or graduate recruitment window. If you already know your direction, you can go straight to an openings scan.

Your preferred cities, company types and role types guide the search. Results distinguish confirmed openings from opportunities whose status could not be verified, include official application links where available, and explain fit and timing. Salary ranges, relocation policies and estimated future opening dates are supporting context when reliable information is available; estimates should remain labelled as estimates.

After the initial scan, you can choose a company scope and reminder frequency. Automatic monitoring depends on the host's scheduling tools and notification support. When those tools are unavailable, the workflow provides a manual scan prompt instead of claiming that monitoring is running.

## Use the skill

For a Claude environment that supports custom skill uploads, download this repository and package `SKILL.md` and its `references/` directory together, following that environment's skill installation instructions. For Claude Code, place the repository folder at `~/.claude/skills/auto-design-scout/`, keeping `SKILL.md` at the folder root. The repository provides skill instructions and reference files; it is not a standalone recruitment application.

You can start with: “Help me find automotive HMI design internships that fit my CV,” or “Check which automakers and suppliers are hiring graduate cockpit designers in my preferred cities.” The current skill and reference material are written in Chinese for the hiring market they cover; this public overview is in English.

## Repository structure

```text
auto-design-scout/
├── SKILL.md                      # Workflow and operating rules
├── automotive-jobhunting.md      # Additional job-search material
└── references/
    ├── channels.md               # Official recruitment channels for about 45 companies
    ├── direction-map.md          # Direction, timing and company-fit guidance
    ├── detection.md              # Scanning and opening-status reporting
    └── push-setup.md             # Scheduled monitoring and fallback setup
```

## Sources and maintenance

The recruitment URLs in `references/channels.md` were originally researched in August 2026. Recruitment sites and cohort-specific domains change, so this is a maintained starting list rather than a guarantee that every link remains current. The workflow includes fallback searches; corrections and new official channels are welcome through pull requests.

Current openings and deadlines should be checked against the employer's official channels. An unsuccessful scan means that the opening could not be confirmed, not that no opening exists. This project is independent of the employers and recruitment platforms it references, and its recommendations are job-search guidance rather than guarantees of eligibility or employment.

## License

[MIT](LICENSE)
