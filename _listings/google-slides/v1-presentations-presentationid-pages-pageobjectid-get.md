---
swagger: "2.0"
info:
  title: Google Slides
  description: An API for creating and editing Google Slides presentations.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: slides.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/presentations/{presentationId}/pages/{pageObjectId}:
    get:
      summary: Get Presentation Page
      description: Gets the latest version of the specified page in the presentation
      operationId: slides.presentations.pages.get
      parameters:
      - in: path
        name: pageObjectId
        description: The object ID of the page to retrieve
      - in: path
        name: presentationId
        description: The ID of the presentation to retrieve
      responses:
        200:
          description: OK
      tags:
      - presentation
      - page
definitions:
  AffineTransform:
    properties:
      scaleX:
        description: This is a default description.
        type: post
      scaleY:
        description: This is a default description.
        type: post
      shearX:
        description: This is a default description.
        type: post
      shearY:
        description: This is a default description.
        type: post
      translateX:
        description: This is a default description.
        type: post
      translateY:
        description: This is a default description.
        type: post
      unit:
        description: This is a default description.
        type: post
  AutoText:
    properties:
      content:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  BatchUpdatePresentationRequest:
    properties:
      requests:
        description: This is a default description.
        type: post
  BatchUpdatePresentationResponse:
    properties:
      presentationId:
        description: This is a default description.
        type: post
      replies:
        description: This is a default description.
        type: post
  Bullet:
    properties:
      glyph:
        description: This is a default description.
        type: post
      listId:
        description: This is a default description.
        type: post
      nestingLevel:
        description: This is a default description.
        type: post
  ColorScheme:
    properties:
      colors:
        description: This is a default description.
        type: post
  ColorStop:
    properties:
      alpha:
        description: This is a default description.
        type: post
      position:
        description: This is a default description.
        type: post
  CreateImageRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  CreateImageResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateLineRequest:
    properties:
      lineCategory:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  CreateLineResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateParagraphBulletsRequest:
    properties:
      bulletPreset:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  CreateShapeRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
      shapeType:
        description: This is a default description.
        type: post
  CreateShapeResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateSheetsChartRequest:
    properties:
      chartId:
        description: This is a default description.
        type: post
      linkingMode:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      spreadsheetId:
        description: This is a default description.
        type: post
  CreateSheetsChartResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateSlideRequest:
    properties:
      insertionIndex:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      placeholderIdMappings:
        description: This is a default description.
        type: post
  CreateSlideResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateTableRequest:
    properties:
      columns:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      rows:
        description: This is a default description.
        type: post
  CreateTableResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CreateVideoRequest:
    properties:
      id:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      source:
        description: This is a default description.
        type: post
  CreateVideoResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  CropProperties:
    properties:
      angle:
        description: This is a default description.
        type: post
      bottomOffset:
        description: This is a default description.
        type: post
      leftOffset:
        description: This is a default description.
        type: post
      rightOffset:
        description: This is a default description.
        type: post
      topOffset:
        description: This is a default description.
        type: post
  DeleteObjectRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
  DeleteParagraphBulletsRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
  DeleteTableColumnRequest:
    properties:
      tableObjectId:
        description: This is a default description.
        type: post
  DeleteTableRowRequest:
    properties:
      tableObjectId:
        description: This is a default description.
        type: post
  DeleteTextRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
  Dimension:
    properties:
      magnitude:
        description: This is a default description.
        type: post
      unit:
        description: This is a default description.
        type: post
  DuplicateObjectRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
      objectIds:
        description: This is a default description.
        type: post
  DuplicateObjectResponse:
    properties:
      objectId:
        description: This is a default description.
        type: post
  Group:
    properties:
      children:
        description: This is a default description.
        type: post
  Image:
    properties:
      contentUrl:
        description: This is a default description.
        type: post
  ImageProperties:
    properties:
      brightness:
        description: This is a default description.
        type: post
      contrast:
        description: This is a default description.
        type: post
      transparency:
        description: This is a default description.
        type: post
  InsertTableColumnsRequest:
    properties:
      insertRight:
        description: This is a default description.
        type: post
      number:
        description: This is a default description.
        type: post
      tableObjectId:
        description: This is a default description.
        type: post
  InsertTableRowsRequest:
    properties:
      insertBelow:
        description: This is a default description.
        type: post
      number:
        description: This is a default description.
        type: post
      tableObjectId:
        description: This is a default description.
        type: post
  InsertTextRequest:
    properties:
      insertionIndex:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      text:
        description: This is a default description.
        type: post
  LayoutPlaceholderIdMapping:
    properties:
      layoutPlaceholderObjectId:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  LayoutProperties:
    properties:
      displayName:
        description: This is a default description.
        type: post
      masterObjectId:
        description: This is a default description.
        type: post
      name:
        description: This is a default description.
        type: post
  LayoutReference:
    properties:
      layoutId:
        description: This is a default description.
        type: post
      predefinedLayout:
        description: This is a default description.
        type: post
  Line:
    properties:
      lineType:
        description: This is a default description.
        type: post
  LineFill:
    properties: []
  LineProperties:
    properties:
      dashStyle:
        description: This is a default description.
        type: post
      endArrow:
        description: This is a default description.
        type: post
      startArrow:
        description: This is a default description.
        type: post
  Link:
    properties:
      pageObjectId:
        description: This is a default description.
        type: post
      relativeLink:
        description: This is a default description.
        type: post
      slideIndex:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  List:
    properties:
      listId:
        description: This is a default description.
        type: post
      nestingLevel:
        description: This is a default description.
        type: post
  NestingLevel:
    properties: []
  NotesProperties:
    properties:
      speakerNotesObjectId:
        description: This is a default description.
        type: post
  OpaqueColor:
    properties:
      themeColor:
        description: This is a default description.
        type: post
  OptionalColor:
    properties: []
  Outline:
    properties:
      dashStyle:
        description: This is a default description.
        type: post
      propertyState:
        description: This is a default description.
        type: post
  OutlineFill:
    properties: []
  Page:
    properties:
      objectId:
        description: This is a default description.
        type: post
      pageElements:
        description: This is a default description.
        type: post
      pageType:
        description: This is a default description.
        type: post
      revisionId:
        description: This is a default description.
        type: post
  PageBackgroundFill:
    properties:
      propertyState:
        description: This is a default description.
        type: post
  PageElement:
    properties:
      description:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
  PageElementProperties:
    properties:
      pageObjectId:
        description: This is a default description.
        type: post
  PageProperties:
    properties: []
  ParagraphMarker:
    properties: []
  ParagraphStyle:
    properties:
      alignment:
        description: This is a default description.
        type: post
      direction:
        description: This is a default description.
        type: post
      lineSpacing:
        description: This is a default description.
        type: post
      spacingMode:
        description: This is a default description.
        type: post
  Placeholder:
    properties:
      index:
        description: This is a default description.
        type: post
      parentObjectId:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Presentation:
    properties:
      layouts:
        description: This is a default description.
        type: post
      locale:
        description: This is a default description.
        type: post
      masters:
        description: This is a default description.
        type: post
      presentationId:
        description: This is a default description.
        type: post
      revisionId:
        description: This is a default description.
        type: post
      slides:
        description: This is a default description.
        type: post
      title:
        description: This is a default description.
        type: post
  Range:
    properties:
      endIndex:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Recolor:
    properties:
      name:
        description: This is a default description.
        type: post
      recolorStops:
        description: This is a default description.
        type: post
  RefreshSheetsChartRequest:
    properties:
      objectId:
        description: This is a default description.
        type: post
  ReplaceAllShapesWithImageRequest:
    properties:
      imageUrl:
        description: This is a default description.
        type: post
      replaceMethod:
        description: This is a default description.
        type: post
  ReplaceAllShapesWithImageResponse:
    properties:
      occurrencesChanged:
        description: This is a default description.
        type: post
  ReplaceAllShapesWithSheetsChartRequest:
    properties:
      chartId:
        description: This is a default description.
        type: post
      linkingMode:
        description: This is a default description.
        type: post
      spreadsheetId:
        description: This is a default description.
        type: post
  ReplaceAllShapesWithSheetsChartResponse:
    properties:
      occurrencesChanged:
        description: This is a default description.
        type: post
  ReplaceAllTextRequest:
    properties:
      replaceText:
        description: This is a default description.
        type: post
  ReplaceAllTextResponse:
    properties:
      occurrencesChanged:
        description: This is a default description.
        type: post
  Request:
    properties: []
  Response:
    properties: []
  RgbColor:
    properties:
      blue:
        description: This is a default description.
        type: post
      green:
        description: This is a default description.
        type: post
      red:
        description: This is a default description.
        type: post
  Shadow:
    properties:
      alignment:
        description: This is a default description.
        type: post
      alpha:
        description: This is a default description.
        type: post
      propertyState:
        description: This is a default description.
        type: post
      rotateWithShape:
        description: This is a default description.
        type: post
      type:
        description: This is a default description.
        type: post
  Shape:
    properties:
      shapeType:
        description: This is a default description.
        type: post
  ShapeBackgroundFill:
    properties:
      propertyState:
        description: This is a default description.
        type: post
  ShapeProperties:
    properties: []
  SheetsChart:
    properties:
      chartId:
        description: This is a default description.
        type: post
      contentUrl:
        description: This is a default description.
        type: post
      spreadsheetId:
        description: This is a default description.
        type: post
  SheetsChartProperties:
    properties: []
  Size:
    properties: []
  SlideProperties:
    properties:
      layoutObjectId:
        description: This is a default description.
        type: post
      masterObjectId:
        description: This is a default description.
        type: post
  SolidFill:
    properties:
      alpha:
        description: This is a default description.
        type: post
  StretchedPictureFill:
    properties:
      contentUrl:
        description: This is a default description.
        type: post
  SubstringMatchCriteria:
    properties:
      matchCase:
        description: This is a default description.
        type: post
      text:
        description: This is a default description.
        type: post
  Table:
    properties:
      columns:
        description: This is a default description.
        type: post
      rows:
        description: This is a default description.
        type: post
      tableColumns:
        description: This is a default description.
        type: post
      tableRows:
        description: This is a default description.
        type: post
  TableCell:
    properties:
      columnSpan:
        description: This is a default description.
        type: post
      rowSpan:
        description: This is a default description.
        type: post
  TableCellBackgroundFill:
    properties:
      propertyState:
        description: This is a default description.
        type: post
  TableCellLocation:
    properties:
      columnIndex:
        description: This is a default description.
        type: post
      rowIndex:
        description: This is a default description.
        type: post
  TableCellProperties:
    properties: []
  TableColumnProperties:
    properties: []
  TableRange:
    properties:
      columnSpan:
        description: This is a default description.
        type: post
      rowSpan:
        description: This is a default description.
        type: post
  TableRow:
    properties:
      tableCells:
        description: This is a default description.
        type: post
  TextContent:
    properties:
      lists:
        description: This is a default description.
        type: post
      textElements:
        description: This is a default description.
        type: post
  TextElement:
    properties:
      endIndex:
        description: This is a default description.
        type: post
      startIndex:
        description: This is a default description.
        type: post
  TextRun:
    properties:
      content:
        description: This is a default description.
        type: post
  TextStyle:
    properties:
      baselineOffset:
        description: This is a default description.
        type: post
      bold:
        description: This is a default description.
        type: post
      fontFamily:
        description: This is a default description.
        type: post
      italic:
        description: This is a default description.
        type: post
      smallCaps:
        description: This is a default description.
        type: post
      strikethrough:
        description: This is a default description.
        type: post
      underline:
        description: This is a default description.
        type: post
  ThemeColorPair:
    properties:
      type:
        description: This is a default description.
        type: post
  UpdateImagePropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateLinePropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdatePageElementTransformRequest:
    properties:
      applyMode:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdatePagePropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateParagraphStyleRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateShapePropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateSlidesPositionRequest:
    properties:
      insertionIndex:
        description: This is a default description.
        type: post
      slideObjectIds:
        description: This is a default description.
        type: post
  UpdateTableCellPropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateTextStyleRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  UpdateVideoPropertiesRequest:
    properties:
      fields:
        description: This is a default description.
        type: post
      objectId:
        description: This is a default description.
        type: post
  Video:
    properties:
      id:
        description: This is a default description.
        type: post
      source:
        description: This is a default description.
        type: post
      url:
        description: This is a default description.
        type: post
  VideoProperties:
    properties: []
  WeightedFontFamily:
    properties:
      fontFamily:
        description: This is a default description.
        type: post
      weight:
        description: This is a default description.
        type: post
  WordArt:
    properties:
      renderedText:
        description: This is a default description.
        type: post
  WriteControl:
    properties:
      requiredRevisionId:
        description: This is a default description.
        type: post
x-collection-name: Google Slides
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