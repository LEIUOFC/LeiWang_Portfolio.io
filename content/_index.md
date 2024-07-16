---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing
# draft: true
design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # The user's folder name in `content/authors/`
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""

      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download Résumé
        url: uploads/resume.pdf
      button:
        text: Download CV
        url: uploads/cv.pdf

    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: dian7.jpg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: true

  - block: collection
    id: papers
    content:
      title: Projects
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid #article-grid, citation  date-title-summary
      columns: 2
      # For the Showcase view, do you want to flip alternate rows?
      flip_alt_rows: true
      

  # - block: collection
  #   id: publications
  #   content:
  #     title: Recent Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation
      
  - block: collection
    id: case_study
    content:
      title: Case studies
      text: I enjoy making things. Here are a selection of data science projects that I have worked on over the years.
      filters:
        folders:
          - project
        # exclude_featured: false
    design:
      view: article-grid
      fill_image: false
      columns: 2
---
