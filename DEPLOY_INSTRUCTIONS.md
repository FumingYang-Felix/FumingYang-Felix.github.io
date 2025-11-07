# 🚀 Deployment Instructions

## Quick Deploy to GitHub Pages

### 1. Create GitHub Repository
```bash
# Create a new repository named: YourUsername.github.io
# Example: FumingYang-Felix.github.io
```

### 2. Push to GitHub
```bash
cd PersonalWebsite
git init
git add .
git commit -m "Initial commit: Personal academic website"
git branch -M main
git remote add origin https://github.com/YourUsername/YourUsername.github.io.git
git push -u origin main
```

### 3. Enable GitHub Pages
1. Go to repository **Settings** → **Pages**
2. Under **Source**, select **GitHub Actions**
3. Wait 2-3 minutes for deployment

### 4. Access Your Website
```
https://YourUsername.github.io
```

---

## Local Preview (Optional)

### Using rbenv + Ruby
```bash
# Install dependencies
bundle install

# Start server
bundle exec jekyll serve --host=0.0.0.0 --port=4000

# Visit: http://localhost:4000
```

---

## 📝 Configuration Files

### Main Config: `_config.yml`
- Site metadata (name, email, description)
- Social media links
- Google Scholar ID

### Content Files
- `_pages/about.md` - Homepage content
- `_bibliography/papers.bib` - Publications (BibTeX format)
- `_news/*.md` - News announcements
- `_data/repositories.yml` - GitHub repos to display

### Assets
- `assets/img/prof_pic.jpg` - Profile picture (replace with yours!)
- `assets/img/publication_preview/` - Paper preview images

---

## 🔧 Customization

### Add Publications
Edit `_bibliography/papers.bib`:
```bibtex
@article{yourpaper2025,
  title={Your Paper Title},
  author={Your Name and Coauthors},
  journal={Venue},
  year={2025},
  arxiv={xxxx.xxxxx},
  code={https://github.com/...},
  selected={true}
}
```

### Add News
Create `_news/announcement_YYYY_MM_DD.md`:
```markdown
---
layout: post
date: 2025-11-07
inline: true
---

🎉 Your announcement here!
```

---

## ⚙️ Important Notes

1. **Profile Picture**: Replace `assets/img/prof_pic.jpg` with your photo
2. **GitHub Repo**: Update repository URLs in `_config.yml`
3. **Domain**: Optionally set custom domain in repository settings
4. **Build Time**: First deployment takes ~5 minutes

---

## 📚 Theme Documentation

Original theme: [al-folio](https://github.com/alshedivat/al-folio)

For advanced customization, see the theme's documentation.

---

## ✅ Pre-Deployment Checklist

- [ ] Updated `_config.yml` with your information
- [ ] Replaced `assets/img/prof_pic.jpg` with your photo
- [ ] Added your publications to `_bibliography/papers.bib`
- [ ] Created news announcements in `_news/`
- [ ] Updated `_data/repositories.yml` with your GitHub repos
- [ ] Verified all links work correctly

**Ready to deploy!** 🚀

