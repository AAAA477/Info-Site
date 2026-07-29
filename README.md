# PIWC Edmonton North Canada Forms

A small static info site for church form links. It is ready to deploy on Netlify with no build step.

## Local Preview

Open `index.html` directly in a browser, or run a temporary static server:

```bash
npx serve .
```

## Deploy To Netlify

### Option 1: Netlify Website

1. Push this folder to a GitHub repository.
2. In Netlify, choose **Add new site** then **Import an existing project**.
3. Select the repository.
4. Use these build settings:
   - Build command: leave blank
   - Publish directory: `.`
5. Deploy the site.

### Option 2: Netlify CLI

For CLI deploys, use Node.js 22 or newer. The Netlify website deploy above does not require Node.

Install and log in:

```bash
npm install -g netlify-cli
netlify login
```

Link the folder to a Netlify site:

```bash
netlify init
```

Deploy a preview:

```bash
netlify deploy --dir .
```

Deploy to production:

```bash
netlify deploy --prod --dir .
```
