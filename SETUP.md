# Personal Academic Website Setup

This is a personal academic website for Alex J. Pine, built using the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme.

## About

This website showcases:
- Academic profile and biography
- Research publications
- Project portfolio
- Blog posts
- CV/Resume
- News and announcements

## Deployment

This website is designed to be deployed on GitHub Pages. The repository is configured to automatically build and deploy when changes are pushed to the main branch.

### GitHub Pages Configuration

1. The website is hosted at: `https://ovalb-pine.github.io`
2. GitHub Actions will automatically build and deploy the site from the `main` branch
3. The deployment workflow is defined in `.github/workflows/deploy.yml`

### Local Development

To run the website locally:

1. Install Ruby and Bundler:
   ```bash
   gem install bundler
   ```

2. Install dependencies:
   ```bash
   bundle install
   ```

3. Install Jupyter (required for notebook support):
   ```bash
   pip install jupyter nbconvert
   ```

4. Build and serve the site:
   ```bash
   bundle exec jekyll serve
   ```

5. Visit `http://localhost:4000` in your browser

### Configuration Files

- `_config.yml`: Main site configuration (name, URL, social links, etc.)
- `_data/cv.yml`: CV/Resume content
- `_data/socials.yml`: Social media links
- `_bibliography/papers.bib`: Publication list in BibTeX format
- `_pages/about.md`: About page content

### Content

- **Blog Posts**: Add to `_posts/` directory following `YYYY-MM-DD-title.md` format
- **Projects**: Add to `_projects/` directory
- **Publications**: Add to `_bibliography/papers.bib`
- **News**: Add to `_news/` directory
- **Profile Picture**: Replace `assets/img/prof_pic.jpg`

## Customization

To customize for your own use:

1. Update `_config.yml` with your personal information
2. Modify `_pages/about.md` with your biography
3. Update `_data/socials.yml` with your social media profiles
4. Edit `_data/cv.yml` with your academic background
5. Replace sample publications in `_bibliography/papers.bib` with your own
6. Update or remove sample projects in `_projects/`
7. Replace the profile picture in `assets/img/prof_pic.jpg`

## Features

- Responsive design
- Dark mode support
- Publication management with BibTeX
- Blog with support for various content types (math, code, diagrams)
- Project portfolio
- News announcements
- CV/Resume page
- Search functionality
- Social media integration

## Technical Details

- **Static Site Generator**: Jekyll 4.4.1
- **Theme**: al-folio (customized)
- **Deployment**: GitHub Pages
- **Build Tool**: Bundler
- **Additional Dependencies**: Jupyter (for notebook posts)

## Support

For issues with the al-folio theme, refer to:
- [al-folio documentation](https://github.com/alshedivat/al-folio)
- [al-folio FAQ](https://github.com/alshedivat/al-folio/blob/main/FAQ.md)
- [Jekyll documentation](https://jekyllrb.com/docs/)
