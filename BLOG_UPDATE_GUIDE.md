# 📝 Blog Update Guide

This guide will help you easily add new projects and update your blog content.

## 🚀 Quick Update Steps

### Adding a New Project Preview (Main Page)

1. **Open `index.html`**
2. **Find the Blog Section** (around line 574)
3. **Copy the Template** provided in the comments
4. **Update the Following:**
   - `data-category`: Choose from `web-dev`, `it-support`, `programming`, `upcoming`
   - `src`: Your image file name
   - `alt`: Image description
   - `blog__title`: Your project title
   - `blog__description`: Brief project description (2-3 sentences)
   - `blog__date`: Publication date
   - `blog__category`: Display category name
   - `href`: Link to full blog post (`Blog.html#your-project-id`)

### Adding a Full Blog Post (Blog.html)

1. **Open `Blog.html`**
2. **Find the Template Section** (around line 283)
3. **Copy the Template** in the comments
4. **Update the Following:**
   - `id`: Unique identifier for the project
   - `post-title`: Full project title
   - `post-meta`: Date, category, and technologies
   - `post-images`: 3 images showcasing your project
   - `post-content`: Detailed project information

### Adding Upcoming Projects

1. **Open `index.html`**
2. **Find the "ADD NEW UPCOMING PROJECTS HERE" comment** (around line 686)
3. **Copy the Template** provided above it
4. **Update:**
   - Icon class (find icons at [Unicons](https://iconscout.com/unicons))
   - Project name and description
   - Status (Planning Phase, In Progress, etc.)

## 📁 File Structure

```
JimkmyPortfolio-website-/
├── index.html          # Main page with blog previews
├── Blog.html           # Full blog posts
├── style.css           # Styling (usually no changes needed)
├── main.js             # JavaScript (usually no changes needed)
└── images/             # Store your project images here
```

## 🎨 Available Categories

- **`web-dev`** - Web Development projects
- **`it-support`** - IT Support related content  
- **`programming`** - Programming tutorials/comparisons
- **`upcoming`** - Future projects and ideas

## 🖼️ Image Guidelines

- **Size**: Recommended 800x400px or similar aspect ratio
- **Format**: JPG, PNG, or WebP
- **Naming**: Use descriptive names like `project-name-screenshot.jpg`
- **Location**: Place in the same folder as your HTML files

## ⚡ Quick Templates

### Blog Preview Template
```html
<article class="blog__content" data-category="CATEGORY-HERE">
    <div class="blog__image">
        <img src="YOUR-IMAGE.jpg" alt="Alt Text" class="blog__img">
    </div>
    <div class="blog__data">
        <h3 class="blog__title">Your Project Title</h3>
        <p class="blog__description">
            Your project description here...
        </p>
        <div class="blog__meta">
            <span class="blog__date">Month Year</span>
            <span class="blog__category">Category Name</span>
        </div>
        <a href="Blog.html#your-project-id" class="button button--flex button--small blog__button">
            Read More <i class="uil uil-arrow-right button__icon"></i>
        </a>
    </div>
</article>
```

### Upcoming Project Template
```html
<article class="blog__upcoming-item">
    <div class="blog__upcoming-icon">
        <i class="uil uil-ICON-NAME"></i>
    </div>
    <div class="blog__upcoming-data">
        <h4 class="blog__upcoming-project">Project Name</h4>
        <p class="blog__upcoming-description">Brief project description...</p>
        <span class="blog__upcoming-status">Status: In Progress / Coming Soon</span>
    </div>
</article>
```

## 🔧 Common Icons

- Web Development: `uil-globe`, `uil-browser`, `uil-react`
- Mobile Apps: `uil-mobile-android`, `uil-apps`
- AI/ML: `uil-brain`, `uil-robot`
- Database: `uil-database`, `uil-server-network`
- Security: `uil-shield`, `uil-lock`
- Tools: `uil-wrench`, `uil-setting`

## 📱 Testing Your Changes

1. **Open `index.html`** in your browser
2. **Test the category filters** - click each button
3. **Check responsive design** - resize your browser window
4. **Test links** - ensure "Read More" buttons work
5. **Verify images** - all images should load properly

## 🆘 Troubleshooting

### Images Not Loading
- Check file path is correct
- Ensure image files are in the same folder
- Verify image file names match exactly (case-sensitive)

### Category Filter Not Working
- Ensure `data-category` attribute is set correctly
- Check that category name matches available options
- Refresh the page after making changes

### Links Not Working
- Verify the `href` points to the correct `#id` in Blog.html
- Ensure the `id` attribute in Blog.html matches the link

## ✅ Checklist for Adding New Project

- [ ] Add preview in `index.html`
- [ ] Add full post in `Blog.html`  
- [ ] Upload project images
- [ ] Test category filtering
- [ ] Test "Read More" link
- [ ] Check responsive design
- [ ] Update upcoming projects if needed

---

**Need help?** Check the HTML comments in the files for additional guidance!
