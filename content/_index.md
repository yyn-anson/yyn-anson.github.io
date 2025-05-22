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
      button:
        text: Download CV
        url: uploads/resume.pdf
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
        **👨‍🎓 About Me**  
        I am a self-driven **BSc in Computer Science** student at **McGill University**, specializing in **Data Mining** & **Computational Social Science**.

        **🔍 Research Interest**  
        - **Bias & Misinformation Detection**: Quantifying and tracing misinformation dynamics online.  
        - **Stance Detection**: Determining agreement/disagreement viewpoints in articles.  
        - **Social Event Simulation**: Modeling user profiles & interactions.  
        - **Bot Detection**: Identifying automated social media accounts.  
        - **Recommendation Systems**: Investigating filter bubbles and personalization effects.

        Some specific research questions that interest to me:
          - Can we give evidence of bias/misinformation in the internet?
          - What is the impact of misinformation to the public? How to quantify that?
          - Where are the sources of the misinformation? Can we track them?
          - Articles stance detection, does this article agree/disagree on some viewpoint?

        **👏 Acknowledgments**  
        I would like to express my heartfelt gratitude to my supervisors and mentors for their invaluable guidance and support.

        **Supervisors**  
         - <a href="https://www.cs.sfu.ca/~mhefeeda/">Mohamed Hefeeda</a>  
         - <a href="https://dmas.lab.mcgill.ca/fung/">Benjamin C. M. Fung</a>  
         - <a href="http://www.elenaobukhova.com">Elena Obukhova</a>  

        **Mentors**  
         - <a href="https://zc-alexfan.github.io">Zicong Fan (Alex)</a>  
         - <a href="/authors/gladys-monagan/">Gladys Monagan</a>  
         - <a href="https://www.mcgill.ca/mathstat/tharshanna-nadarajah">Tharshanna Nadarajah</a>  
         - <a href="https://www.linkedin.com/in/yvonne-leung-cfa-6305781a/?originalSubdomain=hk">Yvonne Leung</a>  

        Their encouragement has been instrumental to my journey and growth.

        **🔗 Explore More**  
        Dive deeper into my work:
        - 📄 <a href="#papers">Featured Publications</a>  
        - 🚀 <a href="/projects/">Projects</a>
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
      columns: 1

  - block: collection
    id: hobbies
    content:
      title: Hobbies
      text: |-
        Welcome to my private corner of the internet! Here, you'll find videos showcasing my favorite hobbies—whether I'm shredding riffs on my guitar 🎸, laying down beats on my drums 🥁, or smashing birdies on the badminton court 🏸. Plus, I love sharing fun moments from my life 🎬.

        Music has been my passion for years, and each chord strummed or beat played brings me endless joy and growth.

        I believe that following what makes your heart sing is the secret recipe to mastering any skill ❤️. So grab a seat, explore, and let's have some fun together! ✨
      filters:
        folders:
          - hobbies
    design:
      view: article-grid
      columns: 1

  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: ""
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: false
  #   design:
  #     view: citation

  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     view: article-grid
  #     columns: 1
  
  # - block: collection
  #   id: news
  #   content:
  #     title: Recent News
  #     subtitle: ''
  #     text: ''
  #     # Page type to display. E.g. post, talk, publication...
  #     page_type: post
  #     # Choose how many pages you would like to display (0 = all pages)
  #     count: 5
  #     # Filter on criteria
  #     filters:
  #       author: ""
  #       category: ""
  #       tag: ""
  #       exclude_featured: false
  #       exclude_future: false
  #       exclude_past: false
  #       publication_type: ""
  #     # Choose how many pages you would like to offset by
  #     offset: 0
  #     # Page order: descending (desc) or ascending (asc) date.
  #     order: desc
  #   design:
  #     # Choose a layout view
  #     view: date-title-summary
  #     # Reduce spacing
  #     spacing:
  #       padding: [0, 0, 0, 0]


  # - block: cta-card
  #   demo: true # Only display this section in the Hugo Blox Builder demo site
  #   content:
  #     title: 👉 Build your own academic website like this
  #     text: |-
  #       This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

  #       <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

  #       Easily build anything with blocks - no-code required!
        
  #       From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---
