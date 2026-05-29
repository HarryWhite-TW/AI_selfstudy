# AI_selfstudy

# L2 DIC1 GitHub Hello Page

This repository folder documents a simple from-scratch workflow:

1. Create a single-page `index.html`.
2. Show a greeting with the name `Huan Chen`.
3. Display the current local date and time.
4. Open the page locally in a browser.
5. Publish the result to GitHub in an isolated folder to avoid mixing it with other projects.

## Project Output

The final page displays:

```text
Hello, my name is Huan Chen.
```

It also updates the current local date and time once per second with JavaScript.

## File Structure

```text
l2/
|-- index.html
`-- README.md
```

On GitHub, the file was published under a dedicated folder:

```text
AI_selfstudy/
`-- l2-dic1-github-hello-huan-chen-20260529/
    `-- index.html
```

## Reproduce From Scratch

### 1. Create a new working folder

```powershell
New-Item -ItemType Directory -Path .\l2
Set-Location .\l2
```

### 2. Create `index.html`

Create a file named `index.html` and add the page content. The page should include:

- Standard HTML document structure.
- A greeting that says `Hello, my name is Huan Chen.`
- CSS styling for the layout and visual design.
- JavaScript that updates the current local date and time every second.

The key JavaScript logic is:

```html
<script>
  const dateTime = document.querySelector("#dateTime");

  function updateDateTime() {
    const now = new Date();
    dateTime.textContent = new Intl.DateTimeFormat("en-US", {
      dateStyle: "full",
      timeStyle: "medium"
    }).format(now);
  }

  updateDateTime();
  setInterval(updateDateTime, 1000);
</script>
```

### 3. Run the page locally

Open the file directly in a browser:

```powershell
Start-Process -FilePath .\index.html
```

Expected result:

- The browser opens `index.html`.
- The page shows the greeting.
- The date and time update automatically.

### 4. Publish to GitHub without mixing projects

To avoid confusion with other GitHub projects, publish the page inside a uniquely named folder.

Repository used:

```text
HarryWhite-TW/AI_selfstudy
```

Dedicated folder used:

```text
l2-dic1-github-hello-huan-chen-20260529/
```

Published file path:

```text
l2-dic1-github-hello-huan-chen-20260529/index.html
```

Commit message used:

```text
Add L2 DIC1 hello page
```

Commit SHA:

```text
8b0c1b70134c8a193dd4cc3b118bef37269413af
```

GitHub URL:

```text
https://github.com/HarryWhite-TW/AI_selfstudy/blob/main/l2-dic1-github-hello-huan-chen-20260529/index.html
```

## Verification

After publishing, verify the result by checking:

1. The file exists at the GitHub path above.
2. The file is inside the dedicated folder, not mixed into another project root.
3. The page title is `Hello - Huan Chen`.
4. The page contains the greeting text.
5. The JavaScript includes `setInterval(updateDateTime, 1000)`.

## Notes

- The local folder was not originally a Git repository.
- GitHub CLI was not available in the environment.
- The GitHub connector was used to create the remote file directly.
- The dedicated folder name includes the project label and date to keep it distinct from other GitHub content.
