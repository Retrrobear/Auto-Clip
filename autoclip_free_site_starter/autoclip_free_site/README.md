# AutoClip free website starter

This is a static website designed for GitHub Pages. It does not host video processing or store Google credentials.

## Before publishing

1. Create a separate, reusable Colab notebook for your friend to use.
2. Share that notebook with your friend (Viewer access is enough if they make their own copy; Editor access lets them run the shared original, but separate copies are safer).
3. Open `index.html` and find:
   `const COLAB_NOTEBOOK_URL = "";`
4. Paste the shared Colab notebook URL between the quotes.
5. Upload `index.html` to a GitHub repository.
6. In the repository, open Settings → Pages → Deploy from a branch → `main` → `/ (root)` → Save.
7. GitHub Pages will provide the public website URL. Share that URL with your friend.

## Important

- This website is only the front end. It launches the Colab notebook; it does not directly control a running Colab runtime.
- The Colab notebook must contain the actual AutoClip processing code and must be made safe for other users. Do not publish your personal OAuth client secret, refresh token, or private credentials in a public notebook.
- Each user must authorize their own Google Drive and YouTube access.
- Colab Free may disconnect and has usage limits. The website can be online 24/7, but video processing cannot be guaranteed to run 24/7.
- This setup uses free hosting and user-owned Google storage/processing, subject to provider limits and terms.
