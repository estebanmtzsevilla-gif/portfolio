# Portfolio Hosting Instructions

## File Structure
```
/
├── index.html                 # Main portfolio page
├── .htaccess                 # Server configuration
├── HOSTING_INSTRUCTIONS.md   # This file
├── README.md                 # Original documentation
├── assets/
│   ├── css/
│   │   ├── global.css        # Shared styles
│   │   └── case-study.css    # Case study specific styles
│   ├── js/
│   │   └── main.js           # JavaScript functionality
│   └── images/               # Images folder (currently empty)
└── case-studies/
    ├── scaling-design.html
    ├── centeo.html
    ├── crypto-wallet.html
    ├── designing-with-data.html
    ├── lok-hub.html
    ├── website-revamp.html
    └── app-revamp.html
```

## Hosting Setup

### 1. Upload Files to Hostinger
1. Log into your Hostinger control panel
2. Go to File Manager
3. Navigate to the `public_html` folder (or your domain's root folder)
4. Upload all files maintaining the folder structure

### 2. File Permissions
Ensure the following permissions are set:
- Folders: 755
- HTML/CSS/JS files: 644
- .htaccess: 644

### 3. Domain Configuration
- Point your domain to the folder containing `index.html`
- Ensure `index.html` is set as the default index file

## Dependencies

### External Resources
- **Google Fonts**: DM Sans, DM Mono, Lora (loaded from Google CDN)
- **Logo**: Currently references `https://estebanmartinez.site/assets/img/esteban_logo.svg`

### Missing Assets
The following assets are referenced but not included:
- `about-video.mp4` - Video for the about section
- `about-video-fallback.jpg` - Fallback image for the video
- Logo file (currently external)

## Recommendations

### 1. Add Missing Assets
- Download your logo and place it in `assets/images/`
- Update logo references in HTML files to use local path
- Add the about video and fallback image

### 2. Optimize for Production
- Minify CSS and JavaScript files
- Optimize images (WebP format recommended)
- Enable GZIP compression (handled by .htaccess)

### 3. SEO Optimization
- Add meta descriptions to each page
- Add Open Graph tags for social sharing
- Create a sitemap.xml

## Testing
After uploading:
1. Test all internal links work correctly
2. Verify CSS and JavaScript load properly
3. Check responsive design on mobile devices
4. Test case study navigation

## Support
If you encounter any issues:
1. Check browser console for JavaScript errors
2. Verify file paths are correct
3. Ensure all files uploaded with proper permissions
4. Check .htaccess is working (if supported by hosting)