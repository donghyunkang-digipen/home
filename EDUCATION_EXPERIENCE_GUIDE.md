# Education & Experience Section Guide

## 📚 What Was Added

Your About section now includes three subsections:
1. **Introduction** - Your personal intro
2. **Education** - Your academic background
3. **Experience** - Your volunteer work and internships
4. **Skills** - Your technical skills

## 🎓 Education Section

### Current Template:
```html
<div class="education-item">
    <div class="education-header">
        <h5>Your University Name</h5>
        <span class="education-date">Expected Graduation: Month Year</span>
    </div>
    <p class="education-degree">Bachelor of Science in Computer Science</p>
    <p class="education-details">GPA: X.XX/4.0 | Relevant Coursework: Data Structures, Algorithms, Machine Learning</p>
</div>
```

### How to Customize:

**University Name:**
```html
<h5>University of Washington</h5>
```

**Graduation Date:**
```html
<span class="education-date">Expected Graduation: June 2026</span>
<!-- Or if already graduated: -->
<span class="education-date">Graduated: May 2024</span>
```

**Degree:**
```html
<p class="education-degree">Bachelor of Science in Computer Science</p>
<!-- Other examples: -->
<p class="education-degree">Master of Science in Data Science</p>
<p class="education-degree">Bachelor of Arts in Digital Media</p>
```

**Details (GPA, Coursework, Honors):**
```html
<p class="education-details">GPA: 3.85/4.0 | Relevant Coursework: Data Structures, Algorithms, Machine Learning, Computer Graphics</p>
<!-- Or: -->
<p class="education-details">GPA: 3.9/4.0 | Dean's List | President's Scholarship</p>
<!-- Or: -->
<p class="education-details">Relevant Coursework: Web Development, Database Systems, Software Engineering</p>
```

### Adding Multiple Schools:

```html
<!-- First School -->
<div class="education-item">
    <div class="education-header">
        <h5>University of Washington</h5>
        <span class="education-date">Expected Graduation: June 2026</span>
    </div>
    <p class="education-degree">Bachelor of Science in Computer Science</p>
    <p class="education-details">GPA: 3.85/4.0 | Relevant Coursework: Data Structures, Algorithms</p>
</div>

<!-- Second School (if you transferred, did exchange, etc.) -->
<div class="education-item">
    <div class="education-header">
        <h5>Seoul National University</h5>
        <span class="education-date">Fall 2024</span>
    </div>
    <p class="education-degree">Study Abroad Program - Computer Science</p>
    <p class="education-details">AI and Machine Learning specialization</p>
</div>
```

## 💼 Experience Section

### Current Template (SIGGRAPH Example):
```html
<div class="experience-item">
    <div class="experience-header">
        <h5>Student Volunteer</h5>
        <span class="experience-date">2025</span>
    </div>
    <p class="experience-company">SIGGRAPH 2025</p>
    <ul class="experience-details">
        <li>Assisted with conference operations and attendee support</li>
        <li>Collaborated with international team members</li>
        <li>Gained exposure to cutting-edge computer graphics research</li>
    </ul>
</div>
```

### How to Customize SIGGRAPH Experience:

**Date:**
```html
<span class="experience-date">July 2025</span>
<!-- Or more specific: -->
<span class="experience-date">July 28 - August 1, 2025</span>
```

**Your Specific Responsibilities:**
```html
<ul class="experience-details">
    <li>Managed registration desk and assisted 500+ conference attendees</li>
    <li>Coordinated session logistics for technical papers presentations</li>
    <li>Provided translation support for Korean-speaking attendees</li>
    <li>Networked with industry professionals from Pixar, Disney, and NVIDIA</li>
    <li>Attended talks on real-time rendering and AI in graphics</li>
</ul>
```

### Adding More Experiences:

