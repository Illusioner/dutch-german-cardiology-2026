# The 23rd Dutch-German Joint Meeting - Amsterdam 2026

Complete conference website matching the Heidelberg DGJM style.

## Features
✅ Clean academic design matching Heidelberg conference site
✅ Amsterdam canal image as hero backdrop
✅ Simple, professional typography
✅ Program tables with schedule
✅ Tally form integration for registration & abstracts
✅ Mobile responsive
✅ Ready for GitHub Pages

## Quick Deploy (5 minutes)

### 1. Add Your Image
- Replace `images/hero-amsterdam.jpg` with your Amsterdam canal photo
- Recommended size: 1920x400px (landscape)

### 2. Create Registration Form
Go to https://tally.so (free) and create a form with:
- Name (text, required)
- Email (email, required)
- Affiliation/Institution (text, required)
- Country (dropdown or text)
- Presentation Type (dropdown: Oral / Poster / Attending Only)
- Abstract Title (text, required if presenting)
- **Abstract Body** (long text area, 250-500 words)
- Keywords (text, 3-5 keywords)
- Optional: File upload for PDF

### 3. Update Form Embed
In `index.html`, find this line:
```html
data-tally-src="https://tally.so/embed/YOUR_FORM_ID?..."
```
Replace `YOUR_FORM_ID` with your actual Tally form ID from the embed code.

### 4. Deploy to GitHub Pages
**Option A: Web Upload (Easiest)**
1. Go to https://github.com/new
2. Create repo: `dutch-german-cardiology-2026`
3. Upload all files from this folder
4. Settings → Pages → Deploy from `main` branch
5. Live at: `https://yourusername.github.io/dutch-german-cardiology-2026/`

**Option B: Command Line**
```bash
cd dutch-german-cardiology-2026
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/dutch-german-cardiology-2026.git
git push -u origin main
```
Then enable Pages in Settings.

## File Structure
```
dutch-german-cardiology-2026/
├── index.html              # Main content (edit conference details here)
├── _config.yml             # Jekyll config
├── css/style.css           # Heidelberg-matching styles
├── js/main.js              # Minimal JavaScript
├── images/
│   └── hero-amsterdam.jpg  # YOUR PHOTO GOES HERE
├── _layouts/
│   └── default.html        # Page template
├── Gemfile                 # Jekyll dependencies
└── .gitignore              # Git ignore rules
```

## Customization

### Update Conference Details
Edit `index.html`:
- Change dates, times, session titles
- Update chair names (replace "TBD")
- Modify objectives and theme text
- Update contact information

### Change Colors
Edit `css/style.css`:
- Line 109: `color: #0066cc;` (link color)
- Line 193: `border-left: 4px solid #0066cc;` (accent color)

### Add Logo
Add to `_layouts/default.html` after `<body>` tag:
```html
<div style="text-align: center; padding: 20px;">
    <img src="images/logo.png" alt="Logo" style="max-width: 200px;">
</div>
```

## Export Registrations
From your Tally dashboard:
- View all submissions in real-time
- Export to CSV or Excel
- Integrate with Google Sheets
- Set email notifications

## Support
- Jekyll: https://jekyllrb.com/docs/
- GitHub Pages: https://docs.github.com/pages
- Tally: https://tally.so/help

## License
Free to use and modify for your conference.
