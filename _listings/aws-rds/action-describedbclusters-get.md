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
  /?Action=DescribeDBClusters&k=1:
    get:
      summary: Describe D B Clusters
      description: Returns information about provisioned Aurora DB clusters
      operationId: describedbclusters
      parameters:
      - in: query
        name: DBClusterIdentifier
        description: The user-supplied DB cluster identifier
        type: string
      - in: query
        name: Filters.Filter.N
        description: A filter that specifies one or more DB clusters to describe
        type: string
      - in: query
        name: Marker
        description: An optional pagination token provided by a previous            DescribeDBClusters
          request
        type: string
      - in: query
        name: MaxRecords
        description: The maximum number of records to include in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - clusters
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