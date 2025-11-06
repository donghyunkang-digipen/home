# Portfolio Website - Donghyun "Danny" Kang

A clean and modern portfolio website template with interactive project modals.
Built with HTML, CSS, and JavaScript. Easy to deploy on GitHub Pages.

## 🌟 Features

- ✅ Fully Responsive Design (Mobile, Tablet, Desktop)
- ✅ Clean and Modern UI
- ✅ Interactive Project Modals (Click to view details)
- ✅ 5 Main Sections: About, Academic Projects, Personal Projects, Contact, Resume
- ✅ Easy to Customize
- ✅ GitHub Pages Ready
- ✅ Beginner-Friendly Code

## 📁 File Structure

```
portfolio/
├── index.html          # Main HTML file
├── style.css          # CSS styles
└── README.md          # Documentation (this file)
```

## 🚀 Deploy to GitHub Pages

### 1. Create GitHub Repository
1. Log in to GitHub
2. Create a new repository
3. Name it `username.github.io` (replace username with your GitHub username)

### 2. Upload Files
1. Upload `index.html` and `style.css` to the repository
2. Commit and push

### 3. Configure Settings
1. Go to repository Settings
2. Click "Pages" in the left menu
3. Set Source to "main" branch
4. Click Save

### 4. Done!
- Your site will be live at `https://username.github.io` in a few minutes

## ✏️ Customization Guide

### Update Basic Information

#### 1. Personal Information
Edit `index.html` and update:

```html
<!-- Navigation logo -->
<a href="#home" class="logo">Danny Kang</a>

<!-- Hero section -->
<h1 class="hero-title">Hi, I'm <span class="highlight">Donghyun "Danny" Kang</span></h1>
<p class="hero-subtitle">Computer Science Student | Developer | Problem Solver</p>
```

#### 2. About Section
Update your introduction in the About section:

```html
<div class="about-text">
    <h3>Introduction</h3>
    <p>
        Write your introduction here.
        Include your university, major, and interests.
    </p>
</div>
```

#### 3. Skills
Add or remove skill tags:

```html
<div class="skill-tags">
    <span class="tag">Python</span>
    <span class="tag">Java</span>
    <!-- Add more skills -->
</div>
```

#### 4. Adding Projects

**Step 1: Add Project Card**
In the HTML, add a new project card:

```html
<div class="project-card" onclick="openModal('projectId')">
    <div class="project-image">
        <div class="image-placeholder">Project Name</div>
        <!-- Or use image: <img src="project.jpg" alt="Project"> -->
    </div>
    <div class="project-info">
        <h3>Project Title</h3>
        <p>Brief description</p>
        <div class="project-tags">
            <span class="tag">Tech1</span>
            <span class="tag">Tech2</span>
        </div>
    </div>
</div>
```

**Step 2: Add Project Details**
In the JavaScript section, add project details to the `projectDetails` object:

```javascript
const projectDetails = {
    projectId: {
        title: "Your Project Title",
        image: "project.jpg",
        description: "Full detailed description of your project.",
        technologies: ["Python", "Flask", "MongoDB"],
        features: [
            "Feature 1: Description",
            "Feature 2: Description",
            "Feature 3: Description"
        ],
        challenges: "Describe challenges you faced.",
        results: "Explain the results and impact.",
        links: {
            github: "https://github.com/yourusername/project",
            demo: "https://your-demo-link.com"  // Optional
        }
    }
};
```

#### 5. Contact Information
Update your contact links:

```html
<a href="mailto:your.email@example.com" class="contact-link">
    <span class="icon">✉️</span>
    <span>your.email@example.com</span>
</a>
```

#### 6. Resume
Add your resume PDF file to the repository and it will automatically show a preview:

```html
<!-- The filename must match exactly -->
<iframe src="resume.pdf" type="application/pdf"></iframe>
<a href="resume.pdf" class="btn btn-primary" download>
    📥 Download Resume (PDF)
</a>
```

