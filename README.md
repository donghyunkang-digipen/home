# 🎨 Donghyun "Danny" Kang - Portfolio Website

A modern, responsive portfolio website showcasing my academic and personal projects, skills, and experience as a Computer Science student specializing in Real-Time Interactive Simulation.

![Portfolio Preview](https://img.shields.io/badge/Status-Live-success)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)

---

## 🎆 Features

### Visual Effects
- **🎇 Animated Fireworks Background**: Beautiful CSS-based fireworks animation on the hero section
- **🌊 Smooth Scrolling**: Seamless navigation between sections
- **💫 Neumorphic Design**: Modern neumorphism-style mobile navigation menu
- **🎨 Responsive Design**: Optimized for desktop, tablet, and mobile devices

### Navigation
- **Fixed Navigation Bar**: Easy access to all sections
- **Hamburger Menu**: Slide-in mobile menu from the right
- **Smooth Transitions**: All navigation elements have smooth animations

### Content Sections
- **Hero Section**: Eye-catching introduction with animated background
- **About Me**: Professional introduction with photo, education, experience, and skills
- **Student Projects**: Academic projects with detailed modal views
- **Personal Projects**: Personal work showcasing various technologies
- **Contact**: Direct links to email, GitHub, and LinkedIn
- **Resume**: Embedded PDF viewer with download option

### Interactive Elements
- **Project Modals**: Detailed project information in elegant popup modals
- **Coming Soon Alerts**: User-friendly notifications for projects under development
- **Hover Effects**: Subtle animations on buttons and cards
- **Active States**: Visual feedback for all interactive elements

---

## 🛠️ Technologies Used

- **HTML5**: Semantic markup structure
- **CSS3**: 
  - Custom CSS variables for easy theming
  - Flexbox & Grid for layouts
  - CSS animations and transitions
  - Neumorphism design effects
  - Media queries for responsive design
- **JavaScript**: 
  - Vanilla JS for interactions
  - Dynamic modal content generation
  - Event handling for navigation and modals
  - Coming soon feature alerts

---

## 📁 Project Structure

```
portfolio/
│
├── index.html          # Main HTML file
├── style.css           # All styling and animations
├── README.md           # Project documentation
│
├── assets/             # (Optional) Images and resources
│   ├── images/
│   └── resume.pdf
│
└── screenshots/        # (Optional) Portfolio screenshots
```

---

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- (Optional) A local web server for testing

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/donghyunkang-digipen/portfolio.git
   cd portfolio
   ```

2. **Open the website**
   - Simply open `index.html` in your web browser
   - Or use a local server:
     ```bash
     # Using Python
     python -m http.server 8000
     
     # Using Node.js
     npx http-server
     ```

3. **View in browser**
   - Navigate to `http://localhost:8000`

---

## 🎨 Customization

### Colors
Edit the CSS variables in `style.css`:
```css
:root {
    --primary-color: #000000;      /* Primary color */
    --secondary-color: #0aa03c;    /* Secondary color */
    --text-color: #000000;         /* Text color */
    --bg-color: #ffffff;           /* Background color */
}
```

### Adding Projects
Edit the `projectDetails` object in `index.html`:
```javascript
const projectDetails = {
    yourProject: {
        title: "Your Project Title",
        description: "Project description...",
        technologies: ["Tech1", "Tech2"],
        features: ["Feature 1", "Feature 2"],
        challenges: "Challenges you faced...",
        results: "Project outcomes...",
        links: {
            github: "https://github.com/username/repo",
            demo: "https://your-demo-link.com"
        }
    }
};
```

### Resume
Replace `resume.pdf` in the iframe src:
```html
<iframe src="your-resume.pdf" type="application/pdf"></iframe>
```

---

## 📱 Responsive Design

The portfolio is fully responsive and optimized for:
- **Desktop**: Full-featured experience with hover effects
- **Tablet**: Adapted layouts (max-width: 768px)
- **Mobile**: Neumorphic navigation menu, optimized content (max-width: 480px)

---

## 🎆 Special Features

### Fireworks Animation
The hero section features a beautiful CSS-based fireworks animation that adds a celebratory touch to the portfolio. The animation:
- Launches from the bottom of the screen
- Rises smoothly to the top
- Expands in a circular pattern
- Fades gracefully
- Runs continuously with multiple fireworks

### Neumorphic Mobile Menu
The mobile navigation uses a modern neumorphism design:
- Soft shadows creating a 3D effect
- Smooth slide-in animation from the right
- Tactile button press effects
- Clean, minimalist aesthetic

---

## 🤖 Built with Claude AI

This portfolio website was developed with assistance from **Claude AI by Anthropic**. Claude helped with:
- ✨ HTML structure and semantic markup
- 🎨 CSS styling and animations
- 💻 JavaScript functionality
- 🎆 Fireworks animation implementation
- 📱 Responsive design optimization
- 🔧 Bug fixes and refinements

Claude AI provided guidance on best practices, helped troubleshoot issues, and assisted in creating a polished, professional portfolio website.

---

## 📞 Contact

**Donghyun "Danny" Kang**

- 📧 Email: [donghyunkang.dev@gmail.com](mailto:donghyunkang.dev@gmail.com)
- 💻 GitHub: [@donghyunkang-digipen](https://github.com/donghyunkang-digipen)
- 💼 LinkedIn: [kang-dev](https://linkedin.com/in/kang-dev)

---

## 📄 License

This project is open source and available for personal use. Feel free to use it as a template for your own portfolio!

---

## 🙏 Acknowledgments

- **DigiPen Institute of Technology** - For my education in Computer Science RTIS
- **Claude AI by Anthropic** - For development assistance and guidance
- **The Developer Community** - For inspiration and resources

---

## 🔮 Future Enhancements

- [ ] Add more interactive project demos
- [ ] Implement dark mode toggle
- [ ] Add blog section
- [ ] Include project filtering by technology
- [ ] Add loading animations
- [ ] Integrate with GitHub API for dynamic project updates
- [ ] Add testimonials section
- [ ] Implement contact form with backend

---

<div align="center">

**⭐ Star this repo if you found it helpful!**

Made with ❤️ and ☕ by Danny Kang

*Powered by Claude AI*

</div>
