---
swagger: "2.0"
x-collection-name: ClimaCell
x-complete: 0
info:
  title: ClimaCell Post Historical
  description: "## Historical Weather Data\nThe ```historical``` API call provides
    a time-series of weather information for a specific location and time period.
    The location can be specified as a geocode, or one of your own defined locations
    (see ```locations``` API calls). The weather parameters returned are detailed
    in the __Weather Data__ section.\n###\nNOTES:\nFor the current release, the ```historical```
    call provides data for non\xADprecipitation parameters only, all the way to 1997.
    In addition, you can get precipitation data up to 6 hours back. In the upcoming
    releases, the API will include precipitation data starting from Aug 2017 onward
    (ClimaCell\u2019s proprietary precipitation model) and precipitation classification
    (snow, rain, freezing rain) starting from Jan 2018.\nThe farther back in history
    you go, the less comprehensive the weather data will be, as a result of measurements
    availability for that period of time."
  version: 1.0.0
host: api2.climacell.co
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /historical:
    post:
      summary: Post Historical
      description: "## Historical Weather Data\nThe ```historical``` API call provides
        a time-series of weather information for a specific location and time period.
        The location can be specified as a geocode, or one of your own defined locations
        (see ```locations``` API calls). The weather parameters returned are detailed
        in the __Weather Data__ section.\n###\nNOTES:\nFor the current release, the
        ```historical``` call provides data for non\xADprecipitation parameters only,
        all the way to 1997. In addition, you can get precipitation data up to 6 hours
        back. In the upcoming releases, the API will include precipitation data starting
        from Aug 2017 onward (ClimaCell\u2019s proprietary precipitation model) and
        precipitation classification (snow, rain, freezing rain) starting from Jan
        2018.\nThe farther back in history you go, the less comprehensive the weather
        data will be, as a result of measurements availability for that period of
        time."
      operationId: -historical-weather-datathe-historical-api-call-provides-a-timeseries-of-weather-information-for-a-s
      x-api-path-slug: historical-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Weather
      - Historical
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