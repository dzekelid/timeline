---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
---