**Note:** Desktop users will see a PDF preview. Mobile users will see a download message (this is normal behavior for mobile browsers).

### Change Colors

Edit colors in `style.css` at the top:

```css
:root {
    --primary-color: #2563eb;      /* Primary color */
    --secondary-color: #1e40af;    /* Secondary color */
    /* ... */
}
```

#### Color Scheme Suggestions:

**1. Blue Theme (Default)**
```css
--primary-color: #2563eb;
--secondary-color: #1e40af;
```

**2. Purple Theme**
```css
--primary-color: #7c3aed;
--secondary-color: #5b21b6;
```

**3. Green Theme**
```css
--primary-color: #059669;
--secondary-color: #047857;
```

**4. Orange Theme**
```css
--primary-color: #ea580c;
--secondary-color: #c2410c;
```

### Adding Images

#### Profile Image
1. Upload image file to repository
2. Update in `index.html`:

```html
<div class="about-image">
    <div class="image-placeholder">
        <img src="profile.jpg" alt="Danny Kang">
    </div>
</div>
```

#### Project Images
```html
<div class="project-image">
    <img src="project1.jpg" alt="Project 1">
</div>
```

For modal images, update in JavaScript:
```javascript
image: "project1.jpg",
```

And uncomment this line in the modal HTML:
```javascript
<!-- Uncomment when you have images: <img src="${project.image}" alt="${project.title}"> -->
```

## 📱 Responsive Design

This template automatically optimizes for:
- 📱 Mobile: 480px and below
- 📱 Tablet: 768px and below
- 💻 Desktop: Above 768px

## 🎨 Modal Functionality

### How It Works
1. Click any project card to open a detailed modal
2. Modal shows:
   - Full project description
   - Technologies used
   - Key features
   - Challenges and solutions
   - Results and impact
   - Links to GitHub and live demo
3. Close modal by:
   - Clicking the X button
   - Clicking outside the modal
   - Pressing Escape key

### Customizing Modal Content
Edit the `projectDetails` object in the JavaScript section to customize what appears in each project's modal.

## 💡 Useful Tips

### 1. Smooth Scrolling
Already implemented! Navigation links scroll smoothly to sections.

### 2. Change Hero Gradient
Edit in `style.css`:

```css
.hero {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    /* Change to your preferred colors */
}
```

### 3. Add Custom Fonts
Add Google Fonts to `<head>` in `index.html`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap" rel="stylesheet">
```

Then in `style.css`:

```css
body {
    font-family: 'Inter', sans-serif;
}
```

### 4. Add More Sections
To add a new section:

```html
<!-- New section example -->
<section id="experience" class="experience">
    <div class="container">
        <h2 class="section-title">Experience</h2>
        <div class="experience-content">
            <!-- Add content here -->
        </div>
    </div>
</section>
```

Add to navigation:
```html
<li><a href="#experience" class="nav-link">Experience</a></li>
```

## 🔧 Troubleshooting

### Q: Mobile menu doesn't close
A: Check that JavaScript is properly loaded. Ensure the `<script>` tag is at the bottom of `index.html`.

### Q: Modal doesn't open
A: Make sure the project ID in `onclick="openModal('projectId')"` matches the key in `projectDetails` object.

### Q: Colors not changing
A: Clear browser cache and hard refresh (Ctrl+F5 or Cmd+Shift+R).

### Q: GitHub Pages not showing
A: Verify filename is exactly `index.html` and repository name is `username.github.io`.

## 📚 Learn More

- [HTML Basics](https://developer.mozilla.org/en-US/docs/Web/HTML)
- [CSS Basics](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [JavaScript Basics](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- [GitHub Pages Documentation](https://pages.github.com/)

## 🤝 Contributing

Found a bug or have suggestions? Feel free to open an issue or submit a pull request!

## 📝 License

This template is free to use for your personal portfolio!

---

Created: 2024  
Build your amazing portfolio! 🚀
This website is generated by Claude AI