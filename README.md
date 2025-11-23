# Ksar El-Boukhari Province Website

## ولاية قصر البخاري - موقع تفاعلي

A bilingual (Arabic/English) interactive web application showcasing the Ksar El-Boukhari Province in Algeria, featuring administrative information, investment opportunities, and interactive maps.

### Features

- 🗺️ **Interactive Map**: Leaflet-powered map displaying all dairas and municipalities
- 📊 **Statistics Dashboard**: Real-time statistics about population, area, and administrative divisions
- 💼 **Investment Opportunities**: Showcase of key investment sectors and opportunities
- 🏛️ **Administrative Structure**: Complete overview of 6 dairas and their municipalities
- 📱 **Responsive Design**: Mobile-friendly interface that works on all devices
- 🌐 **Bilingual Content**: Arabic (primary) with English translations

### Technologies Used

- HTML5
- CSS3 (Custom CSS Variables, Flexbox, Grid)
- JavaScript (Vanilla JS)
- [Leaflet.js](https://leafletjs.com/) - Interactive maps
- [OpenStreetMap](https://www.openstreetmap.org/) - Map tiles

### Project Structure

```
ksar-el-boukhari-app/
├── index.html          # Main application file (single-page app)
├── README.md           # This file
└── LICENSE            # MIT License
```

### Quick Start

#### Local Development

1. Clone or download this repository
2. Open `index.html` in your web browser
3. No build process or dependencies required!

#### Deploy to GitHub Pages

1. Create a new repository on GitHub
2. Push this code to your repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   git push -u origin main
   ```
3. Go to your repository Settings → Pages
4. Under "Source", select "main" branch
5. Click "Save"
6. Your site will be published at: `https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/`

### Deployment Options

#### GitHub Pages (Recommended)
- Free hosting
- Automatic HTTPS
- Easy updates via Git push
- Custom domain support

#### Other Options
- **Netlify**: Drag & drop deployment
- **Vercel**: Connect GitHub repo for automatic deployments
- **Firebase Hosting**: Google's hosting platform
- **Any static web hosting**: Just upload the files

### Data Structure

The application uses a JSON-like data structure embedded in JavaScript containing:
- 6 Dairas (administrative districts)
- 27 Municipalities with population and area data
- Geographic coordinates for all locations
- 5 Investment opportunity categories

### Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Customization

To modify the data:
1. Open `index.html`
2. Find the `provinceData` object in the JavaScript section
3. Update the information as needed
4. Save and refresh the page

### Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

### License

This project is licensed under the MIT License - see the LICENSE file for details.

### Contact

For questions or suggestions, please open an issue on GitHub.

---

**Live Demo**: [Add your GitHub Pages URL here after deployment]

**Version**: 1.0.0

**Last Updated**: November 2025
