# 📦 GitHub Assets Repository

This repository contains various public assets that can be accessed as a CDN through jsDelivr or GitHub Pages.

## 📁 Folder Structure

```
public/
├── html/
│   └── demo/          # HTML demo files and templates
├── svg/
│   ├── map/           # Map-related SVG icons and graphics
│   └── graphic/       # General SVG graphics and illustrations
├── geojson/           # Geographic data in GeoJSON format
└── image/
    └── preview/       # Preview images and thumbnails
```

## 🚀 How to Use

### Via jsDelivr CDN (Recommended)

Use the following URL format to access files:

```
https://cdn.jsdelivr.net/gh/zedfar/assets@VERSION/public/FOLDER/FILE
```

**Usage Examples:**

```html
<!-- HTML Demo File -->
<iframe src="https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/html/demo/example.html"></iframe>

<!-- SVG Map Icon -->
<img src="https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/svg/map/marker.svg" alt="Map Marker">

<!-- SVG Graphic -->
<img src="https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/svg/graphic/logo.svg" alt="Logo">

<!-- Preview Image -->
<img src="https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/image/preview/thumbnail.jpg" alt="Preview">

<!-- GeoJSON in JavaScript -->
<script>
  fetch('https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/geojson/indonesia.geojson')
    .then(response => response.json())
    .then(data => console.log(data));
</script>
```

### Via Raw GitHub (Alternative)

```
https://raw.githubusercontent.com/zedfar/assets/main/public/FOLDER/FILE
```

**Note:** Not recommended for production due to rate limits and limited caching.

## 📝 File Naming Conventions

- Use lowercase for file names
- Separate words with dashes (-): `my-icon.svg`
- Avoid spaces and special characters
- Use descriptive names

**Examples:**
```
✅ user-profile-icon.svg
✅ indonesia-map.geojson
✅ hero-banner.jpg
❌ User Profile Icon.svg
❌ map 1.geojson
```

## 🗂️ Folder Details

### `/public/html/demo`
HTML demo files, templates, and reusable snippets for testing and showcase purposes.

### `/public/svg/map`
Map-related SVG icons such as markers, pins, location indicators, and cartographic symbols.

### `/public/svg/graphic`
General SVG graphics including logos, illustrations, icons, and decorative elements.

### `/public/geojson`
Geographic data in GeoJSON format for mapping and map visualization applications.

### `/public/image/preview`
Preview images, thumbnails, and screenshots for documentation or showcase purposes.

## ⚡ Usage Tips

1. **Use Versioning**: For production, use specific tags/releases instead of `@main`
   ```
   https://cdn.jsdelivr.net/gh/zedfar/assets@v1.0.0/public/svg/map/marker.svg
   ```

2. **Cache Optimization**: jsDelivr will automatically cache your files for better performance

3. **Combined Paths**: You can access files with complete paths including subfolders
   ```
   https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/image/preview/demo-1.jpg
   ```

4. **CORS Friendly**: jsDelivr supports CORS for cross-origin access

5. **Minification**: jsDelivr can automatically minify certain file types by adding `.min` before the extension

## 🔄 Updating Files

After updating files in the repository:
- jsDelivr cache typically updates within 12 hours
- To force update, add query parameters or use a new version
- Or use: `https://purge.jsdelivr.net/` for manual cache purging

## 📊 Monitoring

Track CDN usage through:
- [jsDelivr Stats](https://www.jsdelivr.com/statistics)
- GitHub repository insights
- Network tab in browser DevTools

## 🌐 Live URLs

All files in this repository are publicly accessible via:

**Base CDN URL:**
```
https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/
```

**Quick Access:**
- HTML Demos: `https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/html/demo/`
- Map SVGs: `https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/svg/map/`
- Graphic SVGs: `https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/svg/graphic/`
- GeoJSON: `https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/geojson/`
- Preview Images: `https://cdn.jsdelivr.net/gh/zedfar/assets@main/public/image/preview/`

## 📄 License

MIT © [defazr](https://github.com/zedfar)

## 🤝 Contributing

Contributions are always welcome! Please feel free to submit a Pull Request or create an Issue.

### Guidelines:
1. Follow the folder structure and naming conventions
2. Optimize files before uploading (compress images, minify SVGs)
3. Add descriptive commit messages
4. Test CDN links before submitting PR

---

**Repository:** [github.com/zedfar/assets](https://github.com/zedfar/assets)