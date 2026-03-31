---
title: Courses
summary: My courses
type: landing

cascade:
  - target:
      path: '{/courses/*/**}'
    type: docs
    params:
      show_breadcrumb: true
  - target:
      path: '{/courses/**}'
    params:
      show_date: false
      reading_time: false
      show_date_updated: false

sections:
  - block: collection
    id: courses
    content:
      title: Courses
      filters:
        folders:
          - courses
    design:
      view: article-grid
      show_read_time: false
      show_date: false
      show_read_more: false
      columns: 1
---
