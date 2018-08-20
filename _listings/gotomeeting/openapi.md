---
swagger: "2.0"
x-collection-name: GoToMeeting
x-complete: 1
info:
  title: Go To Webinar
  description: the-gotowebinar-api-provides-seamless-integration-of-webinar-registrant-and-attendee-data-into-your-existing-infrastructure-or-thirdparty-applications--the-ability-to-register-participants-as-well-as-pull-lists-of-registrants-and-attendees-for-a-webinar-allows-organizers-to-manage-the-flow-of-information-between-their-primary-applications-without-manual-intervention-
  termsOfService: https://developer.citrixonline.com/terms-use
  contact:
    name: Developer Support
    url: https://developer.citrixonline.com
    email: developer-support@citrixonline.com
  version: 1.0.0
host: api.citrixonline.com
basePath: /G2W/rest
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizers/{organizerKey}/historicalWebinars:
    get:
      summary: Get historical webinars
      description: Returns details for completed webinars for the specified organizer
        and completed webinars of other organizers where the specified organizer is
        a co-organizer.
      operationId: getHistoricalWebinars
      x-api-path-slug: organizersorganizerkeyhistoricalwebinars-get
      parameters:
      - in: query
        name: fromTime
        description: A required start of datetime range in ISO8601 UTC format, e
      - in: query
        name: No Name
      - in: query
        name: toTime
        description: A required end of datetime range in ISO8601 UTC format, e
      responses:
        200:
          description: OK
      tags:
      - Organizers
      - OrganizerKey
      - HistoricalWebinars
---