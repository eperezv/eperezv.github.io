---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
#      button:
#        text: Download CV
#        url: uploads/resume.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I have worked in both **natural** and **managed ecosystems**, studying how environmental disturbances affect microbial diversity, community structure, and soil functions related to organic matter decomposition and nutrient cycling. 

        In my first postdoc at the **Biology Centre** (Czech Academy of Sciences, Czech Republic), I shifted my focus to managed ecosystems and other stressors, investigating how landspreading organic materials impacts soil properties and microbial communities. I specifically quantified the spread of environmentally risky bacteria and the release of **antibiotic resistance genes** into the environment.
        
        Recently, in my second postdoc at **INRAE** (France), I joined a research group specializing in the diversity and function of **nitrogen-cycling microorganisms**.
        
        *Please reach out to collaborate* 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
---
