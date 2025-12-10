# Yan He - Personal Homepage (Static Version)

A static HTML/CSS/JavaScript version of the personal homepage, optimized for GitHub Pages deployment.

## 🚀 Features

- **Pure HTML5, CSS3, and JavaScript** - No build process required
- **Matrix Rain Background** - Animated terminal-style background effect
- **Typewriter Effects** - Dynamic text animations
- **Console/Terminal Theme** - Cyberpunk-inspired design
- **Responsive Design** - Works on all devices
- **Smooth Animations** - CSS and JavaScript-powered animations
- **GitHub Pages Ready** - Deploy directly to GitHub Pages

## 📁 Project Structure

```
myhomepage-static/
├── index.html          # Main HTML file
├── styles.css          # All CSS styles
├── script.js           # JavaScript functionality
├── cv.pdf             # CV file (add your own)
└── README.md          # This file
```

## 🌐 Deploying to GitHub Pages

### Method 1: Using GitHub Web Interface

1. **Create a new repository** on GitHub (e.g., `myhomepage`)

2. **Upload files**:
   - Go to your repository
   - Click "Add file" → "Upload files"
   - Drag and drop all files from this directory
   - Commit the changes

3. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click Save

4. **Access your site**:
   - Your site will be available at: `https://YOUR_USERNAME.github.io/myhomepage/`
   - It may take a few minutes to deploy

### Method 2: Using Git Command Line

```bash
# Initialize git repository
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit - Static homepage"

# Add your GitHub repository as remote
git remote add origin https://github.com/YOUR_USERNAME/myhomepage.git

# Push to GitHub
git branch -M main
git push -u origin main
```

Then follow steps 3-4 from Method 1 to enable GitHub Pages.

### Method 3: Using GitHub CLI

```bash
# Install GitHub CLI if not installed
# brew install gh  # macOS
# or download from https://cli.github.com

# Login to GitHub
gh auth login

# Create repository and push
gh repo create myhomepage --public --source=. --remote=origin --push

# Enable GitHub Pages
gh api repos/YOUR_USERNAME/myhomepage/pages -X POST \
  -f source[type]=branch \
  -f source[branch]=main \
  -f source[path]=/
```

## 🔧 Customization

### Update Personal Information

1. **Edit `index.html`**:
   - Search for "Yan He" and replace with your name
   - Update email addresses
   - Update social media links
   - Modify publication entries
   - Update contact information

2. **Update CV**:
   - Replace `cv.pdf` with your own CV file

3. **Customize Colors**:
   - Edit CSS variables in `styles.css`:
   ```css
   :root {
     --background: #0a0a0a;
     --foreground: #00ff00;
     --accent: #00ff41;
     /* ... */
   }
   ```

### Add Your Own CV

1. Place your CV file in the root directory as `cv.pdf`
2. The download button in the publications section will automatically link to it

## 📝 Notes

- **No Build Process**: This is a pure static site - just HTML, CSS, and JavaScript
- **No Dependencies**: All functionality is vanilla JavaScript
- **Icons**: SVG icons are embedded directly in the HTML
- **Fonts**: Uses Google Fonts (Inter and JetBrains Mono) loaded from CDN
- **Compatibility**: Works in all modern browsers

## 🎨 Features Included

- ✅ Matrix rain background animation
- ✅ Typewriter text effects
- ✅ Command cycling in terminal window
- ✅ Smooth scroll navigation
- ✅ Responsive design
- ✅ Console/terminal theme
- ✅ Publication listings
- ✅ Contact section
- ✅ Social media links
- ✅ CV download button

## 🔍 Testing Locally

You can test the site locally before deploying:

```bash
# Using Python 3
python3 -m http.server 8000

# Using Node.js (if you have it)
npx http-server

# Using PHP
php -S localhost:8000
```

Then open `http://localhost:8000` in your browser.

## 📄 License

This project is open source and available for personal use.

## 🤝 Contributing

Feel free to fork this project and customize it for your own use!

## 📧 Contact

For questions or issues, please open an issue on GitHub.

---

**Built with HTML5, CSS3, and JavaScript** | **Deployed on GitHub Pages**

