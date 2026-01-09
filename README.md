# Personal Academic Website

A modern, professional personal website for academics and industry professionals.

## 🚀 Quick Start - Publishing on GitHub Pages

### Option 1: Using GitHub Web Interface (Easiest)

1. **Create a new repository on GitHub**
   - Go to https://github.com/new
   - Name it: `your-username.github.io` (replace `your-username` with your actual GitHub username)
   - Make it Public
   - Don't initialize with README
   - Click "Create repository"

2. **Upload your files**
   - Click "uploading an existing file"
   - Drag and drop the `index.html` file
   - Click "Commit changes"

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Under "Source", select "main" branch
   - Click Save

4. **Visit your site**
   - Your site will be live at: `https://your-username.github.io`
   - It may take 1-2 minutes to deploy

### Option 2: Using Git Command Line

```bash
# Clone your repository
git clone https://github.com/your-username/your-username.github.io.git
cd your-username.github.io

# Add your website file
cp /path/to/index.html .

# Commit and push
git add index.html
git commit -m "Initial commit: Add personal website"
git push origin main
```

## 📝 Customization Guide

### Basic Information to Update

1. **Personal Details** (Lines 13-14, 78-81)
   - Replace "Your Name" with your actual name
   - Update the title and tagline

2. **Work Experience** (Lines 132-164)
   - Update job titles and descriptions
   - Adjust dates

3. **Education** (Lines 170-195)
   - Fill in your undergraduate institution
   - Add dissertation title and advisor name
   - Update graduation years

4. **Publications** (Lines 213-245)
   - Add your actual publication titles
   - Include co-authors
   - Add links to papers, code, slides

5. **Contact Information** (Lines 255-260)
   - Update email address
   - Add your LinkedIn, Twitter handles
   - Update any other social media links

6. **Statistics** (Lines 111-123)
   - Adjust publication count (currently 50+)
   - Citations is already set to 4000+

### Color Customization

The color scheme is defined at the top of the CSS (lines 17-23):

```css
:root {
    --primary: #0f1419;      /* Main dark color */
    --accent: #c1540c;       /* Orange accent */
    --accent-light: #e67e22; /* Lighter orange */
    --bg: #fafafa;           /* Background */
    --text: #1a1a1a;         /* Text color */
}
```

To change colors, simply modify these hex values.

### Popular Color Schemes

**Academic Blue:**
```css
--accent: #0066cc;
--accent-light: #3399ff;
```

**Professional Purple:**
```css
--accent: #7c3aed;
--accent-light: #a78bfa;
```

**Modern Green:**
```css
--accent: #059669;
--accent-light: #10b981;
```

## 🔧 Advanced Customization

### Adding New Sections

To add a new section, copy this template:

```html
<section id="your-section-id">
    <h2>Section Title</h2>
    <p style="font-size: 1.1rem; color: var(--text-muted);">
        Your content here
    </p>
</section>
```

Don't forget to add a navigation link in the header:
```html
<a href="#your-section-id">Section Name</a>
```

### Using a Custom Domain

1. Buy a domain (e.g., from Namecheap, Google Domains)
2. In your repository, create a file named `CNAME`
3. Add your domain: `yourdomain.com`
4. In your domain registrar, add these DNS records:
   ```
   Type: A
   Host: @
   Value: 185.199.108.153
   
   Type: A
   Host: @
   Value: 185.199.109.153
   
   Type: A
   Host: @
   Value: 185.199.110.153
   
   Type: A
   Host: @
   Value: 185.199.111.153
   ```

## 📱 Responsive Design

The website is fully responsive and works on:
- Desktop computers
- Tablets
- Mobile phones

## 🛠️ Technical Details

- **Framework**: Pure HTML, CSS, JavaScript (no dependencies)
- **Fonts**: Google Fonts (Crimson Pro, IBM Plex Mono)
- **Animations**: CSS animations with staggered delays
- **Browser Support**: All modern browsers (Chrome, Firefox, Safari, Edge)

## 📄 File Structure

```
your-username.github.io/
├── index.html          # Main website file
├── README.md          # This file
└── CNAME             # (Optional) Custom domain configuration
```

## 🐛 Troubleshooting

**Site not showing up?**
- Wait 1-2 minutes after pushing
- Check Settings → Pages to ensure Pages is enabled
- Verify your repository is named correctly (`username.github.io`)

**Animations not working?**
- Make sure JavaScript is enabled in your browser
- Try clearing your browser cache

**Fonts not loading?**
- Check your internet connection
- The site uses Google Fonts which require internet access

## 📚 Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Markdown Guide](https://www.markdownguide.org/)
- [Google Fonts](https://fonts.google.com/)

## 📧 Support

If you need help customizing your site, feel free to:
1. Open an issue on GitHub
2. Check the comments in the HTML file for guidance
3. Refer to web development resources like MDN Web Docs

---

**Last Updated**: January 2026

**Template Version**: 1.0
