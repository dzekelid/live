---
swagger: "2.0"
x-collection-name: AWS Config
x-complete: 0
info:
  title: AWS Config API Put Delivery Channel
  version: 1.0.0
  description: Creates a delivery channel object to deliver configuration information
    to an Amazon S3 bucket and Amazon SNS topic.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DeleteDeliveryChannel:
    get:
      summary: Delete Delivery Channel
      description: Deletes the delivery channel.
      operationId: deleteDeliveryChannel
      x-api-path-slug: actiondeletedeliverychannel-get
      parameters:
      - in: query
        name: DeliveryChannelName
        description: The name of the delivery channel to delete
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=DescribeDeliveryChannels:
    get:
      summary: Describe Delivery Channels
      description: Returns details about the specified delivery channel.
      operationId: describeDeliveryChannels
      x-api-path-slug: actiondescribedeliverychannels-get
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=DescribeDeliveryChannelStatus:
    get:
      summary: Describe Delivery Channel Status
      description: Returns the current status of the specified delivery channel.
      operationId: describeDeliveryChannelStatus
      x-api-path-slug: actiondescribedeliverychannelstatus-get
      parameters:
      - in: query
        name: DeliveryChannelNames
        description: A list of delivery channel names
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
  /?Action=PutDeliveryChannel:
    get:
      summary: Put Delivery Channel
      description: Creates a delivery channel object to deliver configuration information
        to an Amazon S3 bucket and Amazon SNS topic.
      operationId: putDeliveryChannel
      x-api-path-slug: actionputdeliverychannel-get
      parameters:
      - in: query
        name: DeliveryChannel
        description: The configuration delivery channel object that delivers the configuration
          information to an Amazon S3 bucket, and to an Amazon SNS topic
        type: string
      responses:
        200:
          description: OK
      tags:
      - Delivery Channels
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