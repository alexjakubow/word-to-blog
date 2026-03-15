# Word to Blog

A lightweight, browser-based tool for converting `.docx` files into clean HTML or Markdown — ready to paste into your blog or service of choice (i.e., Squarespace, WordPress, etc.).

**[Live demo →](https://alexjakubow.github.io/word-to-blog)**

## Features

- Drag-and-drop `.docx` upload
- Live **Preview** tab — see how your post will look before copying
- **HTML** tab — clean markup to paste into your editor's Code Block
- **Markdown** tab — for use with your editor's Markdown Block
- Image detection with re-upload reminder
- Runs entirely in the browser — **your files never leave your machine**
- Dark mode support

## How to use

1. Open the app
2. Drag your `.docx` file onto the drop zone (or click to browse)
3. Check the **Preview** tab to verify formatting
4. Switch to **HTML** or **Markdown** and click **Copy**
5. Paste into your Squarespace blog post

### In Squarespace

- **HTML output** → add a **Code Block** to your page, set it to HTML, and paste
- **Markdown output** → add a **Markdown Block** and paste

> **Images:** Your blogging platform likely works best with images uploaded via its own Image Block. After pasting, replace any inline images with proper image blocks.

## Deploy to GitHub Pages

### First-time setup

1. [Fork this repository](https://github.com/your-username/word-to-blog/fork) or push it to a new repo on your GitHub account
2. Go to your repo on GitHub → **Settings** → **Pages**
3. Under **Source**, select **Deploy from a branch**
4. Set **Branch** to `main` and folder to `/ (root)`
5. Click **Save**

GitHub will publish the site at:

```
https://your-username.github.io/word-to-blog
```

It may take 1–2 minutes on first deploy. After that, any push to `main` will automatically redeploy.

### Local development

No build step needed — just open `index.html` in a browser:

```bash
# Option 1: open directly
open index.html

# Option 2: serve locally (avoids any file:// quirks)
npx serve .
# or
python3 -m http.server 8080
```

## Tech

- [mammoth.js](https://github.com/mwilliamson/mammoth.js) for `.docx` → HTML/Markdown conversion
- Vanilla JS, no framework, no build step
- Hosted via CDN from `cdnjs.cloudflare.com`
