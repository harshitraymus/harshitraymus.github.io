# Harshit Raymus — Personal Portfolio

A responsive, multi-page academic + music portfolio built with plain HTML, CSS and a little JavaScript. Designed for GitHub Pages.

## Files

- `index.html` — homepage
- `research.html` — research interests, experience and education
- `music.html` — music profile and embed placeholders
- `projects.html` — selected technical and creative projects
- `styles.css` — site-wide design and responsive layout
- `script.js` — mobile navigation and current year
- `assets/` — place images, CV and other files here

## Before publishing: personalize these details

1. In all HTML files, update your name if desired and review every project/experience description for accuracy.
2. In `index.html`, replace `YOUR_EMAIL@example.com` with your preferred public contact email.
3. Replace the LinkedIn and GitHub links with your actual profile URLs.
4. Add a profile photo: put it in `assets/` (for example `profile.jpg`) and replace the `.portrait-placeholder` block in `index.html` with:
   ```html
   <img class="profile-photo" src="assets/profile.jpg" alt="Portrait of Harshit Raymus">
   ```
   Then add this CSS:
   ```css
   .profile-photo { width: 100%; aspect-ratio: 4/5; object-fit: cover; }
   ```
5. Add your latest CV as `assets/Harshit_Raymus_CV.pdf`. We can add a visible download link in the next edit.

## Add music recordings and videos

The Music page currently has two visual placeholders.

### YouTube video
On YouTube, open the video → Share → Embed → copy the iframe code. Replace the first `.embed-placeholder` block in `music.html` with the iframe, e.g.
```html
<iframe
  class="media-embed"
  src="https://www.youtube-nocookie.com/embed/VIDEO_ID"
  title="Live piano or keyboard performance"
  loading="lazy"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
  referrerpolicy="strict-origin-when-cross-origin"
  allowfullscreen></iframe>
```

### SoundCloud audio
On SoundCloud, open the track → Share → Embed → copy the iframe code. Replace the second `.embed-placeholder` block with that iframe. Keep the iframe inside the `.media-card`.

Add this CSS to `styles.css` for either embed:
```css
.media-embed {
  display: block;
  width: 100%;
  aspect-ratio: 16 / 9;
  border: 0;
}
```
For a SoundCloud player, you can use a taller aspect ratio if you prefer.

Only embed audio/video that you own or have permission to share. Unlisted videos may still be accessible to anyone who has the page link.

## Preview locally

You can open `index.html` directly in a browser. For a more reliable local preview, use VS Code with the Live Server extension.

## Publish with GitHub Pages

1. Open your repository: `https://github.com/harshitraymus/harshitraymus.github.io`
2. Choose **Add file → Upload files**.
3. Upload the contents of this folder (the HTML files, CSS, JS, README and `assets` folder). Upload the files themselves to the repository root, not an extra enclosing folder.
4. Commit the changes to the `main` branch.
5. Go to **Settings → Pages**.
6. Under **Build and deployment**, choose **Deploy from a branch**.
7. Select branch `main` and folder `/ (root)`, then Save.
8. Visit `https://harshitraymus.github.io/`. The first deployment can take a few minutes.

## Important privacy note

A GitHub Pages site is public. Do not put private phone numbers, home addresses, confidential lab data, unpublished sensitive research, or anything you do not want publicly accessible in this repository. A public repository's source files are also visible to everyone.
