# Quick Start Guide - Portfolio Customization

Hi Danny! This guide will help you quickly customize your portfolio.

## 🚀 First Steps

### 1. Update Your Basic Info
Open `index.html` and search for these sections:

**Line ~13:** Change the page title
```html
<title>Donghyun "Danny" Kang - Portfolio</title>
```

**Line ~18:** Update navigation logo
```html
<a href="#home" class="logo">Danny Kang</a>
```

**Line ~36:** Update hero section
```html
<h1 class="hero-title">Hi, I'm <span class="highlight">Donghyun "Danny" Kang</span></h1>
<p class="hero-subtitle">Computer Science Student | Developer | Problem Solver</p>
```

### 2. Write Your Introduction
**Line ~54:** Update your about section
```html
<p>
    Hello! I'm Donghyun Kang, but I go by Danny. 
    I'm a [Your Major] student at [Your University], 
    passionate about [Your Interests].
</p>
```

### 3. Update Your Skills
**Line ~65:** Add your actual skills
```html
<span class="tag">Python</span>
<span class="tag">Java</span>
<!-- Add your skills here -->
```

### 4. Update Contact Info
**Line ~188:** Update your email and links
```html
<a href="mailto:your.email@example.com" class="contact-link">
    <span class="icon">✉️</span>
    <span>your.email@example.com</span>
</a>
<a href="https://github.com/yourusername" target="_blank" class="contact-link">
    <span class="icon">💻</span>
    <span>GitHub</span>
</a>
<a href="https://linkedin.com/in/yourusername" target="_blank" class="contact-link">
    <span class="icon">💼</span>
    <span>LinkedIn</span>
</a>
```

## 📂 Adding Projects

### Step 1: Add Project Card in HTML

Find the Academic or Personal Projects section (around line ~95 or ~132) and add:

```html
<div class="project-card" onclick="openModal('myproject1')">
    <div class="project-image">
        <div class="image-placeholder">My Project</div>
    </div>
    <div class="project-info">
        <h3>My Amazing Project</h3>
        <p>A brief one-sentence description of what this project does.</p>
        <div class="project-tags">
            <span class="tag">Python</span>
            <span class="tag">Flask</span>
        </div>
    </div>
</div>
```

**Important:** The ID in `onclick="openModal('myproject1')"` must match the key you use in Step 2!

### Step 2: Add Project Details in JavaScript

Find the `projectDetails` object (around line ~278) and add your project:

```javascript
const projectDetails = {
    // Existing projects...
    
    myproject1: {  // This must match the ID from Step 1!
        title: "My Amazing Project",
        image: "project.jpg",  // Optional: add image filename
        description: "Write a detailed description of your project here. Explain what it does, why you built it, and what problem it solves. Be specific and thorough - this is where you can really showcase your work!",
        technologies: ["Python", "Flask", "MongoDB", "HTML/CSS"],
        features: [
            "Feature 1: User authentication system with secure password hashing",
            "Feature 2: Real-time data visualization using Chart.js",
            "Feature 3: RESTful API with full CRUD operations"
        ],
        challenges: "Describe the main technical challenges you faced. For example: 'The biggest challenge was implementing real-time updates. I solved this by using WebSockets and optimizing database queries to reduce latency.'",
        results: "Explain what you achieved. For example: 'Successfully deployed to 100+ users, reduced processing time by 50%, learned advanced React hooks.'",
        links: {
            github: "https://github.com/yourusername/project",
            demo: "https://project-demo.com"  // Optional - remove if no demo
        }
    }
};
```

### Example: Complete Project Addition

**In HTML (around line ~95):**
```html
<div class="project-card" onclick="openModal('chatbot')">
    <div class="project-image">
        <div class="image-placeholder">AI Chatbot</div>
    </div>
    <div class="project-info">
        <h3>AI-Powered Chatbot</h3>
        <p>An intelligent chatbot using natural language processing.</p>
        <div class="project-tags">
            <span class="tag">Python</span>
            <span class="tag">TensorFlow</span>
            <span class="tag">NLP</span>
        </div>
    </div>
</div>
```

