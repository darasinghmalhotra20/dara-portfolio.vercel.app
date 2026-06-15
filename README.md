# Professional Resume Portfolio with Loom Integration

A modern, responsive resume portfolio showcasing business analysis expertise with integrated Loom video introduction.

## 📋 Features

- **Professional Design**: Modern, clean layout with gradient header
- **Loom Video Integration**: Embedded video introduction section
- **Responsive Layout**: Fully responsive design for mobile, tablet, and desktop
- **Print-Friendly**: Optimized for printing to PDF
- **Easy to Customize**: Simple template to update with your information
- **SEO Optimized**: Proper semantic HTML structure

## 🚀 Quick Start

### 1. Clone or Download
```bash
git clone https://github.com/darasinghmalhotra20/dara-portfolio.vercel.app.git
```

### 2. Update Your Information

Edit `resume/index.html` and update:
- Your name and title
- Contact information (email, LinkedIn, GitHub)
- Professional summary
- **Loom Video ID** (see section below)
- Work experience
- Skills and competencies
- Education and certifications
- Projects

### 3. Add Your Loom Video

#### Step 1: Create a Loom Video
1. Install [Loom Chrome Extension](https://chromewebstore.google.com/detail/loom-%E2%80%93-screen-recorder-sc/liecbddmkiiihnedobmlmillhodjkdmb)
2. Record your professional introduction (30-60 seconds)
3. Share the video

#### Step 2: Get Your Loom Video ID
1. Open your Loom video
2. Copy the URL: `https://www.loom.com/share/YOUR_LOOM_VIDEO_ID`
3. Extract the `YOUR_LOOM_VIDEO_ID` part

#### Step 3: Update the Resume
Find this line in `resume/index.html`:
```html
<iframe src="https://www.loom.com/embed/YOUR_LOOM_VIDEO_ID" ...
```

Replace `YOUR_LOOM_VIDEO_ID` with your actual video ID.

**Example:**
- Video URL: `https://www.loom.com/share/abc123xyz`
- Video ID: `abc123xyz`
- Update to: `https://www.loom.com/embed/abc123xyz`

### 4. Deploy

#### Option A: Deploy to Vercel (Recommended)
```bash
npm install -g vercel
vercel
```

#### Option B: Deploy to GitHub Pages
1. Push to your `main` branch
2. Enable GitHub Pages in repository settings

#### Option C: Local Testing
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx serve
```

Then visit: `http://localhost:8000/resume/`

## 📁 File Structure

```
.
├── resume/
│   └── index.html          # Main resume page
├── css/
│   ├── style.css           # Global styles
│   └── resume.css          # Resume-specific styles
└── README.md               # This file
```

## 🎨 Customization

### Colors
Edit the color scheme in `css/resume.css`:
```css
/* Primary gradient colors */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

### Font
Modify the font family in `css/style.css`:
```css
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
```

### Content Sections
Add or remove sections by editing `resume/index.html`. Each section follows this structure:
```html
<section class="section">
    <h2>Section Title</h2>
    <!-- Your content -->
</section>
```

## 📱 Responsive Features

- Mobile-first design
- Tablet-optimized layout
- Desktop display optimization
- Print-friendly stylesheet

## 🔗 Links Structure

Make sure to update these links in `resume/index.html`:
```html
<!-- Email -->
<a href="mailto:your-email@example.com">Email</a>

<!-- LinkedIn -->
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>

<!-- GitHub -->
<a href="https://github.com/darasinghmalhotra20">GitHub</a>
```

## 📊 Business Analyst Skills Included

The template includes common BA competencies:
- Requirements Gathering
- Process Mapping
- Gap Analysis
- Jira / Azure DevOps
- SQL / Excel
- Power BI / Tableau
- Agile / Scrum
- And more...

## 💡 Tips

1. **Keep it concise**: Highlight key achievements with quantifiable results
2. **Use action verbs**: "Improved", "Streamlined", "Implemented", "Optimized"
3. **Quantify impact**: Use numbers, percentages, time savings
4. **Video quality**: Ensure good lighting and audio for your Loom video
5. **Regular updates**: Keep your portfolio current with recent projects

## 🎥 Loom Video Ideas

- 30-second introduction of yourself and your expertise
- Quick walkthrough of a notable project
- Your approach to business analysis
- Tech stack you're familiar with
- Career goals and aspirations

## 📄 Print to PDF

1. Open the resume in your browser
2. Press `Ctrl+P` (or `Cmd+P` on Mac)
3. Select "Save as PDF"
4. Choose your layout preferences
5. Download

## 🐛 Troubleshooting

**Loom video not displaying?**
- Verify you have the correct video ID
- Check that the video URL format is correct
- Ensure the video is set to public or shared

**Styling issues?**
- Clear browser cache (Ctrl+Shift+Delete)
- Try a different browser
- Check that CSS files are properly linked

**Deployment issues?**
- Verify file paths are correct
- Ensure `resume/index.html` is accessible
- Check that CSS files are in the `css/` directory

## 📝 Next Steps

1. [ ] Update resume content with your information
2. [ ] Record your Loom video introduction
3. [ ] Add your Loom video ID
4. [ ] Customize colors and fonts
5. [ ] Test on mobile devices
6. [ ] Deploy to production
7. [ ] Share with recruiters and networking contacts

## 📧 Contact

For questions or suggestions, feel free to reach out!

---

**Created with ❤️ for Business Analysts**

Last updated: June 15, 2026
