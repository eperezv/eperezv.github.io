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
        I study how environmental disturbances, both **natural and managed**, shape soil microbial diversity, community structure, and ecosystem functions such as organic matter decomposition and nutrient cycling. 
        
        During my PhD, I investigated the effects of forest fires in Mediterranean ecosystems on soil microbial communities, including archaea, bacteria and fungi, focusing on the phylogenetic diversity and the relationship with ecosystem functioning. 
        
        In my first postdoc at the **Biology Centre** of the Czech Academy of Sciences (Chequia), I shifted to managed ecosystems and other stressors, examining how the application of organic amendments impacts soil properties and microbial communities. I specifically quantified the environmental dissemination of potentially pathogenic bacteria and the spread of **antibiotic resistance genes**.
        
        Currently, at **INRAE** in France, I work on the diversity and ecological roles of **nitrogen-cycling microorganisms**, aiming to understand their functional responses to agricultural practices.
        
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
