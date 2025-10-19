---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ''
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Descargar CV
        url: uploads/resume.pdf
      headings:
        about: ''
        education: ''
        interests: ''
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar:
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: markdown
    content:
      title: '🔬 Investigación y líneas de trabajo'
      subtitle: ''
      text: |-
        Soy investigadora postdoctoral en el **Instituto de Ciencias Físicas (UNAM)**. Mi trabajo conecta **electroquímica de la corrosión**, **inhibidores verdes** (extractos y biomoléculas), y **tratamientos con plasmas fríos** para modificar superficies y mejorar su desempeño anticorrosivo. 

        Utilizo **EIS**, **polarización**, y **ensayos gravimétricos**, además de **FTIR/Raman** y **emisión óptica** para caracterizar películas protectoras. Integro **DFT/MD** para comprender la adsorción, enlaces y sinergias iónicas en la interfaz metal–inhibidor.

        Abierta a **colaboraciones** en caracterización, síntesis y evaluación de inhibidores y tratamientos de superficie.
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Publicaciones destacadas
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Publicaciones recientes
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Charlas y seminarios
      filters:
        folders:
          - events
    design:
      view: card

  # NOTE: Se eliminó el bloque de "Recent News" (news) a petición del usuario.

  - block: cta-card
    demo: false
    content:
      title: ¿Colaboramos?
      text: |-
        Si trabajas en **corrosión**, **recubrimientos**, **plasma** o **caracterización electroquímica**, me encantará conocer tu proyecto.
      button:
        text: Contáctame
        url: mailto:america@icf.unam.mx
    design:
      card:
        # Card background color (CSS class)
        css_class: 'bg-primary-300'
        css_style: ''
---

