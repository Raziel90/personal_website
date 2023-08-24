---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: features
  #   content:
  #     title: Skills
  #     items:
  #       - name: Python
  #         description: 90%
  #         icon: fa-python
  #         icon_pack: fab
  #       - name: Machine Learning
  #         description: 100%
  #         icon: fa-brain-circuit
  #         icon_pack: fas
  #       - name: Photography
  #         description: 10%
  #         icon: camera-retro
  #         icon_pack: fas
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
        - title: Applied Scientist
          company: Amazon
          company_url: ''
          # company_logo: amazon
          location: London, UK
          date_start: '2022-07-20'
          date_end: ''
          description: |2-
              Scoped, Developed and deployed cost estimation and volume forecasting solutions for the Amazon Transportation Services Less-Than-Truckload product working in direct contact with business at all the stages of development
        - title: Postdoctoral Researcher
          company: Queen Mary University of London
          company_url: 'https://lorejam.wixsite.com/crisp'
          # company_logo: queen-mary-university
          location: London, UK
          date_start: '2019-05-01'
          date_end: '2022-06-30'
          description: |2-
              * Performed Reseach and supported PhD and Master students as member of the Advanced Robotics Queen-Mary (ARQ) Team.
              * Contributed to and Coordinated the work of PhD/MSc students for the EPSRC MAN3 Project, involving Shadow Robotics, Ocado and Google Deepmind.
              * Conducted research on learning by demonstration for robot manipulation by building a teleoperation platform and a demonstration segmentation system.
        - title: LD11 Cohort Member
          company: Entrepreneur First
          company_url: 'https://www.joinef.com/'
          # company_logo: ef
          location: London, UK
          date_start: '2018-10-01'
          date_end: '2019-01-01'
          description: |2-
              Took the role of CTO cooperating at the ideation of the start-up, public speaking, customer and product development and market analysis.
        - title: Data Scientist
          company: Buzzoole
          company_url: 'https://buzzoole.com/'
          # company_logo: buzzoole
          location: Naples, Italy
          date_start: '2018-04-01'
          date_end: '2018-09-30'
          description: |2-
            - Led the data science team, worked on several Machine Learning Projects central to raise $8.9M funding for the company to improve the analytics product
            - Object Detection in Social Media Images. This project helped to provide analytics about influencer topics to the company platform.
            - Fake Influencer Detection. This project tried to detect fake accounts and accounts using fake influencers to boost their metrics.
        - title: Research Associate
          company: University of Lincoln
          company_url: 'https://lcas.lincoln.ac.uk/'
          # company_logo: uol
          location: Lincoln, UK
          date_start: '2017-01-01'
          date_end: '2018-06-30'
          description: |2-
            - Developed state-of-the-art Human Activity Recognition and Re-identiﬁcation models used in the EU H2020 research projects ENRICHME and FLOBOT.
            - Teaching Assistant for courses of Artiﬁcial Intelligence and Robotics.
        - title: Business Intelligence Consultant
          company: KPMG Advisory
          company_url: 'https://kpmg.com/'
          # company_logo: kpmg
          location: Rome, Italy
          date_start: '2014-01-01'
          date_end: '2014-06-30'
          description: |2-
            - Automated daily BI maintenance tasks with a speed-up above 90% and developed SQL queries to generate BI reports.
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org/account/accomplishments/verify/7V8WQJYTV3E2
          date_end: ''
          date_start: '2019-01-01'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Machine Learning
          url: ''
        - certificate_url: https://graduation.udacity.com/confirm/e/c883be94-8156-11eb-8ddb-3b818c0fccf8
          date_end: ''
          date_start: '2023-08-01'
          description: Deep Reinforcement Learning Nanodegree
          organization: Udacity
          organization_url: https://www.udacity.com/
          icon: udacity
          icon_pack: custom
          title: Deep Reinforcement Learning Nanodegree
          url: https://graduation.udacity.com/confirm/e/c883be94-8156-11eb-8ddb-3b818c0fccf8
        - certificate_url: https://www.coursera.org/account/accomplishments/specialization/RNPASNNUFD2H
          date_end: ''
          date_start: '2020-07-01'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: 'DeepLearning.AI Deep Learning Specialization'
          url: 'https://www.coursera.org/specializations/deep-learning'
        - certificate_url: ""
          date_end: ''
          date_start: '2022-01-01'
          description: 'Award of 2k for Postdocs working in AI'
          organization: The Alan Turing Institute
          organization_url: https://www.coursera.org
          title: 'Postdoc Enrichment Awards'
          url: 'https://www.turing.ac.uk/work-turing/alan-turing-institute-post-doctoral-enrichment-awards-2022'
        - certificate_url: "https://www.daad.de/en/the-daad/postdocnet/fellows/fellows/#claudio"
          date_end: ''
          date_start: '2022-03-01'
          description: 'Award to a group of excellent international researchers from the field of AI and grow our network of current fellows and alumni.'
          organization: DAAD
          organization_url: https://www.daad.de
          title: 'DAAD AINET Awards'
          url: 'https://www.daad.de/en/the-daad/postdocnet'

    design:
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
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
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
      columns: '1'
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
      subtitle:
      text: |-
        Hi Feel Free to send me an email!
      # Contact (add or remove contact options as necessary)
      email: claudiocoppola90@gmail.com
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      # address:
      #   street: 450 Serra Mall
      #   city: Stanford
      #   region: CA
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/ClaudioInClouds'
        - icon: threads
          icon_pack: custom
          name: I am on threads
          link: 'https://www.threads.net/@fullmetal_scientist'
        # - icon: video
        #   icon_pack: fas
        #   name: Zoom Me
        #   link: 'https://zoom.com'
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
