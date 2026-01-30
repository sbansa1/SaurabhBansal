# Profile Picture Instructions

## Adding Your Profile Picture

To display your profile picture on the HTML resume:

1. **Prepare Your Image:**
   - **Recommended size:** 400x400 pixels (square)
   - **Format:** JPG or PNG
   - **Quality:** High resolution for best results
   - **Aspect ratio:** 1:1 (square) - will be displayed in a circular frame

2. **Upload Your Image:**
   - Name your profile picture file: `profile.jpg` or `profile.png`
   - Place it in this `/assets/images/` directory

3. **Alternative Upload Methods:**

   **Via GitHub Web Interface:**
   - Navigate to this folder on GitHub
   - Click "Add file" → "Upload files"
   - Select your profile picture
   - Commit the change

   **Via Git Command Line:**
   ```bash
   # From your repository root
   git add assets/images/profile.jpg
   git commit -m "Add profile picture"
   git push
   ```

4. **Update HTML (if needed):**
   - The resume.html file is already configured to look for `assets/images/profile.jpg`
   - If you use a different filename, update line 425 in resume.html:
     ```html
     <img src="assets/images/profile.jpg" ...>
     ```

## Image Tips

- **Circular Display:** Your image will be displayed in a circular frame, so center your face in the photo
- **Professional Photo:** Use a professional headshot or business casual photo
- **Good Lighting:** Ensure the photo is well-lit and clear
- **Simple Background:** A plain or professional background works best
- **File Size:** Keep under 500KB for fast loading

## No Image?

Don't worry! If you don't add a profile picture:
- The resume will display a placeholder icon (👤)
- Everything will still work perfectly
- The resume remains professional and ATS-friendly
