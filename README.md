# Mohammed Jazar — Portfolio

## Adding your photos

1. Drop new images into `assets/photos/`. Keep file sizes reasonable for
   the web — aim for around 1200px on the long edge, JPEG quality ~80.
   (Full-resolution camera files will make the site slow to load.)
2. Open `index.html` and find the `.gallery` block (search for `id="work"`).
3. Each placeholder tile looks like this:

   ```html
   <div class="tile placeholder">
     <div class="ph-inner"><span class="ph-num">02</span><span>Add photo</span></div>
   </div>
   ```

   Replace it with a real tile:

   ```html
   <div class="tile">
     <img src="assets/photos/your-file.jpg" alt="Short description">
     <div class="tile-caption">Caption or location</div>
   </div>
   ```

4. To make a tile wider or taller, add `wide` or `tall` to the class
   list, e.g. `class="tile wide"`.
5. Duplicate the tile pattern for as many photos as you like — the grid
   reflows automatically, so you can grow past 50 photos without
   touching the CSS.
6. Update the `01 / 50+` counter in the section head once you know
   your real count.

## Adding your portrait

Replace the `.about-media.empty` block in the About section with:
```html
<div class="about-media">
  <img src="assets/photos/portrait.jpg" alt="Mohammed Jazar">
</div>
```

## Things to edit before publishing

- Bio text in the About section (marked with an orange "edit this bio" tag)
- Email and phone number in the Contact section (marked "edit")
- The stats under About (shoots delivered / years shooting)

## Hosting

See the hosting instructions provided in chat. In short: this is a
static site (no build step needed) — the whole folder can be dragged
straight into Netlify, or pushed to GitHub and served with GitHub Pages.
