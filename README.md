# postcutover-instructions

Post-migration setup guide for Safe Site Utility Services employees transitioning from Google Workspace to Microsoft 365.

**Live site:** [postcutover.nexsite.co](https://postcutover.nexsite.co)

## What is this?

A static single-page site that guides employees through setting up OneDrive and accessing their shared drive files after the Google Drive to SharePoint migration. The site covers:

- **Desktop (OneDrive App)** — First-time setup, finding the OneDrive cloud icon (blue = signed in, grey = needs sign-in), accessing shared drive shortcuts in File Explorer/Finder
- **OneDrive Web** — Navigating office.com's Copilot interface to OneDrive via Apps, finding shared drive shortcuts in My Files
- **FAQ** — Common questions about the migration, shared drives, Google Drive read-only access, and file sharing
- **IT Helpdesk** — Direct links to submit tickets, call, or email support

Features a toggleable Desktop/Web view, system-theme dark mode, and responsive mobile layout.

## Deployment

Hosted on Cloudflare Pages. To deploy:

```bash
npx wrangler pages deploy . --project-name postcutover-instructions
```

Custom domain `postcutover.nexsite.co` is configured in the Cloudflare dashboard.

## Related projects

- **[shortcutter](https://github.com/Nexsite/shortcutter)** — Automates creation of OneDrive shortcuts to SharePoint document libraries for all users
- **[gdrivexfer-refreshed](https://github.com/Nexsite/gdrivexfer-refreshed)** — Google Drive to SharePoint permission migration pipeline
- **[migrate-dashboard](https://migrateprogress.nexsite.co)** — Employee-facing migration progress dashboard
