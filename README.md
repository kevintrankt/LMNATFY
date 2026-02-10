# LMNATFY — Let Me Notion AI That For You

A simple LMGTFY-style site that creates shareable links. When someone opens the link, they see the question typed into a search box, a cursor clicks Search, then they’re redirected to [Notion AI](https://dev.notion.so/chat) with that question.

## How it works

1. **Home** — Enter a question and get a short shareable URL (e.g. `https://yoursite.com/s/?q=What+is+TypeScript`).
2. **Shared link** — Opens a page that types the question into a search box, animates a cursor clicking Search, then redirects to `https://dev.notion.so/chat?aq=<url-encoded-query>`.

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

Deploy the repo as a static site (e.g. Vercel, Netlify, GitHub Pages). No build step required.
