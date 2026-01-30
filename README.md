# Saurabh Bansal - Professional Resume Generator

A professional, ATS-friendly resume available in both Markdown and HTML formats, with support for profile pictures and company logos.

## 📋 Table of Contents

- [Features](#features)
- [Quick Start](#quick-start)
- [File Structure](#file-structure)
- [Viewing Your Resume](#viewing-your-resume)
- [Customization Guide](#customization-guide)
- [Adding Images](#adding-images)
- [Converting to PDF](#converting-to-pdf)
- [ATS Compatibility](#ats-compatibility)
- [Browser Compatibility](#browser-compatibility)

## ✨ Features

- **📄 Dual Format**: Both Markdown (resume.md) and HTML (resume.html) versions
- **🎯 ATS-Friendly**: Clean, parseable format optimized for Applicant Tracking Systems
- **🖼️ Image Support**: Optional profile picture and company logos
- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile
- **🖨️ Print-Optimized**: Beautiful PDF output from HTML version
- **🎨 Professional Design**: Clean, modern styling with professional color scheme
- **♿ Accessible**: Semantic HTML with proper heading structure
- **⚡ Fast Loading**: No external dependencies (except optional fonts)
- **🔧 Easy to Customize**: Well-documented and easy to update

## 🚀 Quick Start

### Option 1: View Locally

1. **Clone the repository:**
   ```bash
   git clone https://github.com/sbansa1/SaurabhBansal.git
   cd SaurabhBansal
   ```

2. **Open the resume:**
   - **HTML Version:** Open `resume.html` in your web browser
   - **Markdown Version:** Open `resume.md` in any text editor or Markdown viewer

### Option 2: GitHub Pages

1. Enable GitHub Pages in repository settings
2. Select the main branch as source
3. Access your resume at: `https://sbansa1.github.io/SaurabhBansal/resume.html`

## 📁 File Structure

```
SaurabhBansal/
├── resume.md                      # ATS-friendly Markdown resume
├── resume.html                    # Professional HTML resume
├── index.html                     # Portfolio website (separate)
├── style.css                      # Styles for index.html
├── README.md                      # This file
└── assets/
    ├── images/
    │   ├── README.md             # Instructions for profile picture
    │   ├── profile.jpg           # Your profile picture (add this)
    │   └── companies/
    │       ├── README.md         # Instructions for company logos
    │       ├── venuiti.png       # Company logo (add this)
    │       ├── inferstat.png     # Company logo (add this)
    │       ├── mxpertz.png       # Company logo (add this)
    │       ├── rrd.png           # Company logo (add this)
    │       └── isu.png           # Company logo (add this)
    └── icons/
        └── README.md             # Icon usage guide
```

## 👀 Viewing Your Resume

### Markdown Resume (resume.md)

**Best For:**
- ATS (Applicant Tracking Systems)
- Plain text job applications
- GitHub viewing
- Quick text searches

**How to View:**
- **On GitHub:** Navigate to `resume.md` - it will render automatically
- **Locally:** Open in any text editor, VS Code, or Markdown viewer
- **Convert to PDF:** Use tools like Pandoc or Marked 2

### HTML Resume (resume.html)

**Best For:**
- Professional presentation
- PDF generation
- Portfolio websites
- Direct sharing via URL

**How to View:**
- **In Browser:** Double-click `resume.html` or drag it into your browser
- **Live Server:** Use VS Code Live Server extension for live preview
- **GitHub Pages:** Enable GitHub Pages to host online

## 🎨 Customization Guide

### Updating Contact Information

**In resume.md:**
```markdown
- **Email:** [your.email@example.com](mailto:your.email@example.com)
- **Phone:** [123-456-7890](tel:123-456-7890)
```

**In resume.html:**
Find the header section (around line 365) and update:
```html
<a href="mailto:your.email@example.com" class="contact-item">
    ✉️ your.email@example.com
</a>
```

### Adding/Removing Sections

Both files follow a similar structure. To add a section:

**In resume.md:**
```markdown
## 🆕 New Section

Content goes here...
```

**In resume.html:**
```html
<section class="section">
    <h2 class="section-title">🆕 New Section</h2>
    <p>Content goes here...</p>
</section>
```

### Modifying Colors and Styling

Edit the CSS variables in `resume.html` (around line 31):

```css
:root {
    --primary-color: #1e3a8a;      /* Navy blue for headers */
    --secondary-color: #3b82f6;    /* Lighter blue for accents */
    --text-dark: #374151;          /* Dark gray for text */
    --text-light: #6b7280;         /* Light gray for secondary text */
    --bg-white: #ffffff;           /* White background */
    --bg-light: #f9fafb;           /* Light gray background */
    --border-color: #e5e7eb;       /* Border color */
}
```

### Updating Work Experience

To add a new job, copy an existing experience block and update all fields:
- Company logo filename
- Job title
- Company name
- Date range
- Responsibilities and achievements

## 🖼️ Adding Images

### Profile Picture

1. **Prepare your image:**
   - **Size:** 400x400 pixels recommended
   - **Format:** JPG or PNG
   - **Shape:** Square (will be displayed in circular frame)

2. **Add the file:**
   - Save as `assets/images/profile.jpg` or `profile.png`
   - Update filename in HTML if using different name (line 371)

3. **Via GitHub:**
   - Go to `assets/images/` folder
   - Click "Add file" → "Upload files"
   - Upload your image and commit

**See detailed instructions:** [assets/images/README.md](assets/images/README.md)

### Company Logos

1. **Prepare logos:**
   - **Size:** 100x100px to 200x200px recommended
   - **Format:** PNG with transparent background (preferred)
   - **Files needed:**
     - `venuiti.png` - Venuiti Solutions
     - `inferstat.png` - InferStat
     - `mxpertz.png` - Mxpertz Infolabs
     - `rrd.png` - RR Donnelley
     - `isu.png` - Illinois State University

2. **Add files to:** `assets/images/companies/`

3. **Via Git:**
   ```bash
   git add assets/images/companies/*.png
   git commit -m "Add company logos"
   git push
   ```

**See detailed instructions:** [assets/images/companies/README.md](assets/images/companies/README.md)

### No Images? No Problem!

The resume works perfectly without images:
- Profile picture shows a placeholder icon (👤)
- Company logos show colored placeholders with initials
- All functionality remains intact

## 📄 Converting to PDF

### Method 1: Browser Print (Recommended)

**Chrome / Edge (Best Quality):**
1. Open `resume.html` in Chrome or Edge
2. Press `Ctrl+P` (Windows) or `Cmd+P` (Mac)
3. Configure settings:
   - **Destination:** Save as PDF
   - **Layout:** Portrait
   - **Margins:** Default or Minimum
   - **Background graphics:** Enabled (to keep colors)
4. Click "Save"

**Firefox:**
1. Open `resume.html` in Firefox
2. Press `Ctrl+P` or `Cmd+P`
3. Select "Save as PDF"
4. Adjust margins if needed
5. Save

**Safari:**
1. Open `resume.html` in Safari
2. Press `Cmd+P`
3. Click "PDF" dropdown → "Save as PDF"

### Method 2: Command Line Tools

**Using wkhtmltopdf:**
```bash
# Install wkhtmltopdf first
# macOS: brew install wkhtmltopdf
# Ubuntu: sudo apt-get install wkhtmltopdf

wkhtmltopdf resume.html Saurabh_Bansal_Resume.pdf
```

**Using Puppeteer (Node.js):**
```bash
# Install Puppeteer
npm install -g puppeteer

# Convert to PDF
node -e "const puppeteer = require('puppeteer'); (async () => { const browser = await puppeteer.launch(); const page = await browser.newPage(); await page.goto('file://${PWD}/resume.html', {waitUntil: 'networkidle0'}); await page.pdf({path: 'resume.pdf', format: 'Letter', printBackground: true}); await browser.close(); })();"
```

### Method 3: Online Tools

- **CloudConvert:** https://cloudconvert.com/html-to-pdf
- **HTML to PDF:** https://www.html2pdf.com/
- Upload `resume.html` and download PDF

### Tips for Best PDF Results

1. **Enable background graphics** in print settings (keeps colors)
2. **Use minimum margins** for more content per page
3. **Portrait orientation** works best for resumes
4. **Letter or A4 size** depending on your region
5. **Print preview** before saving to check layout

## 🤖 ATS Compatibility

### Why ATS Matters

Applicant Tracking Systems (ATS) parse resumes to extract information. Many ATS systems struggle with complex layouts.

### Best Practices Implemented

✅ **Use resume.md for ATS submissions** - Plain text is always safest  
✅ **Clean heading hierarchy** - Proper H1, H2, H3 structure  
✅ **Standard section names** - Experience, Education, Skills  
✅ **No tables or complex layouts** - Simple, linear structure  
✅ **Readable fonts** - Standard system fonts used  
✅ **No text in images** - All text is actual text, not images  
✅ **Keywords included** - Technical terms and skills listed  

### Which Format to Use

- **For ATS / Online Applications:** Use `resume.md` or convert it to a simple PDF
- **For Direct Sharing / Portfolio:** Use `resume.html` or its PDF
- **For Email Attachments:** PDF from HTML for best presentation
- **For Recruiter Screening:** PDF from HTML looks most professional

## 🌐 Browser Compatibility

### Fully Supported
- ✅ Chrome/Chromium (version 90+)
- ✅ Firefox (version 88+)
- ✅ Safari (version 14+)
- ✅ Edge (version 90+)
- ✅ Mobile browsers (iOS Safari, Chrome Mobile)

### Print Support
- ✅ Best: Chrome/Edge (most accurate colors and layout)
- ✅ Good: Firefox, Safari
- ⚠️ Avoid: Internet Explorer (not supported)

## 🛠️ Technologies Used

- **HTML5:** Semantic markup for better accessibility and SEO
- **CSS3:** Modern styling with CSS Grid and Flexbox
- **Unicode Emoji:** Icons without external dependencies
- **System Fonts:** Fast loading, professional typography
- **Markdown:** ATS-friendly plain text format

## 📝 Making Updates

### Regular Updates You Might Need

1. **Adding a new job:**
   - Copy an existing experience block
   - Update company info, dates, and responsibilities
   - Add company logo if desired

2. **Adding skills:**
   - Find the skills section
   - Add new bullet points to appropriate categories

3. **Updating contact info:**
   - Update in both resume.md and resume.html
   - Update in index.html if using portfolio site

4. **Adding certifications:**
   - Add to the certifications section
   - Use consistent format with existing entries

### Testing Your Changes

1. **HTML Resume:**
   - Open in browser and verify layout
   - Check print preview (Ctrl+P)
   - Test on mobile (browser dev tools)

2. **Markdown Resume:**
   - Preview on GitHub or in Markdown viewer
   - Ensure formatting is clean
   - Check links work

## 🤝 Contributing

This is a personal resume repository, but feel free to:
- Fork it for your own use
- Suggest improvements via issues
- Share feedback on design/layout

## 📄 License

This resume template is open source and free to use. Just update it with your own information!

## 🙋 Support

If you have questions about using this resume:
1. Check the README files in `/assets/` folders for specific guidance
2. Review the HTML comments in `resume.html` for customization tips
3. Open an issue on GitHub for template-related questions

---

**Created by Saurabh Bansal**  
📧 saurabh.ca007@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/saurabh-bansal-tpm/)  
💻 [GitHub](https://github.com/sbansa1)
