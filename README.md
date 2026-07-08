# Miao Lab Website

Static website for the Miao Lab at Duke University School of Medicine. No build tools or installation required — it's plain HTML, CSS, and JavaScript.

---

## Folder structure

```
miao-lab-website/
├── index.html          ← Home page
├── research.html       ← Research projects
├── people.html         ← Lab members & alumni
├── lab-fun.html        ← Photos and events
├── contact.html        ← Address, email, map
│
├── css/
│   └── style.css       ← All styles (colors, fonts, layout)
│
├── js/
│   └── main.js         ← Navigation behavior only
│
└── img/
    ├── logos/          ← Miao Lab logo
    ├── science/        ← Research figures and hero video
    ├── people/         ← One sub-folder per person
    │   └── Ed/
    │       └── photo.jpg
    └── lab-fun/        ← Gallery photos
```

---

## Run locally in VS Code

1. Install the **Live Server** extension (search "Live Server" in the VS Code Extensions panel and click Install).
2. Open the project folder in VS Code.
3. Right-click `index.html` in the file explorer → **Open with Live Server**.
4. The site opens in your browser and refreshes automatically whenever you save a file.

---

## Common edits

### Add a lab member
1. Create a folder `img/people/[Name]/` and place a `photo.jpg` inside it.
2. Open `people.html` and copy an existing `<div class="people-card">` block.
3. Update the `src`, name, role, and bio fields inside that block.

### Update the PI photo
Replace `img/people/Ed/photo.jpg` with a new file of the same name.

### Add a Lab Fun photo
1. Place your photo in `img/lab-fun/`.
2. Open `lab-fun.html`, find a placeholder `<div class="gallery-item">`, and replace the placeholder `<div class="gallery-photo">` with `<img src="img/lab-fun/yourfile.jpg" alt="...">`.

### Update contact info
Edit `contact.html` directly — find the `<div class="contact-card">` section.

---

## Push changes to GitHub

After making edits, open the Terminal in VS Code (**Terminal → New Terminal**) and run:

```bash
git add .
git commit -m "brief description of what you changed"
git push
```
