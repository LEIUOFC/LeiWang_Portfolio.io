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
      Subtitle: Gas Hydrates Nucletion Mechanisms
      text: Gas hydrates are ice-like crystalline solids where guest molecules such as CH$_4$, H$_2$S, and CO$_2$ can be trapped in water cages. Hydrateas typically form  at low temperatures and high pressures.  Gas hydrates are not only abundant in nature but also represent a promising technology. They have been successfully applied to store, separate, and transport gases, as well as to desalinate seawater. However, the formation and reformation of clathrate hydrates in pipelines during exploitation can cause significant flow assurance issues in the oil and gas industry.
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
      text: I enjoy making things. Here are a selection of data science projects.
      filters:
        folders:
          - project
        # exclude_featured: false
    design:
      view: article-grid
      fill_image: false
      columns: 2
---
