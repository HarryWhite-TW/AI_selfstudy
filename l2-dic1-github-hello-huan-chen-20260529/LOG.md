# From-Scratch Build Log

This log records the full process of creating, running, documenting, and publishing the L2 DIC1 GitHub Hello Page.

## 2026-05-29

### 1. Starting Point

The local working folder was:

```text
C:\Users\admin\Desktop\l2
```

At the beginning, the folder did not contain an `index.html` file and was not a Git repository.

### 2. Recreated the Requested Command

The task shown in the reference image was to create an `index.html` page that:

- says hello;
- shows the name `Huan Chen`;
- displays the current date and time.

The resulting file was created locally:

```text
index.html
```

### 3. Built the HTML Page

The page included:

- a standard HTML document;
- a greeting: `Hello, my name is Huan Chen.`;
- CSS styling for a centered dark interface;
- JavaScript to update the local date and time every second.

The time update logic used:

```javascript
updateDateTime();
setInterval(updateDateTime, 1000);
```

### 4. Ran the Page Locally

The page was opened directly in the browser with:

```powershell
Start-Process -FilePath .\index.html
```

The local run confirmed that the HTML file could be opened and executed as a standalone page.

### 5. Prepared GitHub Publishing

The local folder was checked and found to be:

- not yet initialized as a Git repository;
- missing the GitHub CLI command `gh`.

Because `gh` was unavailable, the connected GitHub tool was used to publish directly to GitHub.

### 6. Chose a Safe GitHub Location

The GitHub account used was:

```text
HarryWhite-TW
```

Available repositories were reviewed. To avoid mixing this work with other projects, the file was placed in the existing `AI_selfstudy` repository under a dedicated folder:

```text
l2-dic1-github-hello-huan-chen-20260529/
```

This made the final GitHub path:

```text
HarryWhite-TW/AI_selfstudy/l2-dic1-github-hello-huan-chen-20260529/index.html
```

### 7. Published `index.html`

The HTML file was created on GitHub with this commit message:

```text
Add L2 DIC1 hello page
```

Commit SHA:

```text
8b0c1b70134c8a193dd4cc3b118bef37269413af
```

Published URL:

```text
https://github.com/HarryWhite-TW/AI_selfstudy/blob/main/l2-dic1-github-hello-huan-chen-20260529/index.html
```

### 8. Created a Reproducible README

A `README.md` file was added locally to explain the project and how to reproduce the work from scratch.

The README includes:

- project purpose;
- file structure;
- local run instructions;
- GitHub publishing location;
- verification checklist;
- notes about the environment.

### 9. Published `README.md`

The README was then uploaded to the same GitHub folder as `index.html`.

Commit message:

```text
Add README for L2 DIC1 hello page
```

Commit SHA:

```text
0f82704ecccce991e82c715733a246349c23c6fa
```

Published URL:

```text
https://github.com/HarryWhite-TW/AI_selfstudy/blob/main/l2-dic1-github-hello-huan-chen-20260529/README.md
```

### 10. Final Local Files

The local working folder contained:

```text
l2/
|-- index.html
|-- README.md
`-- LOG.md
```

## Final Result

The project was successfully created from scratch, opened locally, documented, and published to GitHub in a clearly separated folder.

The GitHub folder for this work is:

```text
https://github.com/HarryWhite-TW/AI_selfstudy/tree/main/l2-dic1-github-hello-huan-chen-20260529
```
