# Yongjae Kim academic homepage

This is a minimal GitHub Pages academic website.

## Files to upload

Upload these files to the repository root:

- index.html
- research.html
- teaching.html
- talks.html
- styles.css
- cv.pdf
- .nojekyll

In GitHub Pages settings, use:

- Source: Deploy from a branch
- Branch: main
- Folder: /root

## How to edit text later

You can edit the website directly on GitHub:

1. Open your GitHub repository.
2. Click the file you want to edit, such as `index.html`.
3. Click the pencil icon, "Edit this file".
4. Change only the visible text between HTML tags.
5. Click "Commit changes".
6. Wait for GitHub Pages to redeploy.

Common edits:

- Homepage introduction: edit the paragraph under `<!-- EDIT HOME INTRO HERE -->` in `index.html`.
- ORCID/GitHub links: edit the URLs in the `<p class="links-line">` part of `index.html`.
- Research interests and manuscript status: edit `research.html`.
- Teaching: edit `teaching.html`.
- Talks: edit `talks.html`.
- CV: replace `cv.pdf` with a new PDF using the same filename.

When editing text, keep the surrounding tags such as `<p>`, `<li>`, `<br />`, and `</a>` unless you are comfortable with HTML.

## How to add a Google Scholar link later

In `index.html`, find this part:

```html
<p class="links-line">
  <a href="https://orcid.org/0009-0006-5982-3118" target="_blank" rel="noopener">ORCID</a>
  <span>/</span>
  <a href="https://github.com/cherrrycooky/yongjaekim" target="_blank" rel="noopener">GitHub</a>
</p>
```

Replace it with:

```html
<p class="links-line">
  <a href="YOUR_GOOGLE_SCHOLAR_URL" target="_blank" rel="noopener">Google Scholar</a>
  <span>/</span>
  <a href="https://orcid.org/0009-0006-5982-3118" target="_blank" rel="noopener">ORCID</a>
  <span>/</span>
  <a href="https://github.com/cherrrycooky/yongjaekim" target="_blank" rel="noopener">GitHub</a>
</p>
```

## How to add your real photo

Upload a file named `profile.jpg` and replace this line in `index.html`:

```html
<div class="photo-placeholder">YK</div>
```

with:

```html
<img class="profile-photo" src="profile.jpg" alt="Yongjae Kim" />
```

Then add this to `styles.css`:

```css
.profile-photo {
  width: 210px;
  height: 260px;
  object-fit: cover;
  border: 1px solid var(--line);
}
```
