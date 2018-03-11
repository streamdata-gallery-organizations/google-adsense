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
  /accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}/adcode:
    get:
      summary: Get Ad Unit Code
      description: Get ad code for the specified ad unit, attaching the specified
        host custom channels
      operationId: adsensehost.accounts.adunits.getAdCode
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client with contains the ad unit
      - in: path
        name: adUnitId
        description: Ad unit to get the code for
      - in: query
        name: hostCustomChannelId
        description: Host custom channel to attach to the ad code
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