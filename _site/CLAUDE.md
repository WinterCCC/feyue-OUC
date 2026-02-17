# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**中国海洋大学飞跃手册** (OUC Feiyue Handbook) is a **non-profit knowledge sharing platform** created by Ocean University of China students to help peers share experiences and practical advice regarding academic advancement, studying abroad, and career development.

### Purpose
The handbook helps students by:
1. Collecting real experiences from successful seniors
2. Providing guidance for preservation, postgraduate exams, studying abroad, and employment
3. Offering mentorship through experienced students
4. Creating a supportive community for career planning

## Project Categories

The handbook covers four main paths for students:

| Category | Content |
|----------|---------|
| **保研升学** (Preservation) | Transfer/promotion programs, summer camps, pre-recommendation |
| **考研深造** (Postgraduate Exams) | Study plans, subject-specific methods, exam strategies |
| **出国留学** (Studying Abroad) | Application experiences, exam prep (TOEFL/GRE), country comparisons |
| **就业创业** (Career/Entrepreneurship) | Job hunting, internship experiences, career planning |

## File Structure

```
.
├── _config.yml          # Jekyll configuration (theme: minima, site metadata)
├── index.md             # Homepage with featured articles and categories
├── about.md             # Project mission and how to use
├── CONTRIBUTING.md      # Detailed contribution guidelines
├── README.md            # Project overview and quick start
├── CLAUDE.md            # This file
├── _posts/              # Blog articles directory
│   ├── YYYY-MM-DD-title1.md
│   ├── YYYY-MM-DD-title2.md
│   └── ...
└── .github/
    ├── workflows/       # GitHub Actions automation (inherited from template)
    └── steps/          # Exercise step guides (inherited from template)
```

### Key Files

- **`index.md`** - Homepage featuring navigation, article highlights, and contribution info
- **`_config.yml`** - Jekyll configuration with site title, theme (minima), and metadata
- **`about.md`** - Project mission, structure, and contributor information
- **`CONTRIBUTING.md`** - Complete guide for writing and submitting articles
- **`_posts/`** - Blog articles following Jekyll naming: `YYYY-MM-DD-title.md`

## Article Format and Structure

### Front Matter (Required)
```yaml
---
title: "Full Article Title"
date: YYYY-MM-DD
categories: [保研/考研/出国/就业]
author: Author Name
---
```

### Recommended Article Structure
1. **Preamble** - Background and credentials
2. **Timeline** - Key preparation phases with specific timeframes
3. **Methods/Strategies** - Detailed techniques and resources
4. **Q&A** - Addressing common questions
5. **Lessons Learned** - Success factors and mistakes
6. **Final Advice** - Encouragement and key takeaways
7. **Author Bio** - Brief professional summary

### Content Standards
- Include quantified results (e.g., "GPA 3.8/4.0", "TOEFL 105", "380/500")
- Provide specific resources and book recommendations
- Share both successes and failures
- Use tables, lists, and clear sections for readability
- Include practical, actionable advice

## Contribution Workflow

### For Contributors
1. Fork the repository
2. Create a branch: `git checkout -b feature/your-article-topic`
3. Create file in `_posts/` with format `YYYY-MM-DD-title.md`
4. Follow the writing standards and template
5. Commit: `git add _posts/YYYY-MM-DD-title.md && git commit -m "Add: Article description"`
6. Push and create Pull Request
7. Await review (typically 3-7 days)

### Review Criteria
- Content authenticity and accuracy
- Follows format and naming conventions
- Proper Markdown formatting
- Clear and well-organized
- Valuable and practical advice

## Technology Stack

- **Jekyll** - Static site generator (built into GitHub Pages)
- **Markdown** - Content format for all articles and pages
- **GitHub Pages** - Hosting and deployment
- **Minima Theme** - Responsive, clean Jekyll theme
- **GitHub Actions** - CI/CD workflows (automated site building)

## Local Development

### Prerequisites
```bash
# Install Ruby and Jekyll
# macOS: brew install ruby jekyll
# Ubuntu: sudo apt-get install ruby-dev jekyll
```

### Running Locally
```bash
# Clone repository
git clone <repository-url>
cd feiyue-ouc

# Install dependencies
bundle install

# Start local server
bundle exec jekyll serve
# Site available at http://localhost:4000
```

### Testing Articles
- Write/edit files in `_posts/`
- Changes auto-reload at `http://localhost:4000`
- Check formatting, links, and images locally before pushing

## Content Management

### Adding Articles
- Create file: `_posts/YYYY-MM-DD-new-article.md`
- Follow template and standards (see CONTRIBUTING.md)
- Submit via Pull Request

### Modifying Existing Articles
- Edit file directly or create new PR
- Include reason for modification
- Preserve author attribution

### Adding Images
1. Create folder: `assets/images/category/`
2. Upload image file
3. Reference in article: `![desc]({{ site.url }}/assets/images/category/image.png)`

## Important Notes

- **Not a software project** - No build commands, tests, or linting required
- **Content-focused** - Primary work is writing and editing Markdown
- **Community-driven** - All content is volunteer contributions
- **Policy-aware** - Guidelines and policies change yearly; articles include context of when written
- **Ethical guidelines** - No ads, spam, or misleading content; real experiences only
- **Open contributions** - Anyone can contribute; reviews ensure quality

## Common Tasks

### View published site
```
https://ouc-feiyue.github.io/
```

### Check for build errors
- GitHub Pages builds automatically on push to `main`
- Check repository settings → Pages for deployment status

### Update categories/navigation
- Modify `_config.yml` navigation section
- Articles filtered by `categories` in front matter

## Best Practices

✅ **Do**
- Write from personal experience
- Include specific dates and numbers
- Share failures and lessons
- Update articles for current year policies
- Provide actionable resources

❌ **Don't**
- Post commercial or promotional content
- Exaggerate or misrepresent facts
- Plagiarize or copy without attribution
- Include sensitive personal information
- Use discriminatory language

## Troubleshooting

**Q: Article doesn't appear after pushing**
A: Wait 1-2 minutes for GitHub Pages to rebuild. Check Actions tab for build errors.

**Q: Markdown formatting looks wrong**
A: Preview locally with `jekyll serve` or use GitHub's preview feature before submitting.

**Q: How to handle outdated information?**
A: Create a new article with current information and note the publication date. Historical articles show their vintage year.

## Contact & Support

- 📧 Email: feiyue@ouc.edu.cn
- 🏢 Location: Student Activity Center 101 (Student Council Office)
- 💬 GitHub Issues: Ask questions and suggest improvements
- 📝 See CONTRIBUTING.md for detailed guidance
