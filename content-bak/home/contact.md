---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle:

content:
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

  # Contact details (edit or remove options as required)
  email: nandischoots@gmail.com
  address:
    street: 30 Aldwych
    city: London 
    region: CA
    postcode: 'WC2B 4BG'
    country: United Kingdom
    country_code: UK
  appointment_url: 'https://calendly.com/nandischoots-1/60min'
  contact_links:
    - icon: twitter
      icon_pack: fab
      name: DM Me
      link: 'https://twitter.com/NandiSchoots'

design:
  columns: '2'
---
