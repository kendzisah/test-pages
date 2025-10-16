# Icons Folder

This folder is designated for storing icon images used by the PWA manifest.

## Required Icons

The PWA manifest requires the following icon files at the root level:

1. **icon512_maskable.png** - 512x512 maskable icon (JPEG format with .png extension)
   - Purpose: maskable
   - Used for adaptive icons on Android

2. **icon512_rounded.png** - 512x512 rounded icon (PNG format)
   - Purpose: any
   - General purpose icon

## Adding Your Own Icons

To replace the placeholder icons with your own:

1. Create or prepare your icon images at 512x512 pixels
2. Save `icon512_maskable.png` as a JPEG image (despite the .png extension, the manifest specifies type: "image/jpeg")
3. Save `icon512_rounded.png` as a PNG image
4. Place both files in the root directory of the project (not in this icons folder)

## Note

The current implementation places icon files at the root level as specified in the manifest.json. This folder can be used for organizing source images or alternative icon sizes if needed.
