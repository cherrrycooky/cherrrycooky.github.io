# Yongjae Kim academic homepage

This is a minimal GitHub Pages academic website.

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

To add your real photo, upload a file named `profile.jpg` and replace the `photo-placeholder` div in index.html with:

<img class="profile-photo" src="profile.jpg" alt="Yongjae Kim" />

Then add this to styles.css:

.profile-photo {
  width: 210px;
  height: 260px;
  object-fit: cover;
  border: 1px solid var(--line);
}
