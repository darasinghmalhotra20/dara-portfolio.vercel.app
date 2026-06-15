# Customization Guide

This guide will help you personalize your resume portfolio.

## 📝 Editing Your Content

### 1. Professional Summary

Find this section in `resume/index.html`:

```html
<section class="section">
    <h2>Professional Summary</h2>
    <p>Results-driven Business Analyst with expertise in requirements gathering, process improvement, and stakeholder management. Proven ability to translate business needs into actionable solutions and deliver measurable outcomes.</p>
</section>
```

**Replace with your summary**, keeping it 2-3 sentences focused on:
- Your years of experience
- Key expertise areas
- Your unique value proposition

### 2. Adding Your Loom Video

**Find:**
```html
<iframe src="https://www.loom.com/embed/YOUR_LOOM_VIDEO_ID" ...
```

**Replace `YOUR_LOOM_VIDEO_ID` with your actual ID**

Example: If your Loom URL is `https://www.loom.com/share/a1b2c3d4e5f6g7h8`, your ID is `a1b2c3d4e5f6g7h8`

### 3. Contact Information

Update these links:

```html
<a href="mailto:your-email@example.com">Email</a>
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
<a href="https://github.com/darasinghmalhotra20">GitHub</a>
```

### 4. Work Experience

Find this section:
```html
<div class="experience-item">
    <div class="experience-header">
        <h3>Business Analyst</h3>
        <span class="date">YYYY - Present</span>
    </div>
    <p class="company">Company Name</p>
    <ul class="achievements">
        <li>Achievement 1: Description of impact and results</li>
        <li>Achievement 2: Description of impact and results</li>
        <li>Achievement 3: Description of impact and results</li>
    </ul>
</div>
```

**Update:**
- `Business Analyst` → Your job title
- `YYYY - Present` → Your employment dates
- `Company Name` → Your company name
- Achievements → Your actual accomplishments

**Pro tip:** Use metrics and action verbs:
- ✅ "Improved data accuracy by 35% through automated validation processes"
- ✅ "Led requirements gathering for $2M enterprise system implementation"
- ❌ "Worked on business analysis tasks"

### 5. Skills and Competencies

Edit the skills grid section:

```html
<div class="skill-category">
    <h3>Analysis & Planning</h3>
    <ul>
        <li>Requirements Gathering</li>
        <li>Process Mapping</li>
        <li>Gap Analysis</li>
        <li>Feasibility Studies</li>
    </ul>
</div>
```

Replace with your actual skills. You can:
- Add new categories by duplicating the `<div class="skill-category">` block
- Modify skill names
- Remove or add list items

**Suggested skill categories:**
- Analysis & Planning
- Tools & Technologies
- Methodologies
- Business Domain Knowledge
- Soft Skills

### 6. Education

Find and update:
```html
<div class="education-item">
    <h3>Bachelor's Degree in [Your Field]</h3>
    <p class="institution">University Name</p>
</div>
```

**Add certifications:**
```html
<div class="education-item">
    <h3>Certifications</h3>
    <ul>
        <li>IIBA CCBA - International Institute of Business Analysis</li>
        <li>Agile Certified Practitioner - PMI</li>
    </ul>
</div>
```

### 7. Projects

Add your project cards:

```html
<div class="project-card">
    <h3>Project Name</h3>
    <p><strong>Role:</strong> Business Analyst</p>
    <p><strong>Description:</strong> Brief description of the project and your contributions</p>
    <p><strong>Impact:</strong> Quantifiable results and outcomes</p>
</div>
```

**Project template:**
- **Title**: Clear project name
- **Role**: Your specific role
- **Description**: 2-3 sentences about the project and your contribution
- **Impact**: Measurable results (time saved, cost reduction, efficiency gain, etc.)

## 🎨 Design Customization

### Colors

**Edit `css/resume.css`:**

Find the gradient (line ~3):
```css
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
```

Replace with your preferred colors:
- `#667eea` - Primary color
- `#764ba2` - Secondary color

**Color palette ideas:**
- Professional Blue: `#0066cc` to `#0099ff`
- Corporate Green: `#004d00` to `#00a300`
- Modern Purple: `#6c27d9` to `#9333ea`

Find accent colors:
```css
border-left: 4px solid #667eea;  /* Change this color */
color: #667eea;                   /* And here */
```

Replace all instances with your chosen color.

### Fonts

**Edit `css/style.css`:**

```css
font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
```

Change to other Google Fonts:
```css
font-family: 'Roboto', sans-serif;
font-family: 'Poppins', sans-serif;
font-family: 'Inter', sans-serif;
font-family: 'IBM Plex Sans', sans-serif;
```

To use Google Fonts, add to `resume/index.html` in the `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
```

### Spacing and Layout

Adjust margins in CSS files:
```css
margin-bottom: 40px;  /* Larger gaps between sections */
padding: 30px;        /* Inner spacing */
gap: 20px;            /* Grid spacing */
```

## 📱 Responsive Testing

Test your resume at different screen sizes:

**Browser DevTools:**
1. Press `F12` (or right-click → Inspect)
2. Click the device toggle (top-left)
3. Select device types to test

**Recommended devices to test:**
- iPhone 12 (390px)
- iPad (768px)
- Desktop (1920px)

## 🔗 Adding Links

### LinkedIn Profile
```html
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
```

Find your LinkedIn URL:
1. Go to linkedin.com
2. Click your profile
3. Copy the URL
4. Use the last part after `linkedin.com/in/`

### GitHub Profile
```html
<a href="https://github.com/yourprofile">GitHub</a>
```

### Email
```html
<a href="mailto:youremail@example.com">Email</a>
```

### Portfolio Website
Add a new link in the contact-info section:
```html
<a href="https://yourportfolio.com">Portfolio</a>
```

## 📄 Print Optimization

To ensure it looks good when printed:

1. Open in browser
2. Press `Ctrl+P` (or `Cmd+P`)
3. Preview:
   - Check that text isn't cut off
   - Verify colors are visible
   - Ensure videos are hidden in print view
4. Save as PDF

**Print CSS is already optimized in `style.css`** - no changes needed!

## ✅ Checklist Before Deployment

- [ ] Updated all personal information
- [ ] Added your Loom video ID
- [ ] Updated all contact links
- [ ] Reviewed work experience descriptions
- [ ] Updated skills and competencies
- [ ] Added your education/certifications
- [ ] Included project examples
- [ ] Customized colors (optional)
- [ ] Tested on mobile devices
- [ ] Tested print-to-PDF functionality
- [ ] Verified all links work
- [ ] Checked spelling and grammar

## 🚀 Ready to Deploy

Once customized, deploy to:
1. **Vercel** (easiest for Vercel projects)
2. **GitHub Pages** (free hosting)
3. **Netlify** (simple drag-and-drop deployment)
4. **Your own server**

---

**Need help?** Check the README.md for more information!
