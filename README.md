# Lange Santé Website

A static website for Lange Santé organization.

## File Structure

```
lange_sante_website/
├── index.html          # Home page (About, Leads, Join Us)
├── presentations.html  # Past and future presentations
├── videos.html         # YouTube videos with downloadable slides
├── style.css           # All styling (blue and white theme)
├── images/             # Folder for lead photos and other images
│   └── (add lead photos here)
├── slides/             # Folder for downloadable PowerPoint files
│   └── (add .pptx files here)
└── README.md           # This file
```

## How to Update Content

### 1. Update About Us Text
Open `index.html` and find the `<section class="about">` section. Replace the placeholder text.

### 2. Update Lead Information
In `index.html`, find the `<section class="leads">` section. For each lead:
- Replace "Lead Name 1" with actual name
- Replace "Title / Position" with their role
- Replace the bio text
- Add their photo to the `images/` folder and update the `<img src="...">` path

### 3. Update Contact Email
In `index.html`, find `your-email@example.com` and replace it with your actual email.

### 4. Add Presentations
In `presentations.html`:
- Copy a `<div class="presentation-card">` block
- Update the date, title, presenter, and description
- Future presentations: add to the first section (chronological order)
- Past presentations: add to the second section (reverse chronological - newest first)

### 5. Add Videos
In `videos.html`:
- Find `VIDEO_ID_1`, `VIDEO_ID_2`, etc.
- Replace with your YouTube video ID
  - Example: if your YouTube URL is `https://www.youtube.com/watch?v=abc123`
  - The VIDEO_ID is `abc123`
- Update the video title, date, and description
- Add your PowerPoint file to the `slides/` folder
- Update the download link: `href="slides/your-file-name.pptx"`

## How to Host on GitHub Pages (FREE)

1. Create a GitHub account at https://github.com (if you don't have one)

2. Create a new repository:
   - Click "New repository"
   - Name it `lange-sante` (or any name)
   - Make it Public
   - Click "Create repository"

3. Upload your files:
   - Click "uploading an existing file"
   - Drag all your website files into the upload area
   - Click "Commit changes"

4. Enable GitHub Pages:
   - Go to repository Settings
   - Click "Pages" in the left sidebar
   - Under "Source", select "main" branch
   - Click "Save"

5. Your website will be live at:
   `https://YOUR-USERNAME.github.io/lange-sante/`

## How to Test Locally

Simply double-click `index.html` to open it in your web browser.

## Color Customization

To change colors, edit the CSS variables at the top of `style.css`:

```css
:root {
    --primary-blue: #1a5276;    /* Main blue color */
    --light-blue: #3498db;      /* Accent blue */
    --dark-blue: #0d3347;       /* Footer blue */
    --white: #ffffff;
    --light-gray: #f5f7fa;
    --medium-gray: #e0e5ec;
}
```
