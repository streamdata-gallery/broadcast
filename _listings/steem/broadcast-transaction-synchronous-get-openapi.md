---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem broadcast_transaction_synchronous
  description: broadcast_transaction_synchronous
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /broadcast_transaction:
    get:
      summary: broadcast_transaction
      description: broadcast_transaction
      operationId: broadcast-transaction
      x-api-path-slug: broadcast-transaction-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
  /broadcast_transaction_synchronous:
    get:
      summary: broadcast_transaction_synchronous
      description: broadcast_transaction_synchronous
      operationId: broadcast-transaction-synchronous
      x-api-path-slug: broadcast-transaction-synchronous-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Transaction
      - Synchronous
  /broadcast_block:
    get:
      summary: broadcast_block
      description: broadcast_block
      operationId: broadcast-block
      x-api-path-slug: broadcast-block-get
      parameters:
      - in: query
        name: b
        description: block
      responses:
        200:
          description: OK
      tags:
      - Broadcast
      - Block
  /broadcast_transaction_with_callback:
    get:
      summary: 'WARNING: can only be used in Steem node or in scripts broadcast_transaction_with_callback'
      description: broadcast_transaction_with_callback
      operationId: broadcast-transaction-with-callback
      x-api-path-slug: broadcast-transaction-with-callback-get
      parameters:
      - in: query
        name: confirmationCallback
        description: confirmationCallback function
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - 'WARNING:'
      - Can
      - Only
      - Be
      - Used
      - In
      - Steem
      - Node
      - In
      - Scripts
      - Broadcast
      - Transaction
      - Callback
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