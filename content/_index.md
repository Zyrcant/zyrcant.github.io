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
          description: 'Advised by **Nikhil Sarda**<br>Langauge Applications (LangApps) Team<br>Conducted research on innovative applications of large language models (LLMs). Designed and prototyped LLM-based tools in Python, emphasizing usability and real-world deployment of AI-generated podacasts.<br>Work recognized with a [Best Paper at CHI 2025](https://doi.org/10.1145/3706598.3713460).<br>Contributed to confidential research initiatives (details redacted).'
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
        I am especially passionate about service in computing. I currently serve as the <strong>faculty advisor</strong> for Drexel’s <strong>Women in Computing Society</strong>, and previously mentored the <strong>ACM-Women</strong> chapter at UCF (2020–2022). I also cofounded and served as <strong>External Vice President</strong> of <a href="https://www.instagram.com/girlswhocodeucf/" target="_blank">Girls Who Code @ UCF</a> from 2022–2024. As part of my commitment to supporting students, I led GWC’s technical interview prep group, helping members gain confidence and skills for industry roles.

        Some of the workshops I created include: <br>
        - <a href="uploads/GitWorkshop.pdf">Introduction to Git and GitHub</a> <br>
        - <a href="https://colab.research.google.com/drive/1XBoCPR-FSeRVGuCvlFEm2kATrp76KzEF?usp=sharing" target="_blank">Technical Interview Practice Problems</a> <br><br>

        In addition to mentoring and student outreach, I actively contribute to the research community through reviewing and editorial service. I have served as an external reviewer for <em>Springer Virtual Reality</em>, <em>ACM Multimedia (ACM MM)</em>, <em>IEEE VR</em>, <em>ACM CHI</em>, <em>IEEE ISMAR</em>, among others—earning multiple <strong>Outstanding Reviewer</strong> distinctions at top HCI venues. I have also served on the <strong>Technical Program Committee</strong> for <em>ACM Multimedia (MM 2022)</em> and <em>ACM Virtual Reality Software and Technology (VRST 2025)</em>, and currently serve as the <strong>Outreach Editor</strong> for <a href="https://dl.acm.org/journal/tochi" target="_blank">ACM Transactions on Computer-Human Interaction (TOCHI)</a>.
 
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
      text: 'Although I teach just one class per term, I place a strong emphasis on quality instruction and consistently receive high student evaluations, with an average instructor rating of **4.75/5**.'
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `items` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Game Design and Development (CS 345)
          date_end: '2025-06-01'
          date_start: '2025-03-01'
          organization: Instructor
        - title: Augmented Reality Programming (CS T480)
          date_end: '2025-03-01'
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
