---
swagger: "2.0"
x-collection-name: AWS Directory Service
x-complete: 0
info:
  title: AWS Directory Service API Get Directory Limits
  version: 1.0.0
  description: Obtains directory limit information for the current region.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetDirectoryLimits:
    get:
      summary: Get Directory Limits
      description: Obtains directory limit information for the current region.
      operationId: getDirectoryLimits
      x-api-path-slug: actiongetdirectorylimits-get
      parameters:
      - in: query
        name: DirectoryLimits
        description: A DirectoryLimits object that contains the directory limits for
          the current         region
        type: string
      responses:
        200:
          description: OK
      tags:
      - Directories
  /?Action=GetSnapshotLimits:
    get:
      summary: Get Snapshot Limits
      description: Obtains the manual snapshot limits for a directory.
      operationId: getSnapshotLimits
      x-api-path-slug: actiongetsnapshotlimits-get
      parameters:
      - in: query
        name: DirectoryId
        description: Contains the identifier of the directory to obtain the limits
          for
        type: string
      responses:
        200:
          description: OK
      tags:
      - Snapshots
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