---
name: Google Adsense
x-slug: google-adsense
description: AdSense is a free, simple way to make money online by placing ads on
  your website. Ads are reviewed to ensure they???re high quality and relevant to
  your content or audience, even when viewed on smartphones and tablets. The result?
  You can make more money online.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Adsense
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/apis.md
specificationVersion: "0.14"
apis:
- name: Google Adsense API Get Accounts
  x-api-slug: google-adsense-api
  description: List hosted accounts associated with this AdSense account by ad client
    id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts
  tags: Advertising,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accounts-get-openapi.md
- name: Google Adsense API Get Account
  x-api-slug: google-adsense-api
  description: Get information about the selected associated AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}
  tags: Advertising,Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountid-get-openapi.md
- name: Google Adsense API Get Ad Clients
  x-api-slug: google-adsense-api
  description: List all hosted ad clients in the specified hosted account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients
  tags: Advertising,Clients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclients-get-openapi.md
- name: Google Adsense API Get Ad Client
  x-api-slug: google-adsense-api
  description: Get information about one of the ad clients in the specified publisher's
    AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}
  tags: Advertising,Clients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientid-get-openapi.md
- name: Google Adsense API Get Ad Units
  x-api-slug: google-adsense-api
  description: List all ad units in the specified publisher's AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits
  tags: Advertising,Units
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunits-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunits-get-openapi.md
- name: Google Adsense API Update Ad Units
  x-api-slug: google-adsense-api
  description: Update the supplied ad unit in the specified publisher AdSense account.
    This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunits-patch-openapi.md
- name: Google Adsense API Create Ad Unit
  x-api-slug: google-adsense-api
  description: Insert the supplied ad unit into the specified publisher AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunits-post-openapi.md
- name: Google Adsense API Update Ad Unit
  x-api-slug: google-adsense-api
  description: Update the supplied ad unit in the specified publisher AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunits-put-openapi.md
- name: Google Adsense API Delete Ad Unit
  x-api-slug: google-adsense-api
  description: Delete the specified ad unit from the specified publisher AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunitsadunitid-delete-openapi.md
- name: Google Adsense API Get Ad Unit
  x-api-slug: google-adsense-api
  description: Get the specified host ad unit in this AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunitsadunitid-get-openapi.md
- name: Google Adsense API Get Ad Unit Code
  x-api-slug: google-adsense-api
  description: Get ad code for the specified ad unit, attaching the specified host
    custom channels.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/adclients/{adClientId}/adunits/{adUnitId}/adcode
  tags: Advertising,Units
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidadclientsadclientidadunitsadunitidadcode-get-openapi.md
- name: Google Adsense API Generate Report
  x-api-slug: google-adsense-api
  description: Generate an AdSense report based on the report request sent in the
    query parameters. Returns the result as JSON; to retrieve output in CSV format
    specify "alt=csv" as a query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///accounts/{accountId}/reports
  tags: Advertising,Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/accountsaccountidreports-get-openapi.md
- name: Google Adsense API Get Ad Clients
  x-api-slug: google-adsense-api
  description: List all host ad clients in this AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients
  tags: Advertising,Clients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclients-get-openapi.md
- name: Google Adsense API Get Ad Client
  x-api-slug: google-adsense-api
  description: Get information about one of the ad clients in the Host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}
  tags: Advertising,Clients
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientid-get-openapi.md
- name: Google Adsense API Get Custom Channels
  x-api-slug: google-adsense-api
  description: List all host custom channels in this AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannels-get-openapi.md
- name: Google Adsense API Update Custom Channels
  x-api-slug: google-adsense-api
  description: Update a custom channel in the host AdSense account. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannels-patch-openapi.md
- name: Google Adsense API Create Custom Channels
  x-api-slug: google-adsense-api
  description: Add a new custom channel to the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannels-post-openapi.md
- name: Google Adsense API Update Custom Channel
  x-api-slug: google-adsense-api
  description: Update a custom channel in the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannels-put-openapi.md
- name: Google Adsense API Delete Custom Channel
  x-api-slug: google-adsense-api
  description: Delete a specific custom channel from the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels/{customChannelId}
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannelscustomchannelid-delete-openapi.md
- name: Google Adsense API Get Custom Channel
  x-api-slug: google-adsense-api
  description: Get a specific custom channel from the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/customchannels/{customChannelId}
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidcustomchannelscustomchannelid-get-openapi.md
- name: Google Adsense API Get URL Channels
  x-api-slug: google-adsense-api
  description: List all host URL channels in the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/urlchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidurlchannels-get-openapi.md
- name: Google Adsense API Add URL Channel
  x-api-slug: google-adsense-api
  description: Add a new URL channel to the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/urlchannels
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidurlchannels-post-openapi.md
- name: Google Adsense API Delete URL Channel
  x-api-slug: google-adsense-api
  description: Delete a URL channel from the host AdSense account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///adclients/{adClientId}/urlchannels/{urlChannelId}
  tags: Advertising,Channels
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/adclientsadclientidurlchannelsurlchannelid-delete-openapi.md
- name: Google Adsense API Create Session
  x-api-slug: google-adsense-api
  description: Create an association session for initiating an association with an
    AdSense user.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///associationsessions/start
  tags: Advertising,Session
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/associationsessionsstart-get-openapi.md
- name: Google Adsense API Verify Session
  x-api-slug: google-adsense-api
  description: Verify an association session after the association callback returns
    from AdSense signup.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///associationsessions/verify
  tags: Advertising,Session
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/associationsessionsverify-get-openapi.md
- name: Google Adsense API Get Report
  x-api-slug: google-adsense-api
  description: Generate an AdSense report based on the report request sent in the
    query parameters. Returns the result as JSON; to retrieve output in CSV format
    specify "alt=csv" as a query parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https://///reports
  tags: Advertising,Report
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/reports-get-openapi.md
- name: Google Adsense API
  x-api-slug: google-adsense-api
  description: AdSense is a free, simple way to make money online by placing ads on
    your website. Ads are reviewed to ensure they???re high quality and relevant to
    your content or audience, even when viewed on smartphones and tablets. The result?
    You can make more money online.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-adsense.png
  humanURL: https://developers.google.com/adsense/
  baseURL: https:///
  tags: Google Adsense
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-adsense/master/_listings/google-adsense/openapi.md
x-common:
- type: x-blog
  url: http://googleadsdeveloper.blogspot.com/search/label/adsense_api
- type: x-blog-rss
  url: http://googleadsdeveloper.blogspot.com/feeds/posts/default?alt=rss
- type: x-developers
  url: https://developers.google.com/adsense/
- type: x-twitter
  url: https://twitter.com/AdSense
- type: x-website
  url: https://www.google.com/adsense/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---