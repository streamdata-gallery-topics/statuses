---
name: Chicago Illinois 311
x-slug: chicago-illinois-311
description: Call 311 for assistance with non-emergency City Services and for information
  on events, programs and agencies within the City of Chicago.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/6A231614-652B-4334-852C-54261F4B13BD
x-kinRank: "7"
x-alexaRank: "0"
tags: Statuses
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/chicago-illinois-311/apis.md
specificationVersion: "0.14"
apis:
- name: Chicago Open311 GeoReport API - Current Status
  x-api-slug: requestservice-request-id-response-format-get
  description: Query the current status of an individual request
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/6A231614-652B-4334-852C-54261F4B13BD
  humanURL: http://cityofchicago.org/311
  baseURL: https://311api.cityofchicago.org//open311/v2/
  tags: 311, Open311
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/chicago-illinois-311/requestservice-request-id-response-format-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/statuses/master/_listings/chicago-illinois-311/requestservice-request-id-response-format-get-openapi.md
x-common:
- type: x-website
  url: http://cityofchicago.org/311
- type: x-api-gallery
  url: http://brookline.massachusetts.311.api.gallery.streamdata.io
- type: x-open-311-feed
  url: http://311api.cityofchicago.org/open311/v2/services.xml?jurisdiction_id=cityofchicago.org
- type: x-twitter
  url: https://twitter.com/Chicago311
- type: x-website
  url: https://www.cityofchicago.org/city/en/depts/311.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---