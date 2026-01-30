# Icons Guide

## Icons in the Resume

The resume uses Unicode emoji and symbols for icons throughout the design. This approach:
- ✅ Works without external dependencies
- ✅ Loads instantly (no external files)
- ✅ Prints perfectly
- ✅ Is accessible and universal

## Icons Used in the Resume

### Contact Information (Header)
- ✉️ Email
- 📞 Phone
- 🔗 LinkedIn
- 💻 GitHub

### Section Headers
- 💼 Professional Summary
- 🏢 Professional Experience
- 🛠️ Core Skills
- 🎓 Education
- 🏆 Certifications
- 🏅 Honors & Awards

### Bullet Points
- ▹ Achievement/responsibility bullets (arrow)
- • Skill list bullets (dot)

## Customizing Icons

If you want to change the icons in your resume:

### Option 1: Unicode Emoji (Current Approach)
Simply replace the emoji in the HTML:
```html
<h2 class="section-title">🚀 Professional Summary</h2>
```

Popular emoji options:
- 📊 Charts/Analytics
- 🎯 Goals/Targets
- 🔧 Tools
- 📈 Growth/Progress
- ⚙️ Settings/Configuration
- 💡 Ideas/Innovation
- 🌟 Achievement/Excellence

### Option 2: Font Awesome (External Library)

To use Font Awesome icons instead:

1. Add this to the `<head>` section of resume.html:
```html
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
```

2. Replace emoji with Font Awesome icons:
```html
<!-- Before -->
<h2 class="section-title">💼 Professional Summary</h2>

<!-- After -->
<h2 class="section-title"><i class="fas fa-briefcase"></i> Professional Summary</h2>
```

Popular Font Awesome icons:
- `<i class="fas fa-briefcase"></i>` - Briefcase
- `<i class="fas fa-code"></i>` - Code
- `<i class="fas fa-graduation-cap"></i>` - Education
- `<i class="fas fa-certificate"></i>` - Certificate
- `<i class="fas fa-trophy"></i>` - Trophy
- `<i class="fas fa-envelope"></i>` - Email
- `<i class="fas fa-phone"></i>` - Phone

### Option 3: No Icons

To remove icons entirely, simply delete them from the HTML:
```html
<!-- Before -->
<h2 class="section-title">💼 Professional Summary</h2>

<!-- After -->
<h2 class="section-title">Professional Summary</h2>
```

## Best Practices

1. **Consistency:** Use the same icon style throughout (all emoji OR all Font Awesome)
2. **Print Friendly:** Emoji prints better than some icon fonts
3. **Accessibility:** Emoji are more accessible for screen readers
4. **Simple:** Don't overuse icons - they should enhance, not distract

## Current Setup Benefits

The current Unicode emoji approach:
- Works offline
- No external dependencies
- Faster loading
- Better print quality
- More accessible
- No licensing concerns
