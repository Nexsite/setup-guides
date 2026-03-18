# setup-guides

Setup guides for Safe Site Utility Services employees hosted on Cloudflare Pages.

**Live site:** [setup.nexsite.co](https://setup.nexsite.co)

## Guides

### `/onedrive` — OneDrive & SharePoint Setup
Guides employees through setting up OneDrive and accessing shared drive files after the Google Drive to SharePoint migration.

- **Desktop (OneDrive App)** — First-time setup, finding the OneDrive cloud icon (blue = signed in, grey = needs sign-in), accessing shared drive shortcuts in File Explorer/Finder
- **OneDrive Web** — Navigating office.com's Copilot interface to OneDrive via Apps, finding shared drive shortcuts in My Files
- **FAQ** — Common questions about the migration, shared drives, Google Drive read-only access, and file sharing
- **IT Helpdesk** — Direct links to submit tickets, call, or email support

Features a toggleable Desktop/Web view, system-theme dark mode, and responsive mobile layout.

## Deployment

Hosted on Cloudflare Pages. To deploy:

```bash
npx wrangler pages deploy . --project-name setup-guides
```

Custom domain `setup.nexsite.co` requires a CNAME record pointing to `setup-guides.pages.dev`.

## Related projects

- **[shortcutter](https://github.com/Nexsite/shortcutter)** — Automates creation of OneDrive shortcuts to SharePoint document libraries for all users
- **[gdrivexfer-refreshed](https://github.com/Nexsite/gdrivexfer-refreshed)** — Google Drive to SharePoint permission migration pipeline
- **[migrate-dashboard](https://migrateprogress.nexsite.co)** — Employee-facing migration progress dashboard
