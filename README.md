# Bracket Lab

A static, browser-based single-elimination tournament bracket with the shadcn/ui-inspired `bJMV1TuK` preset (Nova / Stone + Green).

## Deploy to GitHub Pages

1. Create a new **public** GitHub repository, for example `bracket-lab` (GitHub Free supports Pages from public repositories).
2. Upload the **contents** of this folder to the repository root: `index.html`, `.nojekyll`, and `README.md`. You can use **Add file → Upload files** on GitHub. Remember to include the hidden `.nojekyll` file if uploading individually, but `index.html` is sufficient for this straightforward site.
3. Open the repository's **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**, then choose branch **main** and folder **/(root)**. Click **Save**.
5. Once GitHub Pages finishes deploying, open `https://YOUR_USERNAME.github.io/bracket-lab/` (replace both username and repository name as needed).

## Behavior

- This app works entirely in the browser; no build command or server required.
- Picks, bracket state, and theme preference are saved in this browser's `localStorage`. Each device/browser keeps its own copy. There is **no synchronization between devices**.
- Use **Export** to back up your bracket as JSON, and **Import** to restore it or move it to another browser.
- Font is loaded from Google Fonts; with no internet connection the browser may use a system fallback font.

## Local preview

Open `index.html` in your browser. Alternatively, from the folder:

```bash
python3 -m http.server 8000
```

Visit `http://localhost:8000/`.
