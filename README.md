# RAIN Lab Website

A professional, modern website for the RAIN Lab (Reasoning, AI and NLP) research group.

## 🚀 Quick Start

1. **Open the website**: Simply open `index.html` in your web browser
2. **No build process needed**: This is pure HTML/CSS/JavaScript - works immediately!

## 📁 File Structure

```
RainLAB Website/
├── index.html              # Main website file
├── css/                    # Stylesheets
│   ├── variables.css       # Design system (colors, fonts, spacing)
│   ├── main.css           # Main styles
│   └── responsive.css     # Mobile/tablet styles
├── js/
│   └── main.js            # Interactive features
├── images/
│   ├── team/              # Team member photos (add your photos here)
│   └── news/              # News images (optional)
├── logo/
│   └── rain_lab_logo.jpg  # Lab logo
├── data/                   # JSON files for easy content updates
│   ├── members.json       # Team members
│   ├── publications.json  # Publications
│   ├── news.json          # News items
│   └── alumni.json        # Alumni
└── README.md              # This file
```

## ✏️ How to Update Content

### Adding/Editing Team Members

1. Add team member photos to `images/team/` (recommended size: 600x600px)
2. Edit `data/members.json` and add/modify entries:

```json
{
  "name": "John Doe",
  "role": "Ph.D. Student",
  "category": "phd",
  "photo": "images/team/john-doe.jpg",
  "bio": "John's research focuses on...",
  "links": {
    "website": "https://johndoe.com",
    "scholar": "https://scholar.google.com/...",
    "github": "https://github.com/johndoe"
  }
}
```

**Categories**: `phd`, `masters`, `undergrad`, `postdoc`, `visiting`, `other`

### Adding Publications

Edit `data/publications.json`:

```json
{
  "title": "Your Paper Title",
  "authors": ["Author1", "Author2"],
  "highlightAuthors": ["Author1"],
  "venue": "NeurIPS 2024",
  "venueType": "conference",
  "year": 2024,
  "links": {
    "pdf": "https://arxiv.org/...",
    "code": "https://github.com/...",
    "doi": "https://doi.org/..."
  }
}
```

**Venue types**: `conference`, `journal`, `preprint`, `workshop`

### Adding News Items

Edit `data/news.json`:

```json
{
  "date": "2024-09-15",
  "headline": "Paper Accepted to NeurIPS 2024",
  "description": "Brief description here...",
  "link": "https://optional-link.com"
}
```

News items are automatically sorted by date (newest first).

### Adding Alumni

When a team member graduates, move their entry from `members.json` to `alumni.json`:

```json
{
  "name": "Jane Smith",
  "startYear": 2020,
  "endYear": 2023,
  "role": "Ph.D. Student",
  "currentPosition": "Research Scientist at Google DeepMind",
  "link": "https://janesmith.com"
}
```

### Updating Research Leader Info

Edit the Research Leader section directly in `index.html` (lines 88-135):
- Replace placeholder photo path
- Update name, title, credentials
- Modify research interests tags
- Add your bio paragraphs
- Update contact links

### Updating Footer

Edit the Footer section in `index.html` (lines 201-254):
- Update university affiliation
- Add contact information
- Update social media links

## 🎨 Customizing Design

### Colors

Edit `css/variables.css` to change the color scheme:

```css
--color-sky-blue: #0099FF;
--color-navy: #003366;
```

### Fonts

The site uses **Inter** from Google Fonts. To change, update:
1. The `<link>` tag in `index.html` (line 23)
2. `--font-primary` in `css/variables.css`

### Logo

Replace `logo/rain_lab_logo.jpg` with your logo. The header is now always white, so your logo will display consistently.

## 📱 Features

✅ **Mobile responsive** - Works on all devices
✅ **Smooth scrolling** - Navigation links scroll smoothly to sections
✅ **Active section highlighting** - Current section is highlighted in nav
✅ **Mobile menu** - Hamburger menu on mobile devices
✅ **Dynamic content** - All content loaded from JSON files
✅ **Publication filtering** - Filter publications by year
✅ **Fade-in animations** - Smooth animations as you scroll
✅ **Fast loading** - No framework overhead

## 🌐 Deployment

### Option 1: GitHub Pages (Recommended)

1. Initialize git repository:
   ```bash
   cd "/Users/chadi.helwe/Desktop/RainLAB Website"
   git init
   git add .
   git commit -m "Initial commit"
   ```

2. Create GitHub repository and push:
   ```bash
   git remote add origin https://github.com/yourusername/rainlab-website.git
   git branch -M main
   git push -u origin main
   ```

3. Enable GitHub Pages in repository settings
4. Your site will be live at: `https://yourusername.github.io/rainlab-website`

### Option 2: University Server

Upload all files via FTP/SFTP to your university web server.

### Option 3: Netlify/Vercel

Drag and drop the entire folder to [Netlify](https://netlify.com) or [Vercel](https://vercel.com).

## 🖼️ Image Guidelines

### Team Photos
- **Size**: 600x600px (square)
- **Format**: JPG or PNG
- **File size**: < 200KB (compress with [TinyPNG](https://tinypng.com))

### Research Leader Photo
- **Size**: 800x800px
- **Format**: JPG or PNG
- **File size**: < 300KB

### Logo
- Current logo works great!
- If updating, ensure it works on white background

## 🧪 Testing

Before deploying, test:
- Open `index.html` in different browsers (Chrome, Firefox, Safari)
- Test on mobile devices or use browser DevTools
- Check all links work
- Verify images load correctly

## 🆘 Troubleshooting

**Images not loading?**
- Check file paths in JSON files
- Ensure image files exist in `images/team/`
- File names are case-sensitive on some servers

**Data not showing?**
- Open browser console (F12) to check for errors
- Verify JSON syntax is correct (use [JSONLint](https://jsonlint.com))
- Check file paths to JSON files

**Mobile menu not working?**
- Ensure JavaScript is enabled
- Check browser console for errors

## 📧 Support

For questions or issues, refer to the implementation plan or check the browser console for error messages.

---

**Built with ❤️ for RAIN Lab**
