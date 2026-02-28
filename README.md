https://josec003.github.io/elpeps-portfolio/

# Porfolio - José Cañas Pérez-Angulo (El Peps) - 2026

This repository is my professional as a professional desginer and illustrator. It's based on scrollitelling to create a more immersive narrative. It allows access to specific projects for a better understanding.

## Main Technologies (Detailed Explanation)

### GitHub Pages

- We've used Pages to publish the project live at a URL like `https://usuario.github.io/proyecto`.
- Deployment is automatic: each commit in `main` updates the site.

### Jekyll

- We haven't used it directly, but Pages uses it in the background.
- A `.nojekyll` file is included to avoid conflicts, unless explicitly required.

### GitHub Actions

- Optional CI workflows included:
  - **Critical CI (Student):** checks links, page weight, and accessibility.

- Encouraged: students learn how professional developers automate quality checks.

## Supporting Technologies (Overview)

- **Markdown:** for `README.md` and `project-brief.md`.
- **YAML:** in `project.yaml` to describe project metadata (title, tagline, URL, etc.).
- **Liquid:** not directly edited by students, but used in professor/course templates to display project info.
- **JSON-LD:** added automatically by templates when projects are listed in the showroom.

## Repository Structure

```plaintext
student-project-template/
├── index.html              # Homepage (semantic HTML)
├── assets/
│   ├── css/
│   │   ├── style.css       # Main entry (imports partials)
│   │   ├── _variables.css  # Design tokens
│   │   ├── _reset.css      # Browser reset
│   │   ├── _base.css       # Typography, links
│   │   ├── _layout.css     # Containers, grids
│   │   ├── _components.css # Header, footer, buttons, cards
│   │   ├── _utilities.css  # Helper classes
│   │   ├── _accessibility.css
│   │   ├── _responsive.css
│   │   └── _print.css
│   └── js/
│       └── main.js         # JavaScript functionality
├── images/                 # Image assets (keep optimized)
├── project.yaml            # Project metadata (complete by Week 4)
├── project-brief.md        # Project concept definition (Week 2)
├── project-inspiration.md  # References and moodboard
├── GETTING-STARTED.md      # Setup and methodology guide
├── README.md               # Instructions and weekly progress log
├── .nojekyll               # Prevents Jekyll processing conflicts
└── .github/workflows/
    └── critical.yml        # Automated quality checks (CI/CD)
```

## Workflow in Practice

1. **Clone Template:** Student creates repo from this template.
2. **Week 1:** Setup repo, push first commit (README updated).
3. **Week 2:** Fill out `project-brief.md` and `project.yaml` (project definition).
4. **Weekly Commits:** Update `index.html`, CSS, JS with new lessons. Each class → one commit.
5. **Week 4:** Ensure `project.yaml` is complete; submit metadata to professor’s repo (via PR or form).
6. **Week 5+:** Continue improving project; reflect on commits.

## Scaling and Feedback

- **Commit Log:** Each commit is a trace of weekly learning.
- **Peer Review:** In Week 5, peers view each other’s projects via the course showroom.
- **CI Feedback:** Automated checks give quick signals (broken links, large assets, accessibility issues).
- **Professor Review:** Spot-checks commits or reviews final project.

## Differences from Other Repos

- `web-foundations`: shared lessons & methodology, not edited by students.
- `professor-course-template`: course-level repo with roster and showroom.
- `student-project-template`: student’s own creative space; only this repo is graded per individual.

## References

- GitHub Pages – [https://docs.github.com/en/pages](https://docs.github.com/en/pages)
- GitHub Actions – [https://docs.github.com/en/actions](https://docs.github.com/en/actions)
- Jekyll (optional background) – [https://jekyllrb.com](https://jekyllrb.com)
- Markdown Guide – [https://www.markdownguide.org](https://www.markdownguide.org)
- YAML Introduction – [https://learnxinyminutes.com/docs/yaml/](https://learnxinyminutes.com/docs/yaml/)
- Schema.org / JSON-LD – [https://schema.org](https://schema.org)

© 2025 Rubén Vega Balbás, PhD — WEB ATELIER (UDIT) · ORCID: <https://orcid.org/0000-0001-6862-9081>
