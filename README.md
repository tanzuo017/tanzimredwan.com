# tanzimredwan.com

Personal website of Tanzim Redwan: a plain static site (no build step) that Hostinger can serve straight from this
repository.

## What's where

| Path | What it holds |
|---|---|
| `index.html` | The whole site: design, layout and the code that shows the content |
| `content.json` | About text, footer links, the list of notes, and quotes |
| `notes/*.md` | One file per note, written in simple Markdown |
| `images/` | Pictures used in notes |

## Editing (all of it can be done on github.com, no code)

**About page:** edit `"about"` in `content.json`. Keep line breaks as `\n`; a blank line between paragraphs is `\n\n`.

**Footer links:** edit `"links"` in `content.json`. A link with an empty `"url"` is hidden (Google Scholar is waiting for
its link).

**Add a note:**
1. Create `notes/your-note-name.md` and write the note.
2. Add an entry to `"notes"` in `content.json`:
   ```json
   { "id": "your-note-name", "title": "Your Note Title", "date": "2026-12-01", "file": "notes/your-note-name.md" }
   ```
3. Put any pictures in `images/`.

**Writing a note (Markdown):**
- Leave a blank line between paragraphs.
- `## Heading`
- `**bold**`, `*italic*`
- `[link text](https://...)`
- `> quote`
- `- list item`
- `![caption](../images/picture.png)` on its own line: shows a picture with a caption. The path is relative to
  the note file, so it also displays when you open the note on GitHub.

**Quotes:** edit `"quotes"` in `content.json`. They show in the order listed.

## Previewing on your computer

The page loads its content files, so open it through a small local server rather than double-clicking `index.html`:

```
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Publishing

1. **Put this folder on GitHub.** In GitHub Desktop: File → Add Local Repository → choose this folder → Publish
   repository. Alternatively, create an empty repository on github.com and upload the files.
2. **Connect Hostinger.** In hPanel, open the website for tanzimredwan.com → Advanced → Git.
   - Enter the repository's address (for example `https://github.com/tanzuo017/tanzimredwan.com.git`) and the branch
     `main`.
   - Leave the install directory empty so it deploys into `public_html`, which must be empty first.
   - Click Deploy.
   - A public repository needs nothing else. A private one needs the SSH key Hostinger shows to be added to the
     repository as a deploy key.
3. **Automatic updates.** Hostinger's Git page offers an auto-deployment webhook URL. Add it in the GitHub repository
   under Settings → Webhooks, and every change pushed to GitHub goes live.
4. **HTTPS.** In hPanel, make sure SSL is enabled for the domain.
