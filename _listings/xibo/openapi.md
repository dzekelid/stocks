swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /playlist/widget/stocks/{playlistId}:
    post:
      summary: Add a Stocks Widget
      description: Add a new Stocks Widget to the specified playlist
      operationId: WidgetStocksAdd
      x-api-path-slug: playlistwidgetstocksplaylistid-post
      parameters:
      - in: formData
        name: backgroundColor
        description: A HEX color to use as the background color of this widget
      - in: formData
        name: dateFormat
        description: The format to apply to all dates returned by he widget
      - in: formData
        name: duration
        description: Widget Duration
      - in: formData
        name: durationIsPerPage
        description: A flag (0, 1), The duration specified is per page, otherwise
          the widget duration is divided between the number of pages/items
      - in: formData
        name: effect
        description: 'Effect that will be used to transitions between items, available
          options: fade, fadeout, scrollVert, scollHorz, flipVert, flipHorz, shuffle,
          tileSlide, tileBlind'
      - in: formData
        name: items
        description: Items wanted, can be comma separated
      - in: formData
        name: itemtemplate
        description: Template for each item, replaces [itemsTemplate] in main template,
          Pass only with overrideTemplate set to 1
      - in: formData
        name: javaScript
        description: Optional JavaScript, Pass only with overrideTemplate set to 1
      - in: formData
        name: mainTemplate
        description: Main template, Pass only with overrideTemplate set to 1
      - in: formData
        name: maxItemsPerPage
        description: This is the intended number of items on each page
      - in: formData
        name: name
        description: Optional Widget Name
      - in: formData
        name: noRecordsMessage
        description: A message to display when there are no records returned by the
          search query
      - in: formData
        name: overrideTemplate
        description: flag (0, 1) set to 0 and use templateId or set to 1 and provide
          whole template in the next parameters
      - in: path
        name: playlistId
        description: The playlist ID to add a Stocks widget
      - in: formData
        name: speed
        description: The transition speed of the selected effect in milliseconds (1000
          = normal)
      - in: formData
        name: styleSheet
        description: Optional StyleSheet Pass only with overrideTemplate set to 1
      - in: formData
        name: templateId
        description: 'Use pre-configured templates, available options: stocks1, stocks2'
      - in: formData
        name: updateInterval
        description: Update interval in minutes, should be kept as high as possible,
          if data change once per hour, this should be set to 60
      - in: formData
        name: useDuration
        description: (0, 1) Select 1 only if you will provide duration parameter as
          well
      responses:
        200:
          description: OK
      tags:
      - Stocks
      - Widget