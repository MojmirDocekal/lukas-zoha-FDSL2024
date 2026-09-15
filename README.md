# Working on your article in this repository

## What this repository is for

This repository is used to write and revise your article in `main.tex` and to track editorial feedback through GitHub Issues.

A few quick terms:
- **GitHub** is the website where the project lives, so everyone can see the files, comments, and changes.
- A **commit** is a saved set of changes with a short message describing what you changed.
- **Push** means sending your committed changes to the repository so others can see them and the PDF can be rebuilt.

## Summary of steps

1. Open **`main.tex`** in the repository file list.
2. Edit it either:
   - directly on GitHub (pencil icon), or
   - in online VS Code (`github.dev`), if you prefer a larger editor.
3. If you use `github.dev`, you may want to install **LaTeX Workshop** for easier TeX editing.
4. **Commit and push your changes** with a short message.
5. Check the **Issues** tab for requested corrections from editors, and discuss any questions there.
6. After each push, wait about **6 minutes** for compilation.
7. Download the PDF from **Actions → latest run → Artifacts → `compiled-pdf`** (ZIP file).

---

## 1) Edit `main.tex`

### Option A (recommended for quick edits): directly on GitHub

1. Open the repository in your browser.
2. In the file list, click **`main.tex`**.
3. Click the **pencil icon (Edit this file)** in the top-right.
4. Make your changes and save them by committing (see section 3).

### Option B (recommended for bigger edits): online VS Code (`github.dev`)

1. Open the repository page.
2. Open it in `github.dev` by either:
   - pressing **`.` (dot)** on the repository page, or
   - changing `github.com` in the URL to `github.dev`.
3. In the left Explorer panel, click **`main.tex`** and edit it there.

### Option C (for experienced users)

If you normally work locally with `git pull` / `git push`, you can use your standard workflow.

## 2) In `github.dev`, install a LaTeX extension (helpful)

In online VS Code:

1. Open the **Extensions** panel (left sidebar, square icon).
2. Search for **LaTeX Workshop**.
3. Click **Install**.

Why this helps:
- better TeX syntax highlighting,
- command / IntelliSense support,
- easier navigation in larger `.tex` files.

Preview and build features may be limited in browser VS Code, but the editing support is still very useful.

## 3) Commit and push your changes

After editing, save your work with a commit and push it so editors can see it and the PDF can be rebuilt.

### On GitHub web editor

1. Click **Commit changes…** (top-right).
2. Write a short commit message, for example: `Fix typo in section 2`.
3. Choose **Commit directly to the main branch** unless you were told to do something else.
4. Click **Commit changes**.

### In `github.dev`

1. Open the **Source Control** panel (branch icon on the left).
2. Review the changed files.
3. Enter a commit message.
4. Click **Commit**.
5. Click **Sync Changes** / **Push** if prompted.

### Referencing issues in commit messages

If your commit addresses an issue, you can reference its number in the commit message so GitHub links them automatically.

Examples:
- `Fix example in section 3 (fixes #12)`
- `Improve introduction clarity (addresses #12)`
- `Adjust wording in methods section (relates to #12)`

If the commit fully resolves the issue, use **`fixes #ISSUE_NUMBER`** so GitHub can close it automatically when the commit is merged.

## 4) Use Issues for requested corrections

- Open the **Issues** tab to see what needs to be fixed.
- Each issue describes a requested correction from the editors.
- You can discuss details in the issue comments if something is unclear.
- Most importantly: **apply the correction in `main.tex`, then commit and push** as described above.
- Repeat until all assigned or open issues are resolved.

## 5) Find the compiled PDF in GitHub Actions

Each push triggers automatic compilation of the PDF.

To download it:

1. Open the **Actions** tab.
2. Click the **most recent workflow run**.
3. Scroll to **Artifacts**.
4. Download **`compiled-pdf`** (ZIP file).

Notes:
- Compilation is not immediate; it usually takes about **6 minutes**.
- If you don’t see the artifact yet, wait a bit and refresh the run page.

---

If anything is unclear, ask in the relevant issue and tag the editors.
