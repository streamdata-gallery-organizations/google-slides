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
x-alexaRank: ""
tags: Google Slides
created: "2018-05-21"
modified: "2018-05-21"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/apis.md
specificationVersion: "0.14"
apis:
- name: Google Slides API Create Presentation
  x-api-slug: google-slides-api
  description: |-
    Creates a new presentation using the title given in the request. Other
    fields in the request are ignored.
    Returns the created presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com////v1/presentations
  tags: Presentation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentations-post-openapi.md
- name: Google Slides API Get Presentation
  x-api-slug: google-slides-api
  description: Gets the latest version of the specified presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com////v1/presentations/{presentationId}
  tags: Presentation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationid-get-openapi.md
- name: Google Slides API Get Presentation Page
  x-api-slug: google-slides-api
  description: Gets the latest version of the specified page in the presentation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com////v1/presentations/{presentationId}/pages/{pageObjectId}
  tags: Presentation, Page
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationidpagespageobjectid-get-openapi.md
- name: Google Slides API Update Presentation
  x-api-slug: google-slides-api
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
  baseURL: ://slides.googleapis.com////v1/presentations/{presentationId}:batchUpdate
  tags: Presentation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/v1presentationspresentationidbatchupdate-post-openapi.md
- name: Google Slides API
  x-api-slug: google-slides-api
  description: The Google Slides API lets you create and modify Google Slides presentations.
    Apps can integrate with the Google Slides API to create beautiful slide decks
    automatically from user- and system-provided data. For example, you could use
    customer details from a database and combine them with predesigned templates and
    selected configuration options to create finished presentations in a fraction
    of the time it would take to create them manually.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-slides-icon.png
  humanURL: https://docs.google.com/presentation/
  baseURL: ://slides.googleapis.com//
  tags: Google Slides
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-slides/master/_listings/google-slides/openapi.md
x-common:
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