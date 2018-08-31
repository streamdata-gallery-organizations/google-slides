---
name: Google Slides
x-slug: google-slides
description: The Google Slides API lets you create and modify Google Slides presentations.
  Apps can integrate with the Google Slides API to create beautiful slide decks automatically
  from user- and system-provided data. For example, you could use customer details
  from a database and combine them with predesigned templates and selected configuration
  options to create finished presentations in a fraction of the time it would take
  to create them manually.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Slides
created: "2018-08-30"
modified: "2018-08-30"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/apis.md
specificationVersion: "0.14"
apis:
- name: Google Slides - Create Presentation
  x-api-slug: v1presentations-post
  description: |-
    Creates a new presentation using the title given in the request. Other
    fields in the request are ignored.
    Returns the created presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com//
  tags: Google APIs, Slides, Documents, Stack Network, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentations-post-openapi.md
- name: Google Slides - Get Presentation
  x-api-slug: v1presentationspresentationid-get
  description: Gets the latest version of the specified presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com//
  tags: Google APIs, Slides, Documents, Stack Network, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationid-get-openapi.md
- name: Google Slides - Get Presentation Page
  x-api-slug: v1presentationspresentationidpagespageobjectid-get
  description: Gets the latest version of the specified page in the presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com//
  tags: Google APIs, Slides, Documents, Stack Network, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationidpagespageobjectid-get-openapi.md
- name: Google Slides - Update Presentation
  x-api-slug: v1presentationspresentationidbatchupdate-post
  description: |-
    Applies one or more updates to the presentation.

    Each request is validated before
    being applied. If any request is not valid, then the entire request will
    fail and nothing will be applied.

    Some requests have replies to
    give you some information about how they are applied. Other requests do
    not need to return information; these each return an empty reply.
    The order of replies matches that of the requests.

    For example, suppose you call batchUpdate with four updates, and only the
    third one returns information. The response would have two empty replies:
    the reply to the third request, and another empty reply, in that order.

    Because other users may be editing the presentation, the presentation
    might not exactly reflect your changes: your changes may
    be altered with respect to collaborator changes. If there are no
    collaborators, the presentation should reflect your changes. In any case,
    the updates in your request are guaranteed to be applied together
    atomically.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com//
  tags: Google APIs, Slides, Documents, Stack Network, Productivity, API Service Provider,
    API Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationidbatchupdate-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.site.verification.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.slides.stack.network
- type: x-developer
  url: https://developers.google.com/slides/
- type: x-documentation
  url: https://developers.google.com/slides/reference/rest/
- type: x-getting-started
  url: https://developers.google.com/slides/quickstart/android
- type: x-guides
  url: https://developers.google.com/slides/how-tos/overview
- type: x-samples
  url: https://developers.google.com/slides/samples/
- type: x-support
  url: https://developers.google.com/slides/support
- type: x-website
  url: https://docs.google.com/presentation/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---