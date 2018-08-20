---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Historical
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Meeting Get historical meetings by group
  x-api-slug: go-to-meeting
  description: 'Get historical meetings for the specified group that started within
    the specified date/time range. This API call is only available to users with the
    admin role. This API call is restricted to groups with a maximum of 50 organizers.
    Remark: Meetings which are still ongoing at the time of the request are NOT contained
    in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest//groups/{groupKey}/historicalMeetings
  tags: Groups,GroupKey,HistoricalMeetings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/groupsgroupkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/groupsgroupkeyhistoricalmeetings-get-openapi.md
- name: Go To Meeting Get historical meetings
  x-api-slug: go-to-meeting
  description: 'Get historical meetings for the currently authenticated organizer
    that started within the specified date/time range. Remark: Meetings which are
    still ongoing at the time of the request are NOT contained in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest//historicalMeetings
  tags: HistoricalMeetings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/historicalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/historicalmeetings-get-openapi.md
- name: Go To Meeting Get historical meetings by organizer
  x-api-slug: go-to-meeting
  description: 'Get historical meetings for the specified organizer that started within
    the specified date/time range. Remark: Meetings which are still ongoing at the
    time of the request are NOT contained in the result array.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest//organizers/{organizerKey}/historicalMeetings
  tags: Organizers,OrganizerKey,HistoricalMeetings
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/organizersorganizerkeyhistoricalmeetings-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/organizersorganizerkeyhistoricalmeetings-get-openapi.md
- name: Go To Meeting
  x-api-slug: go-to-meeting
  description: Citrix enables business mobility through the secure delivery of apps
    and data to any device on any network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2M/rest
  tags: Historical
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/openapi.md
- name: Go To Webinar Get historical webinars
  x-api-slug: go-to-webinar
  description: Returns details for completed webinars for the specified organizer
    and completed webinars of other organizers where the specified organizer is a
    co-organizer.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest//organizers/{organizerKey}/historicalWebinars
  tags: Organizers,OrganizerKey,HistoricalWebinars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/organizersorganizerkeyhistoricalwebinars-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/organizersorganizerkeyhistoricalwebinars-get-openapi.md
- name: Go To Webinar
  x-api-slug: go-to-webinar
  description: Citrix enables business mobility through the secure delivery of apps
    and data to any device on any network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Historical
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/gotomeeting/openapi.md
x-common:
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---