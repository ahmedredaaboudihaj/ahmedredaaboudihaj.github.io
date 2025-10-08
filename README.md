# Ahmed Reda ABOUDIHAJ - Portfolio Website

A professional, animated portfolio website showcasing video editing and filming projects with a modern, high-tech design.

## 🎨 Features

- **Animated Background**: Dynamic particle system with digital patterns and light streaks
- **Responsive Design**: Fully responsive across all devices (desktop, tablet, mobile)
- **Smooth Animations**: Professional fade-in effects, parallax scrolling, and interactive elements
- **Dark Theme**: Sophisticated dark color scheme with cyan/blue accents
- **Video Editing Focus**: Dedicated section for your filming and editing projects
- **Interactive Elements**: Hover effects, skill bars, typing animations
- **Professional Sections**:
  - Hero section with animated name and call-to-action
  - About section with stats
  - Skills showcase with progress bars
  - Video editing projects gallery
  - Experience timeline
  - Contact information

## 🚀 Getting Started

### Opening the Website

Simply double-click on `index.html` to open it in your default browser!

### Alternative: Using a Local Server (Recommended)

For better performance:

**Option 1 - Python:**
```bash
cd portfolio-website
python -m http.server 8000
# Then open: http://localhost:8000
```

**Option 2 - VS Code Live Server:**
1. Install "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"

## 📝 Customization Guide

### 1. Update Contact Information

Edit `index.html` around lines 480-545:

```html
<!-- Email -->
<a href="mailto:your-email@example.com">your-email@example.com</a>

<!-- Phone -->
<a href="tel:+212XXXXXXXXX">+212 XXX XXX XXX</a>

<!-- Social Links -->
<a href="https://linkedin.com/in/your-profile">LinkedIn</a>
<a href="https://github.com/your-username">GitHub</a>
<a href="https://instagram.com/your-username">Instagram</a>
```

### 2. Add Your Photo

Replace the placeholder in `index.html` (around line 135):

```html
<div class="profile-placeholder">
    <!-- Replace with your photo -->
    <img src="assets/your-photo.jpg" alt="Ahmed Reda ABOUDIHAJ" 
         style="width: 100%; height: 100%; object-fit: cover; border-radius: 15px;">
</div>
```

### 3. Add Your Video Projects

**Step 1:** Add your project images/thumbnails to the `assets` folder

**Step 2:** Update project cards in `index.html` (lines 270-410):

```html
<div class="project-card">
    <div class="project-image">
        <!-- Add your video thumbnail -->
        <img src="assets/your-project-thumbnail.jpg" alt="Project Name" 
             style="width: 100%; height: 100%; object-fit: cover;">
        <div class="project-overlay">
            <button class="view-project">View Project</button>
        </div>
    </div>
    <div class="project-info">
        <h3>Your Project Title</h3>
        <p>Your project description...</p>
        <div class="project-tags">
            <span>Video Editing</span>
            <span>Color Grading</span>
        </div>
    </div>
</div>
```

**Step 3:** Link to your actual videos

Edit `js/script.js` (around line 225) to link to your YouTube, Vimeo, or video files:

```javascript
viewProjectButtons.forEach(button => {
    button.addEventListener('click', (e) => {
        e.stopPropagation();
        // Replace with your video links
        window.open('https://youtube.com/watch?v=YOUR_VIDEO_ID', '_blank');
    });
});
```

### 4. Update Skills

Edit the skills section in `index.html` (lines 150-250):
- Modify skill names
- Adjust progress percentages in `data-progress` attribute
- Add/remove tools in the tool tags section

### 5. Update Experience Timeline

Edit `index.html` (lines 420-480) to add your actual work experience and projects.

## 🎨 Color Customization

To change the color scheme, edit `css/styles.css` (lines 10-20):

```css
:root {
    --accent-cyan: #00d9ff;      /* Main accent color */
    --accent-blue: #0066ff;      /* Secondary accent */
    --accent-purple: #6b4ce6;    /* Tertiary accent */
    --accent-gold: #ffd700;      /* Highlight color */
}
```

## 📱 Responsive Design

The website is fully responsive and optimized for:
- Desktop (1920px and above)
- Laptop (1024px - 1920px)
- Tablet (768px - 1024px)
- Mobile (320px - 768px)

## 🔧 File Structure

```
portfolio-website/
├── index.html          # Main HTML file
├── css/
│   └── styles.css      # All styling and animations
├── js/
│   └── script.js       # Interactive features and animations
├── assets/             # Your images, videos, and media
└── README.md           # This file
```

## 💡 Tips

1. **Optimize Images**: Compress your images before adding them to reduce load time
2. **Video Thumbnails**: Use high-quality thumbnails for your video projects
3. **Test Responsiveness**: Check the website on different devices
4. **Update Regularly**: Keep your projects and experience up to date
5. **SEO**: Update the meta description in `index.html` for better search visibility

## 🎬 Adding Video Links

You can link your projects to:
- **YouTube**: `https://youtube.com/watch?v=VIDEO_ID`
- **Vimeo**: `https://vimeo.com/VIDEO_ID`
- **Google Drive**: Share link to your video
- **Local Files**: `assets/your-video.mp4`

## 📧 Support

If you need help customizing the website, refer to the comments in the code files. Each section is clearly labeled and documented.

## 🚀 Deployment

To publish your website online:

1. **GitHub Pages** (Free):
   - Create a GitHub repository
   - Upload all files
   - Enable GitHub Pages in repository settings

2. **Netlify** (Free):
   - Drag and drop the `portfolio-website` folder to Netlify
   - Get instant deployment

3. **Vercel** (Free):
   - Import your project
   - Deploy with one click

## ✨ Features to Add Later

- Contact form functionality
- Blog section
- Video player integration
- Project filtering
- Dark/Light mode toggle
- Multi-language support

---

**Created for Ahmed Reda ABOUDIHAJ**  
EMSI Marrakech | Future Informatics Engineer | Professional Video Editor & Photographer

Good luck with your portfolio! 🎥✨
