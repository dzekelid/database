---
swagger: "2.0"
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ApplyPendingMaintenanceAction&k=1:
    get:
      summary: Apply Pending Maintenance Action
      description: Applies a pending maintenance action to a resource (for example,
        to a DB instance)
      operationId: applypendingmaintenanceaction
      parameters:
      - in: query
        name: ApplyAction
        description: The pending maintenance action to apply to this resource
        type: string
      - in: query
        name: OptInType
        description: A value that specifies the type of opt-in request, or undoes
          an opt-in request
        type: string
      - in: query
        name: ResourceIdentifier
        description: The RDS Amazon Resource Name (ARN) of the resource that the       pending
          maintenance action applies to
        type: string
      responses:
        200:
          description: OK
      tags:
      - maintenance actions
definitions: []
x-collection-name: AWS RDS
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