```html
<!-- SIGGRAPH Experience -->
<div class="experience-item">
    <div class="experience-header">
        <h5>Student Volunteer</h5>
        <span class="experience-date">July 2025</span>
    </div>
    <p class="experience-company">SIGGRAPH 2025</p>
    <ul class="experience-details">
        <li>Managed registration and attendee support</li>
        <li>Coordinated technical session logistics</li>
    </ul>
</div>

<!-- Internship -->
<div class="experience-item">
    <div class="experience-header">
        <h5>Software Engineering Intern</h5>
        <span class="experience-date">June - August 2024</span>
    </div>
    <p class="experience-company">Tech Company Name</p>
    <ul class="experience-details">
        <li>Developed new features for mobile app with 100K+ users</li>
        <li>Improved API response time by 40% through optimization</li>
        <li>Collaborated with cross-functional team using Agile methodology</li>
    </ul>
</div>

<!-- Research Position -->
<div class="experience-item">
    <div class="experience-header">
        <h5>Undergraduate Research Assistant</h5>
        <span class="experience-date">January 2024 - Present</span>
    </div>
    <p class="experience-company">University Computer Graphics Lab</p>
    <ul class="experience-details">
        <li>Researching real-time rendering techniques for virtual reality</li>
        <li>Implemented shader optimizations reducing frame time by 25%</li>
        <li>Co-authored paper submitted to SIGGRAPH Asia 2025</li>
    </ul>
</div>

<!-- Teaching Assistant -->
<div class="experience-item">
    <div class="experience-header">
        <h5>Teaching Assistant</h5>
        <span class="experience-date">September 2024 - December 2024</span>
    </div>
    <p class="experience-company">CS 101 - Introduction to Programming</p>
    <ul class="experience-details">
        <li>Led weekly lab sessions for 30 students</li>
        <li>Held office hours and provided one-on-one tutoring</li>
        <li>Graded assignments and provided detailed feedback</li>
    </ul>
</div>
```

## 🎨 Visual Design

The Education and Experience items have a clean card design with:
- White background
- Blue left border (matches your primary color)
- Subtle shadow
- Professional typography
- Responsive layout

### Desktop View:
```
┌────────────────────────────────────┐
│ University Name        [Grad Date] │
│ Bachelor of Science in CS          │
│ GPA: 3.8 | Coursework: ...         │
└────────────────────────────────────┘
```

### Mobile View:
```
┌─────────────────────┐
│ University Name     │
│ [Grad Date]         │
│ Bachelor of CS      │
│ GPA: 3.8 | ...      │
└─────────────────────┘
```

## 💡 Writing Tips

### For Education:
- **Be specific** with coursework that's relevant to your goals
- **Include GPA** if it's 3.5 or higher
- **Add honors** like Dean's List, scholarships, etc.
- **Keep it concise** - one or two lines of details max

### For Experience:
- **Use action verbs**: Developed, Implemented, Managed, Coordinated
- **Quantify results**: "improved by 40%", "managed 500+ attendees"
- **Show impact**: What did you accomplish? What did you learn?
- **Be specific**: Instead of "helped with conference", write "managed registration for 500+ attendees"

### SIGGRAPH-Specific Tips:
Great things to highlight:
- Specific tracks you worked with (Technical Papers, Art Gallery, etc.)
- Number of attendees you helped
- Any translation/international support
- Networking with companies (Pixar, Disney, NVIDIA, etc.)
- Technical talks or demos you attended
- Skills gained (event management, communication, etc.)

## 📝 Example: Complete SIGGRAPH Entry

```html
<div class="experience-item">
    <div class="experience-header">
        <h5>Student Volunteer - Technical Papers Track</h5>
        <span class="experience-date">July 28 - August 1, 2025</span>
    </div>
    <p class="experience-company">SIGGRAPH 2025, Denver, Colorado</p>
    <ul class="experience-details">
        <li>Coordinated session logistics for 20+ technical paper presentations in the rendering and animation tracks</li>
        <li>Provided attendee support and answered technical questions for 500+ conference participants</li>
        <li>Collaborated with international volunteer team from 15+ countries</li>
        <li>Attended keynote presentations from leaders at NVIDIA, Pixar, and Epic Games</li>
        <li>Networked with researchers and industry professionals in computer graphics and visual effects</li>
        <li>Gained hands-on experience with cutting-edge graphics technology and real-time rendering demos</li>
    </ul>
</div>
```

## 🔄 Order Matters

List your entries in **reverse chronological order** (most recent first):
1. Current/Most Recent (2025)
2. Previous (2024)
3. Older (2023)

This helps recruiters see your most relevant and recent experience first!

## ✅ Final Checklist

- [ ] Updated university name and graduation date
- [ ] Added accurate GPA and relevant coursework
- [ ] Updated SIGGRAPH responsibilities with specifics
- [ ] Used action verbs in bullet points
- [ ] Quantified achievements where possible
- [ ] Listed experiences in reverse chronological order
- [ ] Proofread for typos and grammar
- [ ] Tested on mobile (dates should stack on small screens)

---

Your Education and Experience sections are now ready to impress! 🎓✨
