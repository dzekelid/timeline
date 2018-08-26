---
swagger: "2.0"
x-collection-name: Google Glass
x-complete: 1
info:
  title: Google Mirror
  description: interacts-with-glass-users-via-the-timeline-
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /mirror/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /timeline:
    get:
      summary: Get Timelines
      description: Retrieves a list of timeline items for the authenticated user.
      operationId: mirror.timeline.list
      x-api-path-slug: timeline-get
      parameters:
      - in: query
        name: bundleId
        description: If provided, only items with the given bundleId will be returned
      - in: query
        name: includeDeleted
        description: If true, tombstone records for deleted items will be returned
      - in: query
        name: maxResults
        description: The maximum number of items to include in the response, used
          for paging
      - in: query
        name: orderBy
        description: Controls the order in which timeline items are returned
      - in: query
        name: pageToken
        description: Token for the page of results to return
      - in: query
        name: pinnedOnly
        description: If true, only pinned items will be returned
      - in: query
        name: sourceItemId
        description: If provided, only items with the given sourceItemId will be returned
      responses:
        200:
          description: OK
      tags:
      - Timeline
    post:
      summary: Update Timeline
      description: Inserts a new item into the timeline.
      operationId: mirror.timeline.insert
      x-api-path-slug: timeline-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Timeline
  /timeline/{id}:
    delete:
      summary: Delete Timeline
      description: Deletes a timeline item.
      operationId: mirror.timeline.delete
      x-api-path-slug: timelineid-delete
      parameters:
      - in: path
        name: id
        description: The ID of the timeline item
      responses:
        200:
          description: OK
      tags:
      - Timeline
    get:
      summary: Get Timeline
      description: Gets a single timeline item by ID.
      operationId: mirror.timeline.get
      x-api-path-slug: timelineid-get
      parameters:
      - in: path
        name: id
        description: The ID of the timeline item
      responses:
        200:
          description: OK
      tags:
      - Timeline
    patch:
      summary: Update Timeline
      description: Updates a timeline item in place. This method supports patch semantics.
      operationId: mirror.timeline.patch
      x-api-path-slug: timelineid-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The ID of the timeline item
      responses:
        200:
          description: OK
      tags:
      - Timeline
---