**In JavaScript (inside projectDetails object, around line ~278):**
```javascript
chatbot: {
    title: "AI-Powered Chatbot",
    image: "chatbot.jpg",
    description: "Built an intelligent chatbot that understands natural language queries and provides relevant responses. The system uses machine learning to improve its responses over time based on user interactions.",
    technologies: ["Python", "TensorFlow", "NLTK", "Flask", "React"],
    features: [
        "Natural Language Understanding using BERT models",
        "Context-aware conversations with memory of previous messages",
        "Multi-language support (English, Spanish, Korean)",
        "Admin dashboard for monitoring conversations and training"
    ],
    challenges: "The main challenge was handling ambiguous queries. I implemented a confidence scoring system that asks clarifying questions when the intent is unclear. I also optimized the model to run efficiently on limited hardware.",
    results: "The chatbot achieved 92% accuracy in intent classification and reduced customer support tickets by 40%. Learned advanced NLP techniques and cloud deployment on AWS.",
    links: {
        github: "https://github.com/dannykang/chatbot",
        demo: "https://chatbot-demo.dannykang.com"
    }
}
```

## 🎨 Quick Color Changes

To change the color theme, edit `style.css` (lines 8-14):

**Purple Theme:**
```css
--primary-color: #7c3aed;
--secondary-color: #5b21b6;
```

**Green Theme:**
```css
--primary-color: #059669;
--secondary-color: #047857;
```

**Red Theme:**
```css
--primary-color: #dc2626;
--secondary-color: #991b1b;
```

## 📸 Adding Images

### Profile Photo
1. Add your photo file (e.g., `profile.jpg`) to the same folder as `index.html`
2. In `index.html` (around line ~76), change:
```html
<div class="about-image">
    <div class="image-placeholder">
        <img src="profile.jpg" alt="Danny Kang">
    </div>
</div>
```

### Project Images
1. Add project image files to your folder
2. In HTML, replace placeholder:
```html
<div class="project-image">
    <img src="myproject.jpg" alt="My Project">
</div>
```

3. In JavaScript projectDetails, update:
```javascript
image: "myproject.jpg",
```

4. In JavaScript (around line ~367), uncomment the image line:
```javascript
// Change this:
<!-- Uncomment when you have images: <img src="${project.image}" alt="${project.title}"> -->

// To this:
<img src="${project.image}" alt="${project.title}">
```

## 📄 Adding Your Resume

The resume section now shows a preview of your PDF!

1. **Add your resume PDF file** to the folder (name it exactly `resume.pdf`)
2. The preview will automatically appear on desktop
3. On mobile, it will show a download button (since mobile browsers don't always support PDF previews)

**To use a different filename:**
Update both places in `index.html` (around line ~210):
```html
<!-- Change both lines -->
<iframe src="your-resume-name.pdf" type="application/pdf"></iframe>
<!-- AND -->
<a href="your-resume-name.pdf" class="btn btn-primary" download>
```

**Important Notes:**
- The PDF file must be in the same folder as `index.html`
- File name is case-sensitive: `Resume.pdf` ≠ `resume.pdf`
- Desktop users will see a preview before downloading
- Mobile users will see a "download" message (this is normal - mobile browsers don't always show PDF previews)

## ✅ Checklist Before Publishing

- [ ] Updated all personal information (name, email, links)
- [ ] Written your introduction in About section
- [ ] Added your skills
- [ ] Added at least 2 academic projects
- [ ] Added at least 2 personal projects
- [ ] Each project has complete details in JavaScript
- [ ] Updated contact information
- [ ] Added resume PDF
- [ ] Tested on mobile (use browser dev tools)
- [ ] Tested project modals (click each project)

## 🆘 Common Issues

**Problem:** Modal doesn't open when I click a project  
**Solution:** Make sure the ID in `onclick="openModal('ID')"` exactly matches the key in `projectDetails`

**Problem:** Project details show undefined  
**Solution:** Check that all required fields exist in your project object (title, description, technologies, features, challenges, results, links)

**Problem:** Images don't show  
**Solution:** Make sure image files are in the same folder as index.html and filenames match exactly (case-sensitive!)

## 🎯 Pro Tips

1. **Write good project descriptions:** Be specific! Instead of "Built a website," write "Built a full-stack e-commerce platform with user authentication, shopping cart, and payment integration using Stripe API."

2. **Quantify your results:** Use numbers when possible. "Reduced load time by 60%" is better than "Made it faster."

3. **Show, don't tell:** Link to live demos and GitHub repos whenever possible.

4. **Keep it updated:** Add new projects as you complete them. Your portfolio should grow with you!

5. **Test everything:** Click every link, open every modal, test on mobile before publishing.

## 🚀 Ready to Publish?

Once you're done customizing:
1. Create a GitHub repository named `yourusername.github.io`
2. Upload `index.html`, `style.css`, and any image files
3. Go to Settings → Pages → Set source to main branch
4. Your site will be live at `https://yourusername.github.io`!

Good luck with your portfolio, Danny! 🎉
