# HEIC Multi-Format Converter

**A privacy-focused, browser-based tool to convert HEIC images to JPG, PNG, PDF, and SVG formats without uploading files to any server.**

## Live Demo

Visit [https://freeheicconvert.com](https://freeheicconvert.com) to use the converter online.

## Features

- **Multi-format conversion**: Convert HEIC files to JPG, PNG, PDF, and SVG
- **Privacy-first approach**: All processing happens locally in your browser
- **No server uploads**: Your files never leave your device
- **Batch processing**: Convert multiple files at once
- **Drag-and-drop interface**: Simple and intuitive user experience
- **File validation**: Ensures proper HEIC format detection
- **Daily usage limits**: Prevents abuse while maintaining availability
- **Responsive design**: Works on desktop and mobile devices

## How It Works

The HEIC Multi-Format Converter uses client-side JavaScript to handle the entire conversion process in the user's browser:

1. Files are selected via drag-and-drop or file picker
2. Format validation checks ensure proper HEIC files
3. The `heic2any` library converts images to the selected format
4. Converted files are previewed in the browser
5. Users can download converted files with a single click

All processing happens on the user's device, with no data ever being sent to a remote server.

## Privacy & Security

This tool is designed with privacy and security in mind:

- **Zero server processing**: All conversion happens locally in the browser
- **No file uploads**: Files are never transmitted over the internet
- **No data storage**: Converted files exist only in temporary browser memory
- **Automatic cleanup**: All data is cleared when the page is closed or refreshed
- **Open source**: Code is fully transparent and available for review

## Technical Details

The converter uses several technologies:

- **heic2any**: Primary library for HEIC conversion
- **jsPDF**: For creating PDF documents
- **Canvas API**: For format conversions between image types
- **HTML5 File API**: For browser-based file handling
- **localStorage**: To manage usage limits

## Installation & Setup

To run the converter locally:

1. Clone this repository
```bash
git clone https://github.com/darkspacelabs/heic-converter.git
cd heic-converter
```

2. Open `index.html` in a modern web browser or serve using a simple HTTP server:
```bash
# Using Python
python -m http.server

# Using Node.js
npx serve
```

3. Navigate to `http://localhost:8000` or the appropriate port

## Deployment

This is a static HTML application with no server-side dependencies, making it easy to deploy anywhere that can serve static files:

- GitHub Pages
- Netlify
- Vercel
- Any traditional web hosting service

## Usage Limits

To prevent abuse and ensure the tool remains available, daily conversion limits are in place:

- 30 conversions per day per browser
- Limits reset after 24 hours
- Limits are enforced client-side using localStorage

## Browser Compatibility

The HEIC Multi-Format Converter works in all modern browsers:

- Chrome (latest 2 versions)
- Firefox (latest 2 versions)
- Safari (latest 2 versions)
- Edge (latest 2 versions)

Internet Explorer is not supported.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## About Dark Space Labs

This free tool is brought to you by [Dark Space Labs](https://darkspacelabs.com), a technology company specializing in web applications, infrastructure, and security solutions.

## Acknowledgments

- The [heic2any](https://github.com/alexcorvi/heic2any) library for HEIC conversion
- [jsPDF](https://github.com/MrRio/jsPDF) for PDF generation
- The open source community for various tools and libraries that made this project possible

---

Built with ❤️ by [Dark Space Labs](https://darkspacelabs.com)
