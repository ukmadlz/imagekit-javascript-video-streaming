# HTML5 Video Streaming Demo

A demonstration of native HTML5 video capabilities with JavaScript controls and ImageKit video optimization.

## Features

- **Basic Video** - Simple `<video>` element with native browser controls
- **Poster Thumbnail** - Auto-generated thumbnails using ImageKit's `ik-thumbnail.jpg`
- **Autoplay** - Muted autoplay with `loop` and `playsinline` for iOS compatibility
- **Custom Video Player** - Vanilla JavaScript player with play/pause, progress bar, seek, and volume controls
- **Adaptive Bitrate Streaming** - HLS streaming via Video.js with automatic quality switching
- **ImageKit Transformations** - On-the-fly resizing, format conversion, and text watermarks

## Serving Locally

### Option 1: Python (recommended)

```bash
cd /Users/mike/Development/js-video-imagekit
python3 -m http.server 8000
```

Then open http://localhost:8000

### Option 2: Node.js

```bash
npx serve .
```

### Option 3: PHP

```bash
php -S localhost:8000
```

### Option 4: Open directly

You can open `index.html` directly in a browser, though some features may be limited due to CORS restrictions.

## Files

- `index.html` - Main demo page with all video examples
- `styles.css` - Stylesheet for the demo

## Dependencies

- [Video.js 8.10.0](https://videojs.com/) - Loaded via CDN for adaptive streaming support
- [ImageKit](https://imagekit.io/) - Video hosting and transformation API (uses demo assets)

## Browser Support

The HTML5 `<video>` element is supported in all modern browsers. Video.js provides additional compatibility for HLS/DASH streaming in browsers that don't support these formats natively.
