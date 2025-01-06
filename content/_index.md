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
      username: adi_prasetyo # Sesuaikan dengan folder di `content/authors/`
      text: >
        Adi Prasetyo adalah mahasiswa Rekayasa Perangkat Lunak di ITESA Semarang
        dan pengembang perangkat lunak dengan fokus pada teknologi modern seperti
        kecerdasan buatan (AI), blockchain, dan pengembangan aplikasi berbasis web
        serta mobile. Aktif mempelajari teknologi baru dan terus memperluas
        keterampilan teknis.
      button:
        text: Download CV
        url: uploads/resume.pdf # Pastikan file ini ada di folder `static/uploads/`
    design:
      css_class: dark
      background:
        color: black
        image:
          filename: stacked-peaks.svg # Pastikan file ini ada di `assets/media/`
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Penelitian Saya'
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
          - publication # Pastikan folder ini ada di `content/`
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Publikasi Terbaru
      filters:
        folders:
          - publication # Pastikan folder ini ada di `content/`
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Diskusi & Seminar Terbaru
      filters:
        folders:
          - event # Pastikan folder ini ada di `content/`
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Berita Terbaru
      page_type: post
      count: 5
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
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
        css_class: "bg-primary-700"
---
        