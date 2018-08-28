---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Queries the demographics store for
    matching parties, with the query parameters specified in the URL.
  description: Queries the demographics store for matching parties, with the query
    parameters specified in the url..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
paths:
  /demographics/ehr/{ehrId}/party:
    get:
      summary: Retrieves the demographics info for the specified party.
      description: Retrieves the demographics info for the specified party..
      operationId: getPartyByEhrId
      x-api-path-slug: demographicsehrehridparty-get
      parameters:
      - in: path
        name: ehrId
        description: EHR ID of the party to retrieve
      - in: query
        name: when
        description: The instant of time for which to return the information about
          the party in the ISO-8601 format (2014-03-03T15:05:43
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Ehr
      - EhrId
      - Party
  /demographics/party:
    post:
      summary: Creates a new party record in the remote demographics store.
      description: Creates a new party record in the remote demographics store..
      operationId: addParty
      x-api-path-slug: demographicsparty-post
      parameters:
      - in: body
        name: body
        description: The party to create in whatever format the demographics service
          supports
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
    put:
      summary: Updates a party record in the remote demographics store.
      description: Updates a party record in the remote demographics store..
      operationId: updateParty
      x-api-path-slug: demographicsparty-put
      parameters:
      - in: body
        name: body
        description: The party to update
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
  /demographics/party/query:
    get:
      summary: Queries the demographics store for matching parties, with the query
        parameters specified in the URL.
      description: Queries the demographics store for matching parties, with the query
        parameters specified in the url..
      operationId: queryParties
      x-api-path-slug: demographicspartyquery-get
      parameters:
      - in: query
        name: maxHits
        description: Limit the query results to this many hits
      - in: query
        name: parameters
        description: Query parameters in the key1=value1&key2=value2 format
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - Query
    post:
      summary: Queries the demographics store for matching parties.
      description: Queries the demographics store for matching parties..
      operationId: queryParties
      x-api-path-slug: demographicspartyquery-post
      parameters:
      - in: body
        name: body
        description: An array of key-value query criteria
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: maxHits
        description: Limit the query results to this many hits
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - Query
  /demographics/party/{partyId}:
    delete:
      summary: Deletes a party record from the remote demographics store.
      description: Deletes a party record from the remote demographics store..
      operationId: deleteParty
      x-api-path-slug: demographicspartypartyid-delete
      parameters:
      - in: path
        name: partyId
        description: The id of the party to delete
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - PartyId
    get:
      summary: Retrieves the demographics info for the specified party.
      description: Retrieves the demographics info for the specified party..
      operationId: getParty
      x-api-path-slug: demographicspartypartyid-get
      parameters:
      - in: path
        name: partyId
        description: The external ID of the party to retrieve
      - in: query
        name: when
        description: The instant of time for which to return the information about
          the party in the ISO-8601 format (2014-03-03T15:05:43
      responses:
        200:
          description: OK
      tags:
      - Demographics
      - Party
      - PartyId
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