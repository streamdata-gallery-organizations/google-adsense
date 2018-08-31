---
swagger: "2.0"
x-collection-name: Google Adsense
x-complete: 0
info:
  title: Google Adsense API Get Ad Clients
  version: 1.0.0
  description: List all host ad clients in this AdSense account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get Accounts
      description: List hosted accounts associated with this AdSense account by ad
        client id.
      operationId: adsensehost.accounts.list
      x-api-path-slug: accounts-get
      parameters:
      - in: query
        name: filterAdClientId
        description: Ad clients to list accounts for
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Get information about the selected associated AdSense account.
      operationId: adsensehost.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: Account to get information about
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Account
  /accounts/{accountId}/adclients:
    get:
      summary: Get Ad Clients
      description: List all hosted ad clients in the specified hosted account.
      operationId: adsensehost.accounts.adclients.list
      x-api-path-slug: accountsaccountidadclients-get
      parameters:
      - in: path
        name: accountId
        description: Account for which to list ad clients
      - in: query
        name: maxResults
        description: The maximum number of ad clients to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /accounts/{accountId}/adclients/{adClientId}:
    get:
      summary: Get Ad Client
      description: Get information about one of the ad clients in the specified publisher's
        AdSense account.
      operationId: adsensehost.accounts.adclients.get
      x-api-path-slug: accountsaccountidadclientsadclientid-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
  /accounts/{accountId}/adclients/{adClientId}/adunits:
    get:
      summary: Get Ad Units
      description: List all ad units in the specified publisher's AdSense account.
      operationId: adsensehost.accounts.adunits.list
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client for which to list ad units
      - in: query
        name: includeInactive
        description: Whether to include inactive ad units
      - in: query
        name: maxResults
        description: The maximum number of ad units to include in the response, used
          for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad units
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
    patch:
      summary: Update Ad Units
      description: Update the supplied ad unit in the specified publisher AdSense
        account. This method supports patch semantics.
      operationId: adsensehost.accounts.adunits.patch
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-patch
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
      - Advertising
      - Units
    post:
      summary: Create Ad Unit
      description: Insert the supplied ad unit into the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.insert
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-post
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
      - Advertising
      - Units
    put:
      summary: Update Ad Unit
      description: Update the supplied ad unit in the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.update
      x-api-path-slug: accountsaccountidadclientsadclientidadunits-put
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad client
      - in: path
        name: adClientId
        description: Ad client which contains the ad unit
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
  /accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}:
    delete:
      summary: Delete Ad Unit
      description: Delete the specified ad unit from the specified publisher AdSense
        account.
      operationId: adsensehost.accounts.adunits.delete
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitid-delete
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad unit
      - in: path
        name: adClientId
        description: Ad client for which to get ad unit
      - in: path
        name: adUnitId
        description: Ad unit to delete
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
    get:
      summary: Get Ad Unit
      description: Get the specified host ad unit in this AdSense account.
      operationId: adsensehost.accounts.adunits.get
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitid-get
      parameters:
      - in: path
        name: accountId
        description: Account which contains the ad unit
      - in: path
        name: adClientId
        description: Ad client for which to get ad unit
      - in: path
        name: adUnitId
        description: Ad unit to get
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Units
  /accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}/adcode:
    get:
      summary: Get Ad Unit Code
      description: Get ad code for the specified ad unit, attaching the specified
        host custom channels.
      operationId: adsensehost.accounts.adunits.getAdCode
      x-api-path-slug: accountsaccountidadclientsadclientidadunitsadunitidadcode-get
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
      - Advertising
      - Units
  /accounts/{accountId}/reports:
    get:
      summary: Generate Report
      description: Generate an AdSense report based on the report request sent in
        the query parameters. Returns the result as JSON; to retrieve output in CSV
        format specify "alt=csv" as a query parameter.
      operationId: adsensehost.accounts.reports.generate
      x-api-path-slug: accountsaccountidreports-get
      parameters:
      - in: path
        name: accountId
        description: Hosted account upon which to report
      - in: query
        name: dimension
        description: Dimensions to base the report on
      - in: query
        name: endDate
        description: End of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: filter
        description: Filters to be run on the report
      - in: query
        name: locale
        description: Optional locale to use for translating report output to a local
          language
      - in: query
        name: maxResults
        description: The maximum number of rows of report data to return
      - in: query
        name: metric
        description: Numeric columns to include in the report
      - in: query
        name: sort
        description: The name of a dimension or metric to sort the resulting report
          on, optionally prefixed with + to sort ascending or - to sort descending
      - in: query
        name: startDate
        description: Start of the date range to report on in YYYY-MM-DD format, inclusive
      - in: query
        name: startIndex
        description: Index of the first row of report data to return
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Report
  /adclients:
    get:
      summary: Get Ad Clients
      description: List all host ad clients in this AdSense account.
      operationId: adsensehost.adclients.list
      x-api-path-slug: adclients-get
      parameters:
      - in: query
        name: maxResults
        description: The maximum number of ad clients to include in the response,
          used for paging
      - in: query
        name: pageToken
        description: A continuation token, used to page through ad clients
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - Clients
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