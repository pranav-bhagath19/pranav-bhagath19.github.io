# Pranav Sai Bhagath - Portfolio Website

A modern, technical, and professional portfolio website for showcasing AI/ML expertise, projects, and achievements.

## 🎨 Design Features

- **Technical Aesthetic**: Dark theme with electric green accents and animated grid background
- **Distinctive Typography**: Using Syne (display) and JetBrains Mono (monospace) for a unique technical feel
- **Smooth Animations**: Scroll-triggered fade-ins, hover effects, and micro-interactions
- **Fully Responsive**: Mobile-friendly design with hamburger menu
- **Modular Code**: Well-organized CSS with variables for easy customization

## 📁 File Structure

```
portfolio.html          # Main portfolio file (single-page website)
README.md              # This file
```

## 🚀 Quick Start

1. **Open the file**: Simply open `portfolio.html` in any web browser
2. **No build process needed**: This is a static HTML file with inline CSS and JavaScript
3. **Works offline**: No external dependencies except fonts from Google Fonts

## ✏️ How to Modify Content

### 1. Adding New Achievements

Find the `achievements-grid` section (around line 420) and add a new card:

```html
<div class="achievement-card fade-in">
    <div class="achievement-icon">🏆</div>
    <h3 class="achievement-title">Your Achievement Name</h3>
    <p class="achievement-organizer">Organization Name</p>
    <span class="achievement-type">WINNER/RUNNER-UP</span>
</div>
```

### 2. Adding New Projects

Find the `projects-grid` section (around line 550) and add:

```html
<div class="project-card fade-in">
    <div class="project-number">06</div> <!-- Increment number -->
    <div class="project-content">
        <h3>Project Name</h3>
        <p>Project description goes here...</p>
        <div class="project-tech">
            <span class="tech-badge">Technology 1</span>
            <span class="tech-badge">Technology 2</span>
        </div>
        <div class="project-links">
            <a href="YOUR_GITHUB_LINK" class="project-link">View on GitHub →</a>
            <a href="YOUR_DEMO_LINK" class="project-link">Live Demo →</a>
        </div>
    </div>
</div>
```

### 3. Adding New Skills

Find the `skills-container` section (around line 485) and add:

```html
<div class="skill-category fade-in">
    <h3 class="skill-category-title">Category Name</h3>
    <div class="skill-tags">
        <span class="skill-tag">Skill 1</span>
        <span class="skill-tag">Skill 2</span>
        <span class="skill-tag">Skill 3</span>
    </div>
</div>
```

### 4. Adding New Experience

Find the `experience-timeline` section (around line 680) and add:

```html
<div class="experience-item fade-in">
    <div class="experience-header">
        <div>
            <h3 class="experience-title">Job Title</h3>
            <p class="experience-org">Organization Name</p>
        </div>
        <span class="experience-period">2024 - PRESENT</span>
    </div>
    <p class="experience-description">
        Description of your role and responsibilities...
    </p>
</div>
```

### 5. Updating Personal Information

**Hero Section** (around line 350):
- Update name, title, bio in the `hero-content` div
- Modify stats in `hero-stats`

**Contact Section** (around line 730):
- Update email, phone, LinkedIn, GitHub links

**Footer** (around line 800):
- Update social links and copyright year

## 🎨 Customizing Colors

All colors are defined as CSS variables at the top of the `<style>` section (around line 20):

```css
:root {
    --bg-primary: #0a0e17;           /* Main background */
    --bg-secondary: #121821;         /* Card backgrounds */
    --accent-primary: #00ff9f;       /* Primary accent (green) */
    --accent-secondary: #00d4ff;     /* Secondary accent (blue) */
    --text-primary: #e4e4e7;         /* Main text color */
    --text-secondary: #a1a1aa;       /* Secondary text */
}
```

To change the color scheme:
1. Modify these variables to your preferred colors
2. All elements will automatically update

## 📝 Adding Blog Section (Future Feature)

To add a blog section, insert before the contact section:

```html
<section id="blog">
    <div class="section-header fade-in">
        <div class="section-tag">// INSIGHTS & ARTICLES</div>
        <h2 class="section-title">Blog</h2>
        <p class="section-description">Thoughts on AI/ML and technology</p>
    </div>
    
    <div class="projects-grid">
        <!-- Blog posts go here using similar structure to projects -->
    </div>
</section>
```

Don't forget to add "Blog" to the navigation menu.

## 🔧 Technical Details

### Technologies Used
- **HTML5**: Semantic markup
- **CSS3**: Modern features (Grid, Flexbox, Custom Properties, Animations)
- **Vanilla JavaScript**: No frameworks needed
- **Google Fonts**: Syne & JetBrains Mono

### Browser Support
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

### Performance Optimizations
- Inline CSS (no external stylesheet requests)
- Minimal JavaScript
- CSS-only animations
- Optimized font loading with `preconnect`

## 📱 Mobile Responsiveness

The site automatically adapts to mobile screens:
- Hamburger menu for navigation
- Stacked layouts for cards and grids
- Touch-friendly button sizes
- Optimized typography scaling

## 🎯 SEO & Meta Tags

Update the following in the `<head>` section:
- `<title>`: Your name and title
- `<meta name="description">`: Brief description
- Add Open Graph tags for social sharing (optional)

## 📧 Contact Form Integration

The contact form currently shows an alert. To connect to a backend:

1. **Using Formspree** (easiest):
```html
<form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
```

2. **Using Netlify Forms**:
Add `netlify` attribute to form tag

3. **Custom Backend**:
Modify the JavaScript in the contact form event listener

## 🚀 Deployment Options

### GitHub Pages (Free)
1. Create a GitHub repository
2. Upload `portfolio.html` and rename it to `index.html`
3. Enable GitHub Pages in repository settings

### Netlify (Free)
1. Drag and drop the HTML file to netlify.com/drop
2. Get instant deployment

### Vercel (Free)
1. Import repository or upload file
2. Deploy with one click

## 📋 Maintenance Checklist

- [ ] Update projects as you complete them
- [ ] Add new achievements when you win hackathons
- [ ] Keep skills section current with new technologies
- [ ] Update experience when roles change
- [ ] Refresh stats (hackathon wins, projects count)
- [ ] Test on different browsers periodically
- [ ] Check mobile responsiveness after updates

## 💡 Tips for Best Results

1. **Keep it Updated**: Regularly add new projects and achievements
2. **Use High-Quality Content**: Write clear, compelling project descriptions
3. **Add Metrics**: Include quantifiable results in project descriptions
4. **Optimize Images**: If you add images later, compress them for web
5. **Test Forms**: Always test contact form after deployment
6. **Analytics**: Consider adding Google Analytics to track visitors

## 🎓 Learning Resources

To further customize this portfolio:
- [MDN Web Docs](https://developer.mozilla.org/) - HTML/CSS/JS reference
- [CSS-Tricks](https://css-tricks.com/) - CSS techniques
- [Can I Use](https://caniuse.com/) - Browser compatibility

## 📞 Support

If you encounter issues:
1. Check browser console for JavaScript errors
2. Validate HTML at [W3C Validator](https://validator.w3.org/)
3. Test in different browsers
4. Ensure all links are correct

---

**Built with**: Passion for AI/ML and clean code  
**Version**: 1.0  
**Last Updated**: February 2025

Remember: This portfolio represents you. Keep it polished, current, and reflective of your best work! 🚀
