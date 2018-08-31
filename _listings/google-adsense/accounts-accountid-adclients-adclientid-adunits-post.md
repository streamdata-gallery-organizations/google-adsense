---
swagger: "2.0"
info:
  title: Google Adsense Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{accountId}/adclients/{adClientId}/adunits:
    post:
      summary: Create Ad Unit
      description: Insert the supplied ad unit into the specified publisher AdSense
        account
      operationId: adsensehost.accounts.adunits.insert
      parameters:
      - in: path
        name: accountId
        description: Account which will contain the ad unit
      - in: path
        name: adClientId
        description: Ad client into which to insert the ad unit
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - advertising
      - units
definitions: []
x-collection-name: Google Adsense
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