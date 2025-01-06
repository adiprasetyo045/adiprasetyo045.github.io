---
# Website name
title: Adi Prasetyo | Mahasiswa dan Pengembang Perangkat Lunak
# Website URL
baseURL: 'https://adiprasetyo.dev/'
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: adi_prasetyo
      text: >
        Adi Prasetyo adalah mahasiswa Rekayasa Perangkat Lunak di ITESA Semarang
        dan pengembang perangkat lunak dengan fokus pada teknologi modern seperti
        kecerdasan buatan (AI), blockchain, dan pengembangan aplikasi berbasis web
        serta mobile. Aktif mempelajari teknologi baru dan terus memperluas
        keterampilan teknis.
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
      title: '📚 Penelitian Saya'
      subtitle: ''
      text: |-
        Gunakan bagian ini untuk menjelaskan misi Anda. Saya adalah mahasiswa dan pengembang perangkat lunak yang aktif mengeksplorasi berbagai teknologi modern seperti kecerdasan buatan (AI), blockchain, dan pengembangan aplikasi.

        Saya mengaplikasikan pendekatan berbasis riset untuk memahami peran teknologi dalam menyelesaikan tantangan dunia nyata dan meningkatkan efisiensi dalam berbagai sektor.

        Jangan ragu untuk menghubungi saya untuk kolaborasi! 😃
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Publikasi Unggulan
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Publikasi Terbaru
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Diskusi & Seminar Terbaru
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Berita Terbaru
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
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
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: false
    content:
      title: 👉 Bangun Website Akademik Anda Sendiri
      text: |-
        Website ini dibuat dengan Hugo Academic - sebuah builder website berbasis Hugo yang GRATIS dan open source, dipercaya oleh 250.000+ akademisi di seluruh dunia.

        Mudah membangun apa saja dengan blok - tanpa perlu kode!

        Mulai dari landing page, CV akademik, hingga blog teknologi.
      button:
        text: Mulai Sekarang
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
