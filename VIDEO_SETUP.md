# Video/GIF Setup Guide

## Option 1: Google Drive (Recommended for large files)

### Steps:
1. Upload your video/GIF to Google Drive
2. Right-click → Share → Set to "Anyone with the link"
3. Copy the link (format: `https://drive.google.com/file/d/FILE_ID/view`)
4. Extract the FILE_ID from the link
5. Use this format in HTML:

**For Video:**
```html
<video autoplay loop muted playsinline>
  <source src="https://drive.google.com/uc?export=download&id=FILE_ID" type="video/mp4">
</video>
```

**For GIF (as background):**
```css
background-image: url('https://drive.google.com/uc?export=download&id=FILE_ID');
```

## Option 2: YouTube/Vimeo Embed

Upload to YouTube as unlisted and use:
```html
<iframe src="https://www.youtube.com/embed/VIDEO_ID?autoplay=1&mute=1&loop=1&controls=0" 
        style="position:absolute;top:0;left:0;width:100%;height:100%;border:0;"></iframe>
```

## Option 3: Compress the GIF

Use online tools:
- https://ezgif.com/optimize
- https://www.iloveimg.com/compress-image/compress-gif

Target size: Under 5MB for GitHub

## Current Setup

Your `background.gif` is referenced in `index.html` line 13.
Replace with Drive link once you share it!
