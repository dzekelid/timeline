---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Save or Update Negotiator Timeline Preferences
  version: 1.0.0
  description: Save or update negotiator timeline preferences.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/negotiator/my/preferences/timeline:
    get:
      summary: Get a Negotiators Timeline Preferences
      description: Get a negotiators timeline preferences.
      operationId: Negotiator_GetTimelinePreferences
      x-api-path-slug: apinegotiatormypreferencestimeline-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Negotiators
      - Timeline
      - Preferences
    post:
      summary: Save or Update Negotiator Timeline Preferences
      description: Save or update negotiator timeline preferences.
      operationId: Negotiator_SaveTimelinePreferencesBypreferencesDataContract
      x-api-path-slug: apinegotiatormypreferencestimeline-post
      parameters:
      - in: body
        name: preferencesDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - ""
      - Negotiator
      - Timeline
      - Preferences
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---