# Email Signature Generator

A simple, elegant email signature generator that runs entirely in your browser. Create professional email signatures with predetermined company logos, contact information, and easy copy/paste functionality.

## Features

- ✨ **Clean, Modern Interface** - Professional design with live preview
- 🖼️ **Predetermined Logo Library** - Select from pre-configured company logos
- 📋 **One-Click Copy** - Copy signature to clipboard with formatting preserved
- 💾 **Download as HTML** - Save signature as an HTML file
- 🔒 **Privacy-First** - All processing done locally in your browser
- 📱 **Responsive Design** - Works on desktop and mobile devices

## Demo

Try it live: [Your GitHub Pages URL here]

## Usage

### Getting Started

1. Open `index.html` in your web browser
2. Fill in your information:
   - Name (required)
   - Title
   - Company
   - Email (required)
   - Phone
   - Address (street, city, state, ZIP, country)
3. Select a logo from the dropdown (optional)
4. Watch the preview update in real-time
5. Click "Copy Signature" to copy to clipboard
6. Paste into your email client

### Adding Your Company Logos

To add your own logos, edit the `logos` array in the JavaScript section of `index.html`:

```javascript
const logos = [
    {
        id: 1,
        name: 'Company Logo - Blue',
        url: 'logos/company-blue.png'  // Path to your logo file
    },
    {
        id: 2,
        name: 'Company Logo - White',
        url: 'logos/company-white.png'
    }
    // Add more logos as needed
];
```

**Recommended setup:**
1. Create a `logos` folder in your repository
2. Upload your logo image files (PNG, SVG, JPG)
3. Update the `url` field to point to your logo files
4. Update the `name` field with descriptive names

**Logo Guidelines:**
- Use PNG with transparent backgrounds for best results
- Recommended height: 60-80px
- Keep file sizes under 200KB
- SVG format works great for scalable logos

### Installing in Your Email Client

#### Gmail
1. Copy your signature using the "Copy Signature" button
2. Go to Gmail Settings (gear icon → See all settings)
3. Scroll to "Signature" section
4. Create a new signature or edit existing
5. Paste (Ctrl+V or Cmd+V) into the signature editor
6. Click "Save Changes"

#### Outlook (Web)
1. Copy your signature
2. Click Settings (gear icon) → View all Outlook settings
3. Mail → Compose and reply
4. Under "Email signature", paste your signature
5. Click "Save"

#### Apple Mail
1. Download the signature as HTML
2. Open Mail → Preferences → Signatures
3. Create a new signature
4. Open the downloaded HTML file in a browser
5. Select all (Cmd+A) and copy
6. Paste into the signature editor

## Deployment on GitHub Pages

1. Fork or clone this repository
2. Go to repository Settings → Pages
3. Under "Source", select "main" branch
4. Click "Save"
5. Your site will be published at `https://[username].github.io/[repository-name]`

## Customization

### Adding Logos

Edit the `logos` array near the top of the `<script>` section:

```javascript
const logos = [
    {
        id: 1,
        name: 'Primary Logo',
        url: 'logos/primary-logo.png'
    },
    {
        id: 2,
        name: 'Alternative Logo',
        url: 'logos/alt-logo.png'
    }
];
```

### Styling the Signature

The signature style can be customized by editing the HTML template in the `updatePreview()` function. Current styling includes:

- **Name**: 18px, bold, dark blue (#2c3e50)
- **Title**: 14px, purple (#667eea)
- **Company**: 14px, gray (#555)
- **Contact Info**: 13px, light gray (#666)
- **Links**: Purple (#667eea), no underline

## Browser Support

Works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Opera (latest)

## Privacy

All data processing happens locally in your browser. No information is sent to any server. Your contact information remains completely private.

## License

MIT License - feel free to use and modify as needed.

## Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

## Tips

- Create a `logos` folder in your repository for organized logo management
- Use PNG files with transparent backgrounds for best logo appearance
- Keep logos under 200KB for optimal loading
- Test your signature in multiple email clients to ensure compatibility
- Consider creating logos in multiple color variations (light/dark backgrounds)
