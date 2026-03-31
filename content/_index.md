---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me
      text: ''
      # Show a call-to-action button under your biography? (optional)
      # button:
      #   text: Download CV
      #   url: uploads/cv.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Use the new Gradient Mesh which automatically adapts to the selected theme colors
      background:
        gradient_mesh:
          enable: true

      # Name heading sizing to accommodate long or short names
      name:
        size: md # Options: xs, sm, md, lg (default), xl

      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      biography:
        style: "text-align: justify;"
  - block: markdown
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        <div style="text-align: justify;">

        My research addresses a fundamental challenge at the intersection of deep learning and human-centric AI: how can we build machine learning systems that not only perform with high accuracy but also meaningfully understand, adapt to, and collaborate with humans?

        I work across three interconnected areas: **multimodal deep learning for affective and behavioral understanding**, leveraging smartphone sensors, egocentric vision, and physiological signals; **agentic AI and cognitive architectures for conversational agents**, enabling consistent personality, beliefs, and emotional states; and **scalable generative models for embodied expression**, developing efficient transformer pipelines for text-driven and speech-driven facial animation.

        A flagship application is [Digital Einstein](https://ethz.ch/en/the-eth-zurich/global/digital-einstein.html), an embodied conversational agent that has reached thousands of visitors globally at events including SIGGRAPH, GITEX Global, and the World Economic Forum. My system also powers collaborative applied research in digital health — including a Virtual Psychotherapist for mental health support and RehaBot for patient health education.

        Please reach out to collaborate.

        </div>
    design:
      columns: '1'
  - block: collection
    id: projects
    content:
      title: Research Projects
      count: 10
      sort_by: weight
      sort_ascending: true
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 3
      show_date: false
      show_read_time: false
  - block: markdown
    content:
      title: Funding
      text: |-
        <div style="text-align: justify;">
        My research is supported by competitive grants from national and international funding agencies. Current projects include work on cognitive health monitoring funded by the National Research Foundation Singapore (NRF CREATE – Future Health Technologies 2), animation synthesis funded by an SNF Ambizione grant, and applied digital health projects in collaboration with Swiss universities and hospitals. Past funding includes an ETH Grant and project partnerships with the Hasler Foundation and the University of Basel.
        </div>
    design:
      columns: '1'
  - block: markdown
    content:
      title: Selected Talks
      text: |-
        - **Jan 2026** — *AI Literacy and the Future of Work*, Panel discussion, World Economic Forum, Davos
        - **Nov 2025** — *Beyond Avatars*, Panel discussion, Berlin Science Week, Berlin
        - **Oct 2025** — *A Platform for Interactive AI Character Experiences*, Invited talk, GITEX Global, Dubai
        - **Aug 2025** — Digital Einstein at SIGGRAPH, Vancouver
        - **Oct 2024** — *The Creation of Believable Digital Characters*, Keynote, GITEX Global, Dubai
    design:
      columns: '1'
  - block: markdown
    content:
      title: People
      text: |-
        <div style="text-align: justify;">
        I supervise a team of PhD students and research assistants. I currently supervise three PhD students, and have successfully supervised one PhD to completion. Current PhD projects span user interface optimisation, believable narrative agents, and data-driven animation synthesis for conversational characters. I have supervised 35 Bachelor's, 13 Master's, and 7 semester thesis projects, as well as four student research assistants working on the Digital Einstein project.
        </div>
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
      show_read_time: false
  - block: collection
    content:
      title: All Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
      show_read_time: false
  - block: markdown
    content:
      title: Teaching
      text: |-
        | Course | Role | Institution | Years |
        |---|---|---|---|
        | Artificial Intelligence for Digital Characters | Course creator & lecturer | ETH Zurich | 2024 – present |
        | Seminar on Digital Humans | Course creator & lecturer | ETH Zurich | 2022 – present |
    design:
      columns: '1'
---
