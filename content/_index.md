---
# Leave the homepage title empty to use the site title
title: ''
date: 2024-08-20
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: About
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    id: experience
    content:
      title: Research Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Assistant Professor of Computer Science
          company: Drexel University
          company_url: ''
          company_logo: drexel
          location: Philadelphia, PA
          date_start: '2024-09-01'
          date_end: ''
          description: 'College of Computing and Informations (CCI)'
        - title: Research Intern
          company: Labs@Google
          company_url: ''
          company_logo: google
          location: Mountain View, CA
          date_start: '2024-05-01'
          date_end: '2024-09-01'
          description: 'Advised by **Nikhil Sarda**<br>Langauge Applications (LangApps) Team<br>Conducted research and user studies on novel large language model (LLM) applications, driving AI innovation and shaping future advancements.<br>Designed and prototyped LLM (Gemini) applications in Python, focusing on usability and real-world implementation.<br>Contributed to confidential research initiatives (details redacted).'
        - title: Graduate Research Assistant
          company: University of Central Florida
          company_url: ''
          company_logo: ucf
          location: Orlando, FL
          date_start: '2020-01-01'
          date_end: '2024-09-01'
          description: 'Advised by **Ryan P. McMahan**<br>Virtual Reality and Virtual Agents'
        - title: Research Intern
          company: Microsoft Research
          company_url: ''
          company_logo: msft
          location: Redmond, WA
          date_start: '2023-05-01'
          date_end: '2023-08-01'
          description: 'Advised by **Ed Cutrell, Martez Mott,** and **John Tang** <br>Ability Team, HCAIX (Human-Computing AI Experiences) Group<br>Researched AI-driven affect and emotion in inclusive avatars using LLMs (GPT-4), Microsoft Mesh, and Unity (C\#).<br>'
    design:
      columns: '2'
      background:
        gradient_end: '#9FA5D5'
        gradient_start: '#E8F5C8'
        text_color_light: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: publications
    content:
      title: 📝 Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      columns: '2'
      view: citation
  - block: markdown
    id: service
    content:
      title: Service
      text: |
        I am especially passionate about diversity in computing. Previously, I have served as a mentor for the **ACM-Women (2020-2022)** chapter at UCF. I cofounded and currently serve as the **External Vice-President of [Girls Who Code @ UCF](https://www.instagram.com/girlswhocodeucf/)**. Due to my love for coding, I also lead the technical interview prep group at GWC@UCF to help prepare our brilliant club members for industry jobs. See below for some of my workshop materials:
        <br><br>[Introduction to Git and GitHub](uploads/GitWorkshop.pdf)
        <br>[Introduction to Technical Interviews - Practice Problems](https://colab.research.google.com/drive/1XBoCPR-FSeRVGuCvlFEm2kATrp76KzEF?usp=sharingf)<br><br> 
        
        Additionally, I have served as an external reviewer for the following journals and conferences: Springer Virtual Reality (2021), ACM MM (2021, 2022), IEEE VR (2022, 2024), ACM CHI (2022, 2023, 2024), IEEE ISMAR (2022).
      
    design:
      # See Page Builder docs for all section customization options.
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
  - block: slider
    content:
      slides:
        - title: 💻 Girls Who Code Executive Board
          align: right
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: GWC2.jpg
              filters:
                brightness: 0.7
            fit: cover
            position: center
        - title: 👋 Girls Who Code Tabling Event
          align: right
          background:
            image:
              # Specify an image from `assets/media/`
              # or delete the image section to remove it
              filename: GWC3.jpg
              filters:
                brightness: 0.7
            position: left
        - title: 🔧 Girls Who Code Git Workshop
          content: 'I taught this!'
          align: right
          background:
            image:
              filename: GWC4.jpg
              filters:
                brightness: 0.7
            position: left
          link:
            text: My slides
            url: uploads/GitWorkshop.
        - title: 👾 Esports @ UCF Staff
          content: 'I was part of marketing leadership from 2020-2022!'
          align: right
          background:
            image:
              filename: esports.jpg
              filters:
                brightness: 0.7
            position: left
    design:
      # Slide height is automatic unless you force a specific height (e.g. '400px')
      slide_height: '600px'
      # Make the slides full screen within the browser window?
      is_fullscreen: false
      # Automatically transition through slides?
      loop: true
      # Duration of transition between slides (in ms)
      interval: 6000
  - block: accomplishments
    content:
      title: Teaching
      subtitle: '📚 A list of courses I have taught for'
      text: ''
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `items` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Augmented Reality Programming (CS T480)
          date_end: '2025-04-01'
          date_start: '2025-01-01'
          organization: Instructor
        - title: Virtual Reality Engineering (CAP 5115)
          date_end: '2024-05-01'
          date_start: '2024-01-01'
          organization: Graduate Teaching Assistant
        - title: Foundations of HCI (CAP 3104)
          date_end: '2023-08-05'
          date_start: '2023-12-01'
          organization: Graduate Teaching Assistant
        - title: Operating Systems Concepts (CGS 3763)
          date_end: '2021-05-05'
          date_start: '2021-01-01'
          organization: Graduate Teaching Assistant
        - title: Computer Science 1 in C (COP 3502C)
          date_end: '2020-12-05'
          date_start: '2020-01-01'
          description: 'Instructed C programming lab classes for 2-3 sections a week (20-40 students per section). Responsible as TA for ~240 students a semester. <br>Nominated for the CECS Award for Excellence by a Graduate Teaching Assistant by Dr. Tanvir Ahmed. '
          organization: Graduate Teaching Assistant & Lab Instructor
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
---
