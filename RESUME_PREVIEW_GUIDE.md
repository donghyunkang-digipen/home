# Resume Preview Feature - How It Works

## 📄 What Changed

Your Resume section now includes:

1. **PDF Preview Window** - Shows your resume directly on the page (desktop/tablet)
2. **Download Button** - Click to download the PDF file
3. **Mobile Fallback** - On mobile devices, shows a download message instead

## 🖥️ How It Looks

### Desktop/Tablet View:
```
┌─────────────────────────────────────┐
│           Resume Section            │
├─────────────────────────────────────┤
│  View my resume below or download   │
│                                     │
│  ┌───────────────────────────────┐ │
│  │                               │ │
│  │     [PDF Preview Window]      │ │
│  │   Your resume appears here    │ │
│  │      (600px height)           │ │
│  │                               │ │
│  └───────────────────────────────┘ │
│                                     │
│     [📥 Download Resume (PDF)]      │
└─────────────────────────────────────┘
```

### Mobile View:
```
┌───────────────────────┐
│   Resume Section      │
├───────────────────────┤
│  View my resume...    │
│                       │
│  ┌─────────────────┐ │
│  │   📄            │ │
│  │  Preview not    │ │
│  │   available     │ │
│  │                 │ │
│  │ Please download │ │
│  └─────────────────┘ │
│                       │
│  [📥 Download PDF]    │
└───────────────────────┘
```

## 🚀 Setup Instructions

### Step 1: Create Your Resume PDF
Create or export your resume as a PDF file. Name it **exactly** `resume.pdf`

### Step 2: Add to Repository
Place `resume.pdf` in the same folder as your `index.html`:

```
your-portfolio/
├── index.html
├── style.css
├── resume.pdf  ← Add your resume here
└── README.md
```

### Step 3: Test Locally
Open `index.html` in a browser. You should see:
- ✅ Your resume displayed in the preview window
- ✅ Download button working

### Step 4: Deploy to GitHub
Upload all files including `resume.pdf` to your GitHub repository.

## 🔧 Customization Options

### Change PDF Filename
If you want to use a different filename (e.g., `Danny_Kang_Resume.pdf`):

**In index.html** (around line 210), change both:
```html
<iframe src="Danny_Kang_Resume.pdf" type="application/pdf"></iframe>

<a href="Danny_Kang_Resume.pdf" class="btn btn-primary" download>
```

### Adjust Preview Height
**In style.css** (around line 478), change:
```css
.resume-preview {
    height: 600px;  /* Change this number */
}
```

### Change Preview Width
**In style.css** (around line 465), change:
```css
.resume-content {
    max-width: 900px;  /* Change this number */
}
```

## 📱 Mobile Behavior Explained

**Why does mobile show a fallback message?**
- Many mobile browsers don't support embedded PDF viewing
- Safari iOS, Chrome mobile, etc. prefer to download PDFs
- This provides a better user experience than a broken preview

**The fallback automatically shows when:**
- Screen width is below 480px
- Browser doesn't support iframe PDF embedding
- PDF fails to load for any reason

## ⚠️ Troubleshooting

### Preview shows blank page
**Solution:**
1. Check that `resume.pdf` exists in the same folder as `index.html`
2. File name must match exactly (case-sensitive!)
3. Make sure it's a valid PDF file
4. Try opening the PDF directly in browser: `file:///path/to/resume.pdf`

### Preview works locally but not on GitHub Pages
**Solution:**
1. Make sure you uploaded `resume.pdf` to GitHub
2. Check the file is in the root directory (same level as index.html)
3. Wait a few minutes for GitHub Pages to update
4. Try hard refresh: Ctrl+F5 (Windows) or Cmd+Shift+R (Mac)

### Download button doesn't work
**Solution:**
1. Check the href matches your PDF filename exactly
2. Make sure `download` attribute is present:
   ```html
   <a href="resume.pdf" download>
   ```

### Preview shows on mobile (but shouldn't)
**This is actually OK!** If the mobile browser supports PDF viewing, it will show. The fallback only appears when needed.

## 💡 Pro Tips

1. **Optimize Your PDF**
   - Keep file size under 2MB for fast loading
   - Use PDF compression tools if needed
   - Make sure text is selectable (not just an image)

2. **Update Regularly**
   - Keep your resume current
   - Just replace the `resume.pdf` file in your repository
   - No code changes needed!

3. **Alternative: Multiple Versions**
   You can offer multiple resume versions:
   ```html
   <a href="resume-technical.pdf" download>Technical Resume</a>
   <a href="resume-creative.pdf" download>Creative Resume</a>
   ```

4. **Test on Different Devices**
   - Desktop Chrome/Firefox
   - Mobile Safari
   - Mobile Chrome
   Each may render slightly differently

## 📊 Browser Support

| Browser | Preview Support | Download Support |
|---------|----------------|------------------|
| Chrome Desktop | ✅ Yes | ✅ Yes |
| Firefox Desktop | ✅ Yes | ✅ Yes |
| Safari Desktop | ✅ Yes | ✅ Yes |
| Edge Desktop | ✅ Yes | ✅ Yes |
| Chrome Mobile | ⚠️ Limited | ✅ Yes |
| Safari Mobile | ❌ No | ✅ Yes |
| Firefox Mobile | ⚠️ Limited | ✅ Yes |

**Legend:**
- ✅ Full support
- ⚠️ Partial support (may show fallback)
- ❌ Shows fallback message

## 🎯 Expected Behavior

**Desktop Users:**
1. Visit Resume section
2. See PDF preview immediately
3. Can scroll through resume in preview
4. Click download button to save

**Mobile Users:**
1. Visit Resume section
2. See fallback message (or preview if browser supports)
3. Click download button
4. PDF opens in browser or downloads

Both experiences are completely normal and expected!

## 🔐 Privacy Note

Your resume is publicly accessible once uploaded to GitHub Pages. Only include information you're comfortable sharing publicly. Consider:
- Using a professional email (not personal)
- Including LinkedIn but not full address
- Phone number is optional

---

Your resume preview is now ready! Just add your `resume.pdf` file and you're all set! 🎉
