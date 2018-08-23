---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 1
info:
  title: GoToWebinar API
  description: todo-add-description
  version: 1.0.0
host: api.getgo.com
basePath: /G2W/rest/organizers
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{organizerKey}/historicalWebinars:
    get:
      summary: Historical Webinars
      description: "Returns details for completed webinars for the specified organizer
        and completed webinars of other organizers where the specified organizer is
        a co-organizer.\n\nParameters:\n- organizerkey \n- fromTime\n- toTime"
      operationId: HistoricalWebinarsByOrganizerKeyGet
      x-api-path-slug: organizerkeyhistoricalwebinars-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: fromTime
      - in: path
        name: organizerKey
      - in: query
        name: toTime
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Webinars
---