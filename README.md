# Credits — Marksheet Equivalence Mapping System

An automatic credit management system with marksheet upload and course equivalence mapping for student readmission. This is a fully offline, standalone web application that requires no backend server or external dependencies.

## Features

- **Marksheet Upload**: Upload and parse Excel/CSV marksheet files with student course data
- **Course Equivalence Mapping**: Automatically map courses between different academic systems
- **Automatic Credit Calculation**: Calculate and assign credits based on course mapping rules
- **Offline Operation**: Works completely offline with no internet or backend required
- **Embedded Data Processing**: Built-in JavaScript libraries (SheetJS, pako) for file processing
- **Professional Typography**: Uses IBM Plex Sans/Mono and Playfair Display fonts (embedded)
- **Responsive Design**: Clean, modern interface built with custom CSS

## System Architecture

### Core Components

- **HTML5 Application**: Single-page application with embedded stylesheets and scripts
- **Excel Processing**: Built-in SheetJS library (xlsx.js) for reading Excel/CSV files
- **PDF Support**: Embedded pako library for compressed data handling
- **Font System**: All fonts are embedded as base64 WOFF2 for offline operation
- **Custom Styles**: Professional CSS with custom color scheme (#1d4e89 primary theme)

## Usage

### Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd credits-
```

2. Open in browser:
   - Simply open `index.html` in any modern web browser
   - No installation or build process required

### Workflow

1. **Prepare Data**: Prepare your marksheet in Excel or CSV format with student records
2. **Upload File**: Use the application interface to upload the marksheet file
3. **Configure Mapping**: Set up course equivalence rules for your institution
4. **Generate Report**: The system will automatically calculate credits and generate mappings
5. **Export Results**: Download the processed results as needed

## Technical Details

### Browser Support

- Chrome/Chromium (recommended)
- Firefox
- Safari
- Edge

Requires JavaScript enabled.

### File Formats Supported

- Excel (.xlsx, .xls)
- CSV (.csv)

### Dependencies

All dependencies are embedded directly in the HTML file:

- **SheetJS CE 0.18.5**: Excel/CSV file parsing
- **pako 2.1.0**: Compression/decompression (zlib)
- **CodePage Tables**: Character encoding support (CP437, CP620, CP737, CP850, etc.)

### Data Processing

The application processes marksheet data client-side:
- No data is sent to any server
- All processing happens in the browser
- Results are available for download or further processing

## File Structure

```
credits-/
├── README.md              # This file
├── index.html             # Main application (all-in-one)
├── .git/                  # Git repository
└── .github/               # GitHub configuration
```

## Metadata

- **Theme Color**: #1d4e89 (dark blue)
- **Viewport**: Responsive (width=device-width, initial-scale=1.0)
- **Character Set**: UTF-8

## Security Notes

- All processing is done client-side
- No data is transmitted to external servers
- Safe for handling confidential student data
- Works offline without internet connection

## Development

The application is a single-file HTML application. To modify:

1. Edit `index.html` directly
2. Update styles within the `<style>` tag
3. Modify functionality within the `<script>` tags
4. All fonts and libraries are embedded - no external CDN required

## License

[Add your license information here]

## Support

[Add support/contact information here]

---

**Last Updated**: 2026-07-15
**Version**: 1.0.0