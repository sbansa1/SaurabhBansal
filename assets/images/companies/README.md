# Company Logos

## Adding Company Logos to Your Resume

Company logos appear next to each job title in the HTML resume, adding a professional and visual touch.

## How to Add Company Logos

1. **Prepare Your Logos:**
   - **Recommended size:** 100x100px to 200x200px (square)
   - **Format:** PNG with transparent background (preferred) or JPG
   - **Quality:** High resolution, clean company logo
   - **Style:** Official company logo or icon

2. **Name Your Logo Files:**
   
   Use descriptive names matching the company in your resume:
   - `venuiti.png` - Venuiti Solutions Inc.
   - `inferstat.png` - InferStat
   - `mxpertz.png` - Mxpertz Infolabs
   - `rrd.png` - RR Donnelley
   - `isu.png` - Illinois State University

3. **Upload Logos:**

   **Via GitHub Web Interface:**
   - Navigate to `/assets/images/companies/` on GitHub
   - Click "Add file" → "Upload files"
   - Select all your company logo files
   - Commit the changes

   **Via Git Command Line:**
   ```bash
   # From your repository root
   git add assets/images/companies/*.png
   git commit -m "Add company logos"
   git push
   ```

## Where to Find Company Logos

- **Company Websites:** Most companies have a "Press" or "Brand" page with logo downloads
- **LinkedIn:** Company LinkedIn pages often have high-quality logos
- **Google Images:** Search for "[Company Name] logo png transparent"
- **Logo Databases:** sites like brandsoftheworld.com or worldvectorlogo.com

## HTML Configuration

The resume.html file is already configured to look for company logos:
- Venuiti: `assets/images/companies/venuiti.png`
- InferStat: `assets/images/companies/inferstat.png`
- Mxpertz: `assets/images/companies/mxpertz.png`
- RR Donnelley: `assets/images/companies/rrd.png`
- Illinois State: `assets/images/companies/isu.png`

## Fallback Behavior

If a logo file is not found:
- A colored placeholder with the company initial will display instead
- Your resume will still look professional
- The layout remains intact

## Tips for Best Results

- **Consistent Size:** Try to keep all logos similar in dimensions
- **Transparent Background:** PNG files with transparency look most professional
- **High Quality:** Avoid pixelated or low-resolution images
- **Official Logos:** Use official brand logos when possible
- **Square Format:** Logos work best when they're roughly square-shaped
