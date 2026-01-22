# Davy Jones Portfolio

A professional portfolio website built with vanilla HTML, CSS, and JavaScript to showcase web development projects and skills.

## 🚀 Features

- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Smooth Animations** - Modern scroll animations and transitions
- **Project Filtering** - Filter projects by category (Full Stack, API, Frontend)
- **Contact Form** - Integrated form ready for API connection
- **Mobile Navigation** - Hamburger menu for mobile devices
- **SEO Optimized** - Proper meta tags and semantic HTML
- **Fast Loading** - Optimized for performance

## 📁 Project Structure

```
Jones-Portfolio/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styling
├── js/
│   └── script.js       # JavaScript functionality
├── assets/
│   └── images/         # Project screenshots and images
└── README.md           # This file
```

## 🛠️ Technologies Used

- HTML5
- CSS3 (with CSS Variables)
- Vanilla JavaScript (ES6+)
- Font Awesome Icons

## 📝 Customization Guide

### 1. Update Personal Information

**In `index.html`:**
- Update your name in the hero section
- Change social media links (GitHub, LinkedIn, Email)
- Update contact information
- Add your real project links

### 2. Add Project Screenshots

1. Take screenshots of your projects
2. Save them in `assets/images/` folder
3. Recommended names:
   - `jobconnect.png` - JobConnect SA screenshot
   - `3rdeyevisualz.png` - 3rdEyeVisualz screenshot
   - `notifications-api.png` - Notifications API screenshot

### 3. Update Project Details

**For each project in `index.html`:**
- Update the `<img src>` with actual screenshot path
- Update Live Demo and GitHub links
- Modify project descriptions
- Update technology tags

### 4. Integrate Contact Form with Your API

**In `js/script.js` (around line 125):**

```javascript
// Uncomment and modify this section:
const response = await fetch('YOUR_NOTIFICATIONS_API_ENDPOINT', {
    method: 'POST',
    headers: {
        'Content-Type': 'application/json',
    },
    body: JSON.stringify(formData)
});
```

Replace `'YOUR_NOTIFICATIONS_API_ENDPOINT'` with your actual API URL.

### 5. Customize Colors

**In `css/styles.css` (top of file):**

```css
:root {
    --primary-color: #2563eb;      /* Change to your preferred color */
    --secondary-color: #1e40af;
    --accent-color: #3b82f6;
    /* etc... */
}
```

### 6. Add More Projects

Copy this template and add to the projects grid in `index.html`:

```html
<div class="project-card" data-category="YOUR_CATEGORY">
    <div class="project-image">
        <img src="assets/images/YOUR_IMAGE.png" alt="Project Name">
        <div class="project-overlay">
            <a href="#" class="project-link" target="_blank">
                <i class="fas fa-external-link-alt"></i> Live Demo
            </a>
            <a href="#" class="project-link" target="_blank">
                <i class="fab fa-github"></i> GitHub
            </a>
        </div>
    </div>
    <div class="project-content">
        <h3>Project Name</h3>
        <p>Project description goes here...</p>
        <div class="project-tags">
            <span>Tech1</span>
            <span>Tech2</span>
        </div>
    </div>
</div>
```

## 🌐 Deployment

### Option 1: GitHub Pages (Recommended)

1. Create a new repository on GitHub
2. Push your code:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin YOUR_REPO_URL
git push -u origin main
```
3. Go to Settings → Pages
4. Select branch: `main`, folder: `/ (root)`
5. Your site will be live at `https://yourusername.github.io/Jones-Portfolio`

### Option 2: Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in your project directory
3. Follow the prompts
4. Your site will be deployed instantly

### Option 3: Netlify

1. Drag and drop your folder to [netlify.com/drop](https://app.netlify.com/drop)
2. Your site goes live immediately

## 📱 Testing

Before deploying, test your site:

1. **Desktop** - Open `index.html` in Chrome, Firefox, Safari
2. **Mobile** - Use browser DevTools (F12) → Toggle device toolbar
3. **Links** - Check all navigation and project links work
4. **Form** - Test contact form validation
5. **Responsive** - Test on different screen sizes

## 🎨 Design Notes

- **Color Scheme**: Blue gradient theme (customizable)
- **Typography**: System fonts for fast loading
- **Layout**: CSS Grid and Flexbox for responsiveness
- **Icons**: Font Awesome CDN

## 📚 Learning Resources

As you study this code:
- **CSS Variables** - Lines 1-15 in styles.css
- **Flexbox** - Used in navigation and hero sections
- **CSS Grid** - Used in skills and projects sections
- **Event Listeners** - Throughout script.js
- **DOM Manipulation** - script.js lines 1-50
- **Intersection Observer** - script.js lines 154-166

## 🔄 Next Steps

1. Replace placeholder content with your real information
2. Add actual project screenshots:
   - jobconnect-app.png (for the web app)
   - jobconnect-website.png (for the marketing site)
   - 3rdeyevisualz.png
   - notifications-api.png
3. Test on multiple devices
4. Deploy to GitHub Pages
5. Share the link in job applications!

## 💡 Tips for Job Applications

- Add this project to your GitHub pinned repositories
- Include the live link in your resume
- Mention specific features you built (filtering, animations, etc.)
- Explain how you applied JavaScript fundamentals

## 📞 Support

If you encounter any issues or have questions about customizing this portfolio, refer to the code comments for guidance.

---

**Built with 💙 by Davy Jones**
