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
      username: admin
      text: ""
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      avatar:
        size: medium
        shape: circle
      background:
        color: black
        image:
          filename: stacked-peaks.png
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  # ---- Featured Publications ----
  - block: collection
    id: papers
    content:
      title: Featured Publications
      text: '<span style="color:#1E90FF; font-weight:700; font-size:1.1rem; letter-spacing:1px; text-transform:uppercase;">[See All Publications →](/publication/)</span>'
      filters:
        folders: [publication]
        featured_only: true
    design:
      view: article-grid
      columns: 2


      
  # ---- Projects on homepage ----
  - block: collection
    content:
      title: Projects
      text: "A selection of projects across computer vision, edge AI, and real-time analytics."
      filters:
        folders: [project]
    design:
      view: article-grid
      fill_image: false
      columns: 3
 

     # ---- Experience on homepage ----
  - block: resume-experience
    content:
      title: Experience
      username: admin
    design:
      date_format: "January 2006"
      is_education_first: false

---
