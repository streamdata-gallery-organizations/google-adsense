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
    patch:
      summary: Update Ad Units
      description: Update the supplied ad unit in the specified publisher AdSense
        account
      operationId: adsensehost.accounts.adunits.patch
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client which contains the ad unit
      - in: query
        name: adUnitId
        description: Ad unit to get
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