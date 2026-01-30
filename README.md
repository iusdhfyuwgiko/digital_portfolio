# Personal Portfolio Website

A modern, responsive personal portfolio website built with HTML5, CSS3, and vanilla JavaScript. Showcase your work, skills, and experience with a clean, professional design.

## 📁 Project Structure

```
digital_portfolio/
├── index.html          # Main HTML file with all sections
├── styles.css          # Responsive CSS with modern design
├── script.js           # Interactive JavaScript features
├── assets/             # Folder for custom assets (icons, etc.)
├── images/             # Folder for portfolio images
└── README.md           # This file
```

## ✨ Features

- **Responsive Design**: Mobile-first approach with breakpoints at 768px and 1024px
- **Modern Navigation**: Sticky navbar with smooth scroll links and mobile hamburger menu
- **Hero Section**: Eye-catching introduction with call-to-action buttons
- **About Section**: Personal bio, photo placeholder, and statistics
- **Skills Section**: 4-column grid showcasing technical and soft skills
- **Projects Gallery**: 4 project cards with hover effects and overlay links
- **Contact Form**: Functional contact form with validation
- **Social Links**: Footer with social media links
- **Accessibility**: Semantic HTML, ARIA labels, and keyboard navigation
- **Smooth Animations**: Fade-in effects, hover animations, and smooth scrolling
- **Scroll-to-Top Button**: Floating button for easy navigation

## 🎨 Color Scheme

The portfolio uses a modern color palette:

- **Primary Color**: `#6366f1` (Indigo)
- **Secondary Color**: `#06b6d4` (Cyan)
- **Accent Color**: `#ec4899` (Pink)
- **Dark Background**: `#0f172a`
- **Light Background**: `#f8fafc`

You can customize these colors by editing the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #6366f1;
    --secondary-color: #06b6d4;
    --accent-color: #ec4899;
    /* ... other variables ... */
}
```

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code recommended)
- Basic knowledge of HTML, CSS, and JavaScript (optional for customization)

### Installation

1. Open the project folder in your code editor:
   ```bash
   code digital_portfolio
   ```

2. Open `index.html` in your browser using Live Server:
   - Install the "Live Server" extension in VS Code
   - Right-click on `index.html` and select "Open with Live Server"
   - Or simply open the file directly in your browser

## ✏️ Customization Guide

### 1. Update Personal Information

Edit `index.html` and replace:

- `<span class="highlight">Your Name</span>` - Your actual name
- Hero subtitle and description
- About section text
- Contact information (email, phone, location)
- Social media links

### 2. Update Content Sections

#### Navigation Bar
```html
<div class="logo">
    <a href="#home" class="logo-link">YourName</a>
</div>
```

#### Hero Section
```html
<h1 class="hero-title">Hi, I'm <span class="highlight">Your Name</span></h1>
<p class="hero-subtitle">Your Title | Your Specialty</p>
```

#### Skills
Edit the skill categories in the Skills section:
```html
<h3>Your Skill Category</h3>
<ul class="skill-list">
    <li>Skill Name</li>
    <!-- Add more skills -->
</ul>
```

#### Projects
Update project cards with your work:
```html
<h3>Your Project Name</h3>
<p>Project description</p>
<div class="project-tags">
    <span class="tag">Technology</span>
</div>
```

### 3. Add Project Images

Replace the icon placeholders with actual images:

1. Add images to the `images/` folder
2. Replace the `<div class="image-placeholder-project">` with:
   ```html
   <img src="images/project-name.jpg" alt="Project Name" class="project-image">
   ```

3. Update CSS for the image:
   ```css
   .project-image {
       width: 100%;
       height: 250px;
       object-fit: cover;
   }
   ```

### 4. Add Your Profile Photo

1. Add your profile photo to the `images/` folder
2. Replace the icon placeholder in the hero section:
   ```html
   <img src="images/profile.jpg" alt="Your Name" class="profile-photo">
   ```

3. Update the about section image similarly

### 5. Customize Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --primary-color: #your-color;
    --secondary-color: #your-color;
    --accent-color: #your-color;
    /* Update other colors as needed */
}
```

### 6. Modify Typography

Change fonts in `styles.css`:

```css
:root {
    --font-main: 'Your Font', sans-serif;
    --font-heading: 'Your Heading Font', serif;
}
```

### 7. Update Social Media Links

In the contact section, update the social links:

```html
<a href="https://github.com/yourprofile" class="social-link" aria-label="GitHub">
    <i class="fab fa-github"></i>
</a>
```

## 📱 Responsive Breakpoints

- **Mobile**: Below 480px
- **Tablet**: 480px - 768px
- **Desktop**: 768px - 1024px
- **Large Desktop**: 1024px and above

The CSS automatically adjusts layouts and font sizes at these breakpoints.

## 🎯 JavaScript Features

### 1. Mobile Menu Toggle
The hamburger menu automatically appears on screens below 768px and toggles the navigation menu.

### 2. Smooth Scrolling
All internal links use smooth scrolling to navigate between sections.

### 3. Contact Form Validation
The contact form validates:
- All fields are filled
- Email format is correct
- Shows success/error notifications

### 4. Scroll Animations
Elements fade in and slide up when they enter the viewport using Intersection Observer API.

### 5. Active Navigation Indicator
The navbar automatically highlights the current section link as you scroll.

### 6. Scroll-to-Top Button
A floating button appears when you scroll down, allowing quick return to the top.

## 🔧 Advanced Customization

### Add More Sections

To add a new section:

1. Add HTML in `index.html`:
```html
<section id="new-section" class="new-section" aria-labelledby="new-title">
    <div class="container">
        <h2 id="new-title">Section Title</h2>
        <!-- Content here -->
    </div>
</section>
```

2. Add navigation link:
```html
<li><a href="#new-section" class="nav-link">New Section</a></li>
```

3. Add CSS styling in `styles.css`

### Form Integration

To send form emails, integrate with a service like:
- **Formspree**: `https://formspree.io/`
- **EmailJS**: `https://www.emailjs.com/`
- **SendGrid**: `https://sendgrid.com/`

Example with Formspree:
```html
<form action="https://formspree.io/f/your_form_id" method="POST" id="contactForm">
    <!-- form fields -->
</form>
```

### Adding Analytics

Add Google Analytics or similar service:
```html
<!-- In the <head> section -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'GA_ID');
</script>
```

## 📊 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## 🎓 Learning Resources

- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS-Tricks](https://css-tricks.com/)
- [JavaScript.info](https://javascript.info/)
- [Font Awesome Icons](https://fontawesome.com/icons)
- [Google Fonts](https://fonts.google.com/)

## 🐛 Troubleshooting

### Images not displaying
- Check the image path is correct relative to `index.html`
- Verify the image file exists in the `images/` folder
- Use the correct image format (jpg, png, webp, gif)

### Styles not applying
- Clear browser cache (Ctrl+Shift+Delete)
- Check if the `styles.css` file is linked correctly in `index.html`
- Use browser DevTools (F12) to inspect elements

### JavaScript not working
- Check browser console for errors (F12 → Console)
- Verify `script.js` is linked at the bottom of `index.html`
- Ensure elements have correct IDs matching JavaScript selectors

### Mobile menu not closing
- Check if `hamburger` and `navMenu` IDs match in HTML
- Clear browser cache and reload
- Try a different browser

## 📝 License

This project is free to use and modify for personal and commercial purposes.

## 💡 Tips for Success

1. **Keep content concise**: Use clear, scannable text
2. **Use high-quality images**: Optimize images for web (compress, right dimensions)
3. **Add your own projects**: Replace placeholder projects with your actual work
4. **Keep it updated**: Regularly add new projects and skills
5. **Test on mobile**: Always test on real devices or browser DevTools
6. **Add real links**: Update social media and project links to your profiles
7. **Consider SEO**: Add meaningful meta descriptions and alt text
8. **Backup regularly**: Keep a version control system (Git) for your files

## 🚀 Deployment

### Host on GitHub Pages (Free)
1. Create a GitHub repository
2. Push your files to the repository
3. Go to Settings → Pages
4. Select your branch and save
5. Your site will be live at `username.github.io/portfolio`

### Host on Netlify (Free)
1. Visit [netlify.com](https://netlify.com)
2. Connect your GitHub repository
3. Deploy automatically on every push

### Host on Vercel (Free)
1. Visit [vercel.com](https://vercel.com)
2. Import your repository
3. Deploy with zero configuration

## 📧 Contact & Support

For questions or issues, create an issue in your repository or contact the project maintainer.

---

**Happy building! 🎉 Your portfolio is ready to showcase your amazing work!**
