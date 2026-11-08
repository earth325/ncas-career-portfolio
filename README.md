# Ethan Wu — NCAS Career Portfolio: Editing Guide

This folder is a clean, plain-HTML version of your portfolio, built from your
current site and adapted to the NCAS Student Challenge requirements.
Due: **November 30, 2026**.

## Files

- `index.html` — the whole portfolio page (all text and sections)
- `styles.css` — how the page looks (colors, fonts, spacing, photo grid)
- `images/` — all 23 photos from your current portfolio, as separate files
  (no more buried base64 blobs). 22 are used on the page; one spare,
  `first-robotics-5-closeup.jpg`, is in the folder ready to use — swap it
  in by changing a `src="images/..."` value.

## How to change text

1. Open `index.html` in any text editor (VS Code, TextEdit, Notepad, or
   GitHub's web editor).
2. Find the words you want to change and edit only the words between the
   tags. Example: to change a paragraph, edit the words inside
   `<p> ... </p>` — leave the `<p>` and `</p>` tags alone.
3. Helpful comments in the file start with `<!-- EDIT: ... -->` and
   `<!-- MOVE: ... -->` — read those first.

## How to move pictures or sections

- **Move a picture:** cut the whole `<figure> ... </figure>` block
  (from `<figure>` to `</figure>`) and paste it where you want it.
- **Reorder the 3 NCAS experiences:** move a whole
  `<section class="experience"> ... </section>` block.
- **Reorder projects:** same idea — move the whole `<article> ... </article>`
  block.

## How to swap a picture

Easiest: replace the file in `images/` with your new picture, using the
**same filename** (e.g. replace `images/coaster-1-navy.jpg`). The page
updates automatically.

Or: put the new file in `images/` and change the `src="images/..."` value
in `index.html` to the new filename. Always update the `alt="..."` text
too, so it describes the new picture.

## How to add a project

Copy a whole `<article> ... </article>` block in the Additional Projects
section, paste it after the last one, and change the heading, text, and
`src` filenames. Do **not** add a 4th experience to the "Experiences and
Projects" section — NCAS allows at most 3 there.

## Rules to keep

- Executive Summary: 250 words or fewer (currently ~197 words).
- Each Experience description: 4 sentences or fewer.
- Each NASA Alignment paragraph: 4 sentences or fewer.
- Technical Skills: 3–10 skills (currently 8).
- Do **not** use the NASA "meatball" or "worm" logo anywhere.
  There is no NASA logo in this site.
- If you add a citation in the text, add a matching numbered entry in
  References and keep the superscript numbers consistent.

## How to publish to GitHub Pages

1. Go to your repo: https://github.com/earth325/portfolio
2. Replace `index.html` with the `index.html` from this folder.
3. Add `styles.css` and the `images/` folder to the repo (same level as
   `index.html`, not inside another folder).
4. Commit. GitHub Pages rebuilds automatically — wait a minute or two,
   then check https://earth325.github.io/portfolio/

Tip: if you use `git` on your computer instead, copy these three things
into your local clone of the repo, then `git add .`, `git commit`, and
`git push`.

## How to export the PDF (must match the website exactly)

1. Open your published site in Chrome (or any browser).
2. File → Print (or Ctrl/Cmd + P).
3. Destination: **Save as PDF**.
4. Save it as: `Ethan Wu - NCAS Student Challenge - Career Portfolio.pdf`
5. Check the PDF: it should contain the same sections, words, and pictures
   as the website.

## What's in the portfolio

1. Executive Summary
2. Technical Skills (8)
3. Experiences and Projects — exactly 3: FIRST Robotics (FRC 2204),
   Launch-Pad, Quad Motor Tester — each with a NASA Alignment paragraph
4. Additional Projects — bartcv, Coaster, Yeti adapter, solar cooker,
   ThinkPad Hackintosh, plus the patent-pending project and FLL teaching
5. Resume (on-page, 1-page section + FlowCV link)
6. References (3 sources, all cited with superscripts)
