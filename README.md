# Asset CDN Repository

This repository serves as a content delivery network (CDN) for static assets including images and videos. Rather than storing assets directly within application repositories, this approach reduces bundle sizes and improves website load times while maintaining flexibility for content updates.

## 🌐 GitHub Pages - this is technically a live site

This repository is deployed as a [GitHub Pages](https://pages.github.com/) site, however we're only using it to store assets. <br>
The Root URL is:
`https://refactor-games.github.io/cdn/`

## 🔗 Usage

All assets are accessible via the root URL followed by the file path:
<br>
`https://refactor-games.github.io/cdn/[path-to-asset]`

### Example
For an image located at `images/about-bg.webp`, the full CDN URL would be:
<br>

https://refactor-games.github.io/cdn/images/about-bg.webp

## 📁 Asset Organization

Assets are organized into directories by type:
- `images/` - Image files (.webp, .jpg, .png)
- `videos/` - Video files (.webm, .mp4)

## 📋 Asset Best Practices

- **Images**: Use `.webp` format over `.jpg` or `.png` for better compression and quality
- **Videos**: Use `.webm` format over `.mp4` for improved web performance

## 🔄 Integration with Refactor Website

In the main [Refactor Website](https://github.com/refactorburbs/refactor-website) repository, assets are referenced in two locations:

### CSS Modules
- [About Section Background Image](https://github.com/refactorburbs/refactor-website/blob/main/components/about/about.module.css)
- [All other Sections Background Image](https://github.com/refactorburbs/refactor-website/blob/main/app/globals.css)  
- [LED Overlay Background Image](https://github.com/refactorburbs/refactor-website/blob/main/components/home/ledOverlay.module.css)

### Constants
- [Website-Facing Asset Links](https://github.com/refactorburbs/refactor-website/blob/main/lib/constants/assets.constants.ts)

## ✏️ Updating Assets

### Method 1: Replace Existing Asset
1. Replace the image file in this CDN repository
2. Ensure the filename and format remain identical
3. No code changes needed in the main website repository

### Method 2: Add New Asset
1. Add the new image or video to the appropriate directory in this CDN repository
2. Update the asset references in the main website repository (CSS Modules or Constants)
