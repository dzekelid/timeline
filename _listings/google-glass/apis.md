---
name: Google Glass
x-slug: google-glass
description: Glass is fundamentally different than existing mobile platforms in both
  design and use. Follow these principles when building Glassware to give users the
  best experience.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
  Shot 2017-03-16 at 11.10.43 PM.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Timeline
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/apis.md
specificationVersion: "0.14"
apis:
- name: Google Mirror - Get Timelines
  x-api-slug: timeline-get
  description: Retrieves a list of timeline items for the authenticated user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 11.10.43 PM.png
  humanURL: https://developers.google.com/glass/
  baseURL: ://www.googleapis.com//mirror/v1
  tags: Wearables, Glasses, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/timeline-get-openapi.md
- name: Google Mirror - Update Timeline
  x-api-slug: timeline-post
  description: Inserts a new item into the timeline.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 11.10.43 PM.png
  humanURL: https://developers.google.com/glass/
  baseURL: ://www.googleapis.com//mirror/v1
  tags: Wearables, Glasses, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/timeline-post-openapi.md
- name: Google Mirror - Delete Timeline
  x-api-slug: timelineid-delete
  description: Deletes a timeline item.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 11.10.43 PM.png
  humanURL: https://developers.google.com/glass/
  baseURL: ://www.googleapis.com//mirror/v1
  tags: Wearables, Glasses, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/timelineid-delete-openapi.md
- name: Google Mirror - Get Timeline
  x-api-slug: timelineid-get
  description: Gets a single timeline item by ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 11.10.43 PM.png
  humanURL: https://developers.google.com/glass/
  baseURL: ://www.googleapis.com//mirror/v1
  tags: Wearables, Glasses, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/timelineid-get-openapi.md
- name: Google Mirror - Update Timeline
  x-api-slug: timelineid-patch
  description: Updates a timeline item in place. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/Screen
    Shot 2017-03-16 at 11.10.43 PM.png
  humanURL: https://developers.google.com/glass/
  baseURL: ://www.googleapis.com//mirror/v1
  tags: Wearables, Glasses, Google APIs, Stack Network, API Service Provider, API
    Provider, Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/timeline/master/_listings/google-glass/timelineid-patch-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.genomics.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.glass.stack.network
- type: x-authentication
  url: https://developers.google.com/glass/develop/gdk/authentication
- type: x-best-practices
  url: https://developers.google.com/glass/distribute/best-practices
- type: x-getting-started
  url: https://developers.google.com/glass/develop/gdk/quick-start
- type: x-website
  url: https://developers.google.com/glass/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---