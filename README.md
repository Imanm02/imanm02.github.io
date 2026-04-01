# Iman Mohammadi - Personal Academic Website

My personal academic portfolio website, built with [Jekyll](https://jekyllrb.com/) and hosted on [GitHub Pages](https://pages.github.com/).

**Live at:** [https://imanm02.github.io](https://imanm02.github.io)

## Structure

| Page | Path | Description |
|---|---|---|
| Landing | `/` | Intro, about, selected publications & projects, experience, education, honors |
| Research | `/research/` | Full list of publications with [Paper], [GitHub], [Poster] links |
| Projects | `/projects/` | All projects with descriptions, tags, and links |
| Teaching | `/teaching/` | Teaching assistant roles at Sharif University |
| Service | `/service/` | Conference reviewing and student leadership |
| Honors | `/honors/` | Awards and achievements |
| Updates | `/updates/` | Full news timeline |

## Data Files

All content is managed through YAML files in `_data/`:

| File | Content |
|---|---|
| `bio.yml` | Name, bio, research interests, social links |
| `publications.yml` | Papers with authors, venue, and resource links |
| `projects.yml` | Project descriptions, tags, images, and GitHub links |
| `experience.yml` | Research and professional positions |
| `education.yml` | Degrees and institutions |
| `teaching.yml` | TA roles and courses |
| `service.yml` | Reviewing and volunteering |
| `honors.yml` | Awards and rankings |
| `updates.yml` | News entries |

## Adding Content

### New Publication
Add an entry to `_data/publications.yml`:
```yaml
- title: "Paper Title"
  authors: "Author1, Author2, Iman Mohammadi"
  venue: "Conference Name"
  year: 2025
  month: "May"
  selected: true          # show on landing page
  paper: "https://..."    # [Paper] link
  github: "https://..."   # [GitHub] link
  poster: "/assets/pdf/poster.pdf"  # [Poster] link
  slides: "/assets/pdf/slides.pdf"  # [Slides] link
  video: "https://..."    # [Video] link
  code: "https://..."     # [Code] link
```
Only add the fields you need - missing fields are simply not rendered.

### New Project
Add an entry to `_data/projects.yml`:
```yaml
- title: "Project Name"
  description: "Short description."
  image: "/assets/img/project-name.png"  # landscape ~16:9
  selected: true
  tags: ["Tag1", "Tag2"]
  link: "https://..."
  github: "https://github.com/..."
```

### New Update
Add an entry to the top of `_data/updates.yml`:
```yaml
- date: "Mar 2025"
  text: "Your update text here."
```

## Local Development

```bash
bundle install
bundle exec jekyll serve
```
Then open [http://localhost:4000](http://localhost:4000).

## Tech Stack

- **Framework:** Jekyll
- **Hosting:** GitHub Pages
- **Fonts:** Inter, Space Grotesk (Google Fonts)
- **Styling:** Vanilla CSS with custom properties
