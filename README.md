# LMNATFY — Let Me Notion AI That For You

A simple LMGTFY-style site that creates shareable links. When someone opens the link, they see the question typed into a search box, a cursor clicks Search, then they’re redirected to [Notion AI](https://www.notion.so/chat) with that question.

## How it works

1. **Home** — Enter a question and get a short shareable URL (e.g. `https://yoursite.com/s/?q=What+is+TypeScript`).
2. **Shared link** — Opens a page that types the question into a search box, animates a cursor clicking Search, then redirects to `https://www.notion.so/chat?aq=<url-encoded-query>`.

## Run locally

Serve the project with any static server, for example:

```bash
# Python 3
python3 -m http.server 8080

# Node (npx)
npx serve .

# Then open http://localhost:8080
```

## Deploy

No build step required — just deploy the folder as a static site.

### GitHub Pages

1. Push this repo to GitHub.
2. Open the repo on GitHub → **Settings** → **Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Under **Branch**, pick your default branch (e.g. `main`) and set the folder to **/ (root)**.
5. Click **Save**. The site will be at `https://<username>.github.io/<repo-name>/`.

If the repo name is `lmnatfy`, shareable links will look like:  
`https://<username>.github.io/lmnatfy/s/?q=Your+question`.

### Other hosts

You can also deploy the same static files to [Vercel](https://vercel.com), [Netlify](https://netlify.com), or any static hosting. No build or config needed.
