---
# Leave the homepage title empty to use the site title
title: 
date: 
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: features
    content:
      title: Skills
      items:
        - name: R
          description: Advanced
          icon: r-project
          icon_pack: fab        
        - name: Python
          description: Beginner
          icon: python
          icon_pack: fab
        - name: Statistics
          description: Advanced
          icon: chart-line
          icon_pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Researcher
          company: ALSOLIFE
          company_url: 'https://www.alsolife.com/national/'
          company_logo: org-also
          location: Beijing
          date_start: '2022-06-06'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Manuscript writing
              * Analysing & modelling
              * Work-flow building
              * Poduct design
              * Patent strategy design
        - title: Research Assisstant
          company: Tao Li's Psychiatry Lab at Zhejiang University
          company_url: 'https://www.zju.edu.cn/english/'
          company_logo: org-zu
          location: Hangzhou
          date_start: '2021-01-01'
          date_end: '2021-11-30'
          description: |2-
              Responsibilities include:

              * Manuscript writing
              * Analysing & modelling
              * Research design
              * Data collecting
              * Funding application
              * Lab management & Project management
        - title: Research Assisstant
          company: Tao Li's Psychiatry Lab at Sichuan University
          company_url: 'https://en.scu.edu.cn/'
          company_logo: org-hx
          location: Chengdu
          date_start: '2020-08-01'
          date_end: '2020-12-30'
          description: |2-
              Responsibilities include:

              * Manuscript writing
              * Data collecting
    design:
      columns: '2'
  - block: experience
    content:
      title: Education
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: M.S. in Applied Psychology
          company: The Chinese University of Hong Kong, Shenzhen
          company_url: 'https://cuhk.edu.cn/en'
          company_logo: org-cuhk
          location: Beijing
          date_start: '2022-06-06'
          date_end: ''
          description: |2-
             * Advisor: Prof. Freedom Y.K. Leung
             * Admission Scholarship 2018
        - title: B.A. in Chinese & B.P. in Philosophy
          company: Beijing Normal University
          company_url: 'https://english.bnu.edu.cn/'
          company_logo: org-bnu
          location: Beijing
          date_start: '2014-09-01'
          date_end: '2018-07-01'
          description: |2-
              * The Outstanding Intern in 2017 education internship
              * Academic Excellence Award 2016
              * Best Report Award 3rd prize (NRRA of China)
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: '2'
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Mental Health
          tag: 'Mental Health'
        - name: Other
          tag: Statistics
          tag: Machine Learning
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
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
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      address:
        street: 19 Huangping Road
        region: Beijing
        postcode: '102200'
        country: CN
        country_code: CN
      directions: Enter Building E and take the stairs to Office 416 on Floor 4
      office_hours:
        - 'Monday 10:00 to 13:00'
        - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/Kiosiky_J'
      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
