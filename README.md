# Test-image-type PWA

A basic Progressive Web App (PWA) for testing image types in web applications.

## Features

- ✅ Service Worker for offline functionality
- ✅ Web App Manifest for installability
- ✅ Responsive design
- ✅ Custom icons (maskable and rounded)

## Files Structure

```
.
├── index.html              # Main HTML file
├── manifest.json           # PWA manifest with exact specifications
├── sw.js                   # Service Worker for caching
├── icon512_maskable.png    # Maskable icon (512x512)
├── icon512_rounded.png     # Rounded icon (512x512)
└── icons/                  # Folder for additional icons
    └── README.md           # Instructions for adding custom icons
```

## Manifest Configuration

The PWA uses the following manifest configuration:
- **Theme Color:** #8936FF (Purple)
- **Background Color:** #2EC6FE (Cyan)
- **Display Mode:** Standalone
- **Orientation:** Any
- **Language:** en-US
- **Name:** Test-image-type
- **Short Name:** type

## Running the PWA

To test the PWA locally:

1. Start a local web server:
   ```bash
   python3 -m http.server 8080
   ```

2. Open your browser and navigate to:
   ```
   http://localhost:8080
   ```

3. The Service Worker should register automatically, and you'll see the status on the page.

## Customizing Icons

To add your own icons, replace the placeholder images:

1. Create your 512x512 icons
2. Save `icon512_maskable.png` as a JPEG image
3. Save `icon512_rounded.png` as a PNG image
4. Place them in the root directory

See `icons/README.md` for more details.

## Testing PWA Installation

To test the PWA installation:
1. Open the app in Chrome/Edge
2. Look for the install prompt in the address bar
3. Click to install the app
4. The app will run in standalone mode

## Browser Support

This PWA works in all modern browsers that support:
- Service Workers
- Web App Manifest
- Cache API