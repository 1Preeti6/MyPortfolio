# How to edit my portfolio (no tools needed)

My live site: **https://1preeti6.github.io/MyPortfolio/**
The whole site is ONE file: `index.html` (plus `Preeti-Lakhera-Resume.pdf`).
Everything is editable directly on GitHub in the browser. Changes go live automatically in ~1 minute.

---

## ✅ The golden rule
From now on, **always edit my OWN repo**, not anyone else's:
👉 https://github.com/1Preeti6/MyPortfolio

(Make sure I'm signed in as **1Preeti6**.)

---

## How to make ANY change (the only workflow I need)

1. Go to https://github.com/1Preeti6/MyPortfolio
2. Click on **`index.html`**
3. Click the **pencil icon** (✏️ "Edit this file") in the top-right of the file.
4. Find the text I want to change (use **Ctrl/Cmd + F** to search inside the editor).
5. Type my change.
6. Scroll to the bottom → green **"Commit changes"** button → **Commit changes** again in the popup.
7. Wait ~1 minute, then refresh https://1preeti6.github.io/MyPortfolio/ — done. ✅

That's it. Every edit = open file → pencil → change → Commit.

---

## Where things live inside index.html
Use Ctrl/Cmd + F to jump to these markers:

| I want to change... | Search for this text |
|---|---|
| My intro / tagline | `Building` (the hero heading) |
| The "about me" paragraphs | `Who I am` |
| The quick-facts box (status, base, CGPA…) | `class="stat-card"` |
| My skills / tools | `Tools I work with` |
| A project | `Selected projects` |
| Work experience / education | `Experience &amp; education` |
| Certifications | `Certifications` |
| Contact links (email, LinkedIn, GitHub, phone) | `class="contact-links"` |

---

## Common edits — copy the pattern that's already there

### Change a piece of text
Just find it and type over it. E.g. to change my phone, search `7701887037` and edit it.

### Add a new skill tag
Skill tags look like this:
```html
<span class="tag">Docker</span>
```
Copy one, paste it next to the others, change the word inside.

### Add a new certification (clickable)
Find the certifications block and copy one card like this, then change the link, name, and label:
```html
<a class="cert reveal" href="PUT-BADGE-LINK-HERE" target="_blank" rel="noopener">
  <span class="badge">🏅</span>
  <div><div class="ct-name">Certificate name</div><div class="ct-by">Issued by · view badge ↗</div></div>
</a>
```

### Add a new project
Find `Selected projects` and copy one whole project block (starts with `<a ... class="project reveal">` and ends with `</a>`). Paste it below the last one, then change the number, title, description, link, and tags.

### Update my résumé PDF
1. On https://github.com/1Preeti6/MyPortfolio click **Add file → Upload files**.
2. Upload the new PDF, but **rename it to exactly** `Preeti-Lakhera-Resume.pdf` first (so the download button keeps working).
3. Commit. (If GitHub asks to replace the existing file, say yes.)

### Change a color
At the very top of the file, search `:root`. The colors are listed there (e.g. `--accent: #2ee6c5;`). Change a hex code to restyle the whole site.

---

## If I break something
Every change is saved as a version. To undo:
1. Go to the repo → click **"commits"** (the clock/history icon).
2. Find the last good version → click it → click **"Revert"** (or just re-edit the file to fix it).
Nothing is ever permanently lost.

---

## Backup
A copy of all these files also lives on my laptop at: `/Users/preeti.l/portfolio/`
