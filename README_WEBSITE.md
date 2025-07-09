# Personal Website with Timeline

A modern, responsive personal website featuring a beautiful timeline component and interactive elements.

## Features

### 🎨 Design & UI
- **Modern Design**: Clean, professional layout with smooth animations
- **Responsive**: Works perfectly on desktop, tablet, and mobile devices
- **Dark/Light Themed**: Beautiful gradient hero section with glassmorphism effects
- **Interactive Elements**: Hover effects, smooth transitions, and engaging animations

### 📱 Navigation
- **Fixed Navigation Bar**: Stays at the top with blur effects when scrolling
- **Mobile Menu**: Hamburger menu for mobile devices
- **Smooth Scrolling**: Seamless navigation between sections
- **Active Link Highlighting**: Shows current section in navigation

### ⭐ Timeline Features
- **Interactive Timeline**: Central vertical timeline with alternating content
- **Animated Timeline Items**: Items fade in with staggered animations as you scroll
- **Hover Effects**: Timeline dots scale and glow on hover
- **Technology Tags**: Color-coded tags for each experience/role
- **Responsive Design**: Stacks properly on mobile devices

### 🚀 Interactive Elements
- **Stats Counter**: Animated number counting in the About section
- **Skills Animation**: Skills fade in and scale as you scroll
- **Contact Form**: Functional form with validation and notifications
- **Scroll-to-Top Button**: Appears after scrolling down
- **Typing Animation**: Hero title types out on page load

## File Structure

```
├── index.html          # Main HTML structure
├── styles.css          # Complete CSS styling and responsive design
├── script.js           # JavaScript functionality and animations
└── README_WEBSITE.md   # This documentation file
```

## Getting Started

### 1. Local Development
```bash
# Start a local server (Python 3)
python3 -m http.server 8000

# Or with Python 2
python -m SimpleHTTPServer 8000

# Or with Node.js
npx http-server

# Then open: http://localhost:8000
```

### 2. Deployment
- Upload all files to your web hosting service
- Ensure `index.html` is in the root directory
- No server-side processing required - pure frontend

## Customization Guide

### 📝 Personal Information

#### Update Header & Navigation
```html
<!-- In index.html, line ~12 -->
<title>Your Name - Personal Website</title>

<!-- In index.html, line ~20 -->
<div class="nav-logo">
    <a href="#home">Your Name</a>
</div>
```

#### Update Hero Section
```html
<!-- In index.html, lines ~34-45 -->
<h1 class="hero-title">
    Hi, I'm <span class="highlight">Your Name</span>
</h1>
<p class="hero-subtitle">Your Title/Role</p>
<p class="hero-description">
    Your personal description and what you do...
</p>
```

### 🕒 Timeline Customization

#### Add/Edit Timeline Items
```html
<!-- In index.html, timeline section -->
<div class="timeline-item" data-aos="fade-up">
    <div class="timeline-dot"></div>
    <div class="timeline-content">
        <div class="timeline-date">2024 - Present</div>
        <h3>Your Job Title</h3>
        <h4>Company Name</h4>
        <p>Description of your role and achievements...</p>
        <div class="timeline-tags">
            <span class="tag">Technology 1</span>
            <span class="tag">Technology 2</span>
        </div>
    </div>
</div>
```

### 🎨 Color Scheme

#### Primary Colors (in styles.css)
```css
/* Blue theme */
--primary-color: #2563eb;
--primary-hover: #1d4ed8;
--accent-color: #fbbf24;

/* Change to your preferred colors */
--primary-color: #your-color;
--primary-hover: #your-hover-color;
--accent-color: #your-accent;
```

#### Background Gradients
```css
/* Hero section gradient */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Timeline line gradient */
background: linear-gradient(to bottom, #2563eb, #7c3aed);
```

### 💼 Skills Section

#### Update Skills Categories
```html
<!-- In index.html, skills section -->
<div class="skill-category">
    <h3>Your Category</h3>
    <div class="skill-items">
        <span class="skill-item">Skill 1</span>
        <span class="skill-item">Skill 2</span>
    </div>
</div>
```

### 📞 Contact Information

#### Update Contact Details
```html
<!-- In index.html, contact section -->
<div class="contact-method">
    <i class="fas fa-envelope"></i>
    <span>your.email@domain.com</span>
</div>
<div class="contact-method">
    <i class="fas fa-phone"></i>
    <span>+1 (555) 123-4567</span>
</div>
```

#### Social Links
```html
<!-- Update href attributes with your profiles -->
<a href="https://linkedin.com/in/yourprofile" class="social-link">
    <i class="fab fa-linkedin"></i>
</a>
<a href="https://github.com/yourusername" class="social-link">
    <i class="fab fa-github"></i>
</a>
```

## Advanced Customization

### 🖼️ Add Profile Image
Replace the icon placeholder with an actual image:
```html
<!-- Replace this -->
<div class="profile-img">
    <i class="fas fa-user"></i>
</div>

<!-- With this -->
<div class="profile-img">
    <img src="your-photo.jpg" alt="Your Name" />
</div>
```

### 📊 Statistics Counter
Update the numbers in the About section:
```html
<div class="stat">
    <h3>100+</h3>
    <p>Your Metric</p>
</div>
```

### 🎭 Animations
Modify animation delays and speeds in `script.js`:
```javascript
// Timeline animation delay
setTimeout(() => {
    item.style.opacity = '1';
    item.style.transform = 'translateY(0)';
}, index * 200); // Change 200 to adjust speed
```

## Browser Support

- ✅ Chrome (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Edge
- ✅ Mobile browsers

## Performance Features

- **Optimized CSS**: Efficient animations and transitions
- **Lazy Loading**: Elements animate only when visible
- **Lightweight**: No heavy frameworks or libraries
- **Fast Loading**: Minimal external dependencies

## External Dependencies

- [Font Awesome 6.0.0](https://fontawesome.com/) - Icons
- [Google Fonts (Inter)](https://fonts.google.com/) - Typography

## Tips for Success

1. **Keep Content Updated**: Regularly update your timeline and skills
2. **Optimize Images**: Compress any images you add
3. **Test Responsiveness**: Check on multiple devices
4. **SEO Friendly**: Update meta tags and descriptions
5. **Fast Hosting**: Use reliable hosting for best performance

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

If you need help customizing the website or encounter any issues, feel free to create an issue or reach out for support.

---

**Happy coding! 🚀**

*Remember to update all placeholder content with your actual information before deploying.*