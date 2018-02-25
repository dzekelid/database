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
  /?Action=PromoteReadReplica&k=1:
    get:
      summary: Promote Read Replica
      description: Promotes a Read Replica DB instance to a standalone DB instance
      operationId: promotereadreplica
      parameters:
      - in: query
        name: BackupRetentionPeriod
        description: The number of days to retain automated backups
        type: string
      - in: query
        name: DBInstanceIdentifier
        description: The DB instance identifier
        type: string
      - in: query
        name: PreferredBackupWindow
        description: The daily time range during which automated backups are created        if
          automated backups are enabled,        using the BackupRetentionPeriod parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - replicas
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