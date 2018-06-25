---
name: YouTube
x-slug: youtube
description: Enjoy the videos and music you love, upload original content, and share
  it all with friends, family, and the world on YouTube.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
x-kinRank: "9"
x-alexaRank: "2"
tags: Live
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/apis.md
specificationVersion: "0.14"
apis:
- name: Youtube Delete Live Broadcasts
  x-api-slug: youtube
  description: Delete livebroadcasts
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-delete-openapi.md
- name: Youtube Get Live Broadcasts
  x-api-slug: youtube
  description: Returns a list of YouTube broadcasts that match the API request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-get-openapi.md
- name: Youtube Add Live Broadcasts
  x-api-slug: youtube
  description: Creates a broadcast.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-post-openapi.md
- name: Youtube Put Live Broadcasts
  x-api-slug: youtube
  description: Updates a broadcast. For example, you could modify the broadcast settings
    defined in the liveBroadcast resource's contentDetails object.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts
  tags: Livebroadcasts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcasts-put-openapi.md
- name: Youtube Add Live Broadcasts Bind
  x-api-slug: youtube
  description: Binds a YouTube broadcast to a stream or removes an existing binding
    between a broadcast and a stream. A broadcast can only be bound to one video stream,
    though a video stream may be bound to more than one broadcast.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/bind
  tags: Livebroadcasts, Bind
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcastsbind-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcastsbind-post-openapi.md
- name: Youtube Add Live Broadcasts Control
  x-api-slug: youtube
  description: Controls the settings for a slate that can be displayed in the broadcast
    stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/control
  tags: Livebroadcasts, Control
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcastscontrol-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcastscontrol-post-openapi.md
- name: Youtube Add Live Broadcasts Transition
  x-api-slug: youtube
  description: Changes the status of a YouTube live broadcast and initiates any processes
    associated with the new status. For example, when you transition a broadcast's
    status to testing, YouTube starts to transmit video to that broadcast's monitor
    stream. Before calling this method, you should confirm that the value of the status.streamStatus
    property for the stream bound to your broadcast is active.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveBroadcasts/transition
  tags: Livebroadcasts, Transition
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcaststransition-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livebroadcaststransition-post-openapi.md
- name: Youtube Delete Livestreams
  x-api-slug: youtube
  description: Deletes a video stream.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveStreams
  tags: Livestreams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-delete-openapi.md
- name: Youtube Get Livestreams
  x-api-slug: youtube
  description: Returns a list of video streams that match the API request parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveStreams
  tags: Livestreams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-get-openapi.md
- name: Youtube Add Livestreams
  x-api-slug: youtube
  description: Creates a video stream. The stream enables you to send your video to
    YouTube, which can then broadcast the video to your audience.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveStreams
  tags: Livestreams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-post-openapi.md
- name: Youtube Put Livestreams
  x-api-slug: youtube
  description: Updates a video stream. If the properties that you want to change cannot
    be updated, then you need to create a new stream with the proper settings.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//liveStreams
  tags: Livestreams
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/livestreams-put-openapi.md
- name: Youtube
  x-api-slug: youtube
  description: Enjoy the videos and music you love, upload original content, and share
    it all with friends, family, and the world on YouTube.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1
  tags: Live
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/live/master/_listings/youtube/openapi.md
x-common:
- type: x-articles
  url: https://developers.google.com/youtube/articles/
- type: x-authentication
  url: https://developers.google.com/youtube/v3/guides/authentication
- type: x-blog
  url: https://youtube-eng.googleblog.com/
- type: x-blog-rss
  url: https://youtube-eng.googleblog.com/feeds/posts/default?alt=rss
- type: x-branding
  url: https://developers.google.com/youtube/branding_guidelines
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/entry
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/list?q=label:API-YouTube
- type: x-buttons
  url: https://developers.google.com/youtube/youtube_subscribe_button
- type: x-crunchbase
  url: https://crunchbase.com/organization/youtube
- type: x-deprecation-policy
  url: https://developers.google.com/youtube/youtube-api-list
- type: x-developer
  url: https://developers.google.com/youtube/
- type: x-email
  url: copyright@youtube.com
- type: x-getting-started
  url: https://developers.google.com/youtube/v3/getting-started
- type: x-github
  url: https://github.com/youtube
- type: x-github
  url: https://github.com/youtube/
- type: x-terms-of-service
  url: https://developers.google.com/youtube/terms
- type: x-training
  url: https://developers.google.com/youtube/training/
- type: x-twitter
  url: https://twitter.com/YouTubeDev
- type: x-twitter
  url: https://twitter.com/YouTube
- type: x-website
  url: https://www.youtube.com/
- type: x-widgets
  url: https://developers.google.com/youtube/youtube_upload_widget
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---