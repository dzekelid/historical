---
swagger: "2.0"
x-collection-name: LogMeIn
x-complete: 0
info:
  title: GoToWebinar Historical Webinars
  description: "Returns details for completed webinars for the specified organizer
    and completed webinars of other organizers where the specified organizer is a
    co-organizer.\n\nParameters:\n- organizerkey \n- fromTime\n- toTime"
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
  /historicalMeetings:
    get:
      summary: Historical meetings
      description: 'Get historical meetings for the currently authenticated organizer
        that started within the specified date/time range. Remark: Meetings which
        are still ongoing at the time of the request are NOT contained in the result
        array.'
      operationId: HistoricalMeetingsGet
      x-api-path-slug: historicalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
  /organizers/{organizerKey}/historicalMeetings:
    get:
      summary: Historical meetings by organizer
      description: Get historical meetings for the specified organizer that started
        within the specified date/time range. Meetings which are still ongoing at
        the time of the request are not included in the result.
      operationId: OrganizersHistoricalMeetingsByOrganizerKeyGet
      x-api-path-slug: organizersorganizerkeyhistoricalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: organizerKey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
      - By
      - Organizer
  /groups/{groupkey}/historicalMeetings:
    get:
      summary: Historical meetings by group
      description: 'Get historical meetings for the specified group that started within
        the specified date/time range. This API call is only available to users with
        the admin role. This API call is restricted to groups with a maximum of 50
        organizers. Remark: Meetings which are still ongoing at the time of the request
        are NOT contained in the result array.'
      operationId: GroupsHistoricalMeetingsByGroupkeyGet
      x-api-path-slug: groupsgroupkeyhistoricalmeetings-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: endDate
      - in: path
        name: groupkey
      - in: query
        name: startDate
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Meetings
      - By
      - Group
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