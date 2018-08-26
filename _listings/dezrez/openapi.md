---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/offeraccepted:
    post:
      summary: Generates a correspondence any parties of the acceptance of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the acceptance of an
        offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferAcceptedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferaccepted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Acceptance
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerrejected:
    post:
      summary: Generates a correspondence any parties of the rejection of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the rejection of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferRejectedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferrejected-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Rejection
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerwithdrawn:
    post:
      summary: Generates a correspondence to notify any parties of the withdrawl of
        an offer.  Uses default values where possible.
      description: Generates a correspondence to notify any parties of the withdrawl
        of an offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferwithdrawnLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferwithdrawn-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Withdrawl
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/completed:
    post:
      summary: Generates a correspondence to notify any parties of completion.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of completion.  uses
        default values where possible..
      operationId: DocumentGeneration_CompletedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcompleted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Completion
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/exchanged:
    post:
      summary: Generates a correspondence to notify any parties of exchanged.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of exchanged.  uses
        default values where possible..
      operationId: DocumentGeneration_ExchangedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationexchanged-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Exchanged
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/confirmationofviewing:
    post:
      summary: Generates a correspondence to notify all parties of a scheduled viewing.  Uses
        default values where possible.
      description: Generates a correspondence to notify all parties of a scheduled
        viewing.  uses default values where possible..
      operationId: DocumentGeneration_ConfirmationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - ""
      - Parties
      - Of
      - Scheduled
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/cancellationofviewing:
    post:
      summary: Generates a correspondence to notify parties of a cancellation of a
        viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties of a cancellation
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_CancellationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancellationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Of
      - Cancellation
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/reschedulingofviewing:
    post:
      summary: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties involved of a rescheduling
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_ReschedulingOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulingofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Involved
      - Of
      - Rescheduling
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/job/SendSystemEmail:
    post:
      summary: Sends a basic email to any specified party.
      description: Sends a basic email to any specified party..
      operationId: Job_SendSystemEmailBysendSystemEmail
      x-api-path-slug: apijobsendsystememail-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendSystemEmail
        description: The send system email
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Basic
      - Email
      - To
      - Any
      - Specified
      - Party
---