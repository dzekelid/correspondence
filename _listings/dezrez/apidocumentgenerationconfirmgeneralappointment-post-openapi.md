---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a confirm general appointment letter correspondence
  version: 1.0.0
  description: Generates a confirm general appointment letter correspondence.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/custompack:
    post:
      summary: Generates any correspondence and can allow you to overpost information
        to the correspondence
      description: Generates any correspondence and can allow you to overpost information
        to the correspondence.
      operationId: DocumentGeneration_GeneratePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcustompack-post
      parameters:
      - in: body
        name: generatePackDetails
        description: broad contract that allows for overposting and underposting,
          however you must specify a correspondence Id            you must then follow
          the validation rules for the for that individual correspondence type, each
          route to the controller is named in the same way            as the enumerated
          correspondence type system name, and the mappings for the specific class
          to the GeneratePackJobDataContract are detailed in             the each
          individual simplified contract
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
      - Any
      - Correspondence
      - Can
      - Ow
      - You
      - To
      - Overpost
      - Information
      - To
      - Correspondence
  /api/documentgeneration/boardordernew:
    post:
      summary: Generates an board ordering New correspondence
      description: Generates an board ordering new correspondence.
      operationId: DocumentGeneration_BoardOrderingNewPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordernew-post
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
      - Board
      - Ordering
      - New
      - Correspondence
  /api/documentgeneration/boardorderreplace:
    post:
      summary: Generates an board ordering Replace correspondence
      description: Generates an board ordering replace correspondence.
      operationId: DocumentGeneration_BoardOrderReplacePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderreplace-post
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
      - Board
      - Ordering
      - Replace
      - Correspondence
  /api/documentgeneration/boardordertakedown:
    post:
      summary: Generates an board ordering Takedown correspondence
      description: Generates an board ordering takedown correspondence.
      operationId: DocumentGeneration_BoardOrderTakedownPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardordertakedown-post
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
      - Board
      - Ordering
      - Takedown
      - Correspondence
  /api/documentgeneration/boardorderupdate:
    post:
      summary: Generates an board ordering Update correspondence
      description: Generates an board ordering update correspondence.
      operationId: DocumentGeneration_BoardOrderUpdatePackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationboardorderupdate-post
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
      - Board
      - Ordering
      - ""
      - Correspondence
  /api/documentgeneration/confirmvaluation:
    post:
      summary: Generates a correspondence confirming the booking of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the booking of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationConfirmationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmvaluation-post
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
      - Confirming
      - Booking
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/valuationresult:
    post:
      summary: Generates a correspondence confirming the result of a valuation appointment.  Uses
        default values where possible.
      description: Generates a correspondence confirming the result of a valuation
        appointment.  uses default values where possible..
      operationId: DocumentGeneration_GenerateValuationResultLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationresult-post
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
      - Confirming
      - Result
      - Of
      - Valuation
      - Appointment
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/instruction:
    post:
      summary: Generates a Instruction letter correspondence to the vendor of a particular
        marketing role
      description: Generates a instruction letter correspondence to the vendor of
        a particular marketing role.
      operationId: DocumentGeneration_GenerateInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationinstruction-post
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
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/tenancyagreementast:
    post:
      summary: Generates Tenancy Agreement correspondence
      description: Generates tenancy agreement correspondence.
      operationId: DocumentGeneration_TenancyAgreementASTBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationtenancyagreementast-post
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
      - Tenancy
      - Agreement
      - Correspondence
  /api/documentgeneration/tenancyguarantor:
    post:
      summary: Generates Tenancy Guarantor correspondence
      description: Generates tenancy guarantor correspondence.
      operationId: DocumentGeneration_TenancyGuarantorBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationtenancyguarantor-post
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
      - Tenancy
      - Guarantor
      - Correspondence
  /api/documentgeneration/withdrawninstruction:
    post:
      summary: Generates a Withdrawn Instruction letter correspondence to the vendor
        of a particular marketing role
      description: Generates a withdrawn instruction letter correspondence to the
        vendor of a particular marketing role.
      operationId: DocumentGeneration_GenerateWithdrawnInstructionLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationwithdrawninstruction-post
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
      - Withdrawn
      - Instruction
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/reschedulevaluation:
    post:
      summary: Generates a Reschedule Valuation letter correspondence
      description: Generates a reschedule valuation letter correspondence.
      operationId: DocumentGeneration_RescheduleValuationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulevaluation-post
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
      - Reschedule
      - Valuation
      - Letter
      - Correspondence
  /api/documentgeneration/valuationlost:
    post:
      summary: Generates a Valuation Lost letter correspondence to the vendor of a
        particular marketing role
      description: Generates a valuation lost letter correspondence to the vendor
        of a particular marketing role.
      operationId: DocumentGeneration_GenerateValuationLostLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationvaluationlost-post
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
      - Valuation
      - Lost
      - Letter
      - Correspondence
      - To
      - Vendor
      - Of
      - Particular
      - Marketing
      - Role
  /api/documentgeneration/rescheduleepcappointment:
    post:
      summary: Generates a EPC Appointment letter correspondence
      description: Generates a epc appointment letter correspondence.
      operationId: DocumentGeneration_RescheduleEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationrescheduleepcappointment-post
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
      - EPC
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/reschedulemeeting:
    post:
      summary: Generates a meeting letter correspondence
      description: Generates a meeting letter correspondence.
      operationId: DocumentGeneration_ReschedulMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationreschedulemeeting-post
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
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/cancelvaluation:
    post:
      summary: Generates a cancel a valuation letter correspondence
      description: Generates a cancel a valuation letter correspondence.
      operationId: DocumentGeneration_CancelValuationLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelvaluation-post
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
      - Cancel
      - Valuation
      - Letter
      - Correspondence
  /api/documentgeneration/cancelepcappointment:
    post:
      summary: Generates a cancel an epc appointment letter correspondence
      description: Generates a cancel an epc appointment letter correspondence.
      operationId: DocumentGeneration_CancelEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelepcappointment-post
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
      - Cancel
      - Epc
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/confirmepcappointment:
    post:
      summary: Generates a confirm an epc appointment letter correspondence
      description: Generates a confirm an epc appointment letter correspondence.
      operationId: DocumentGeneration_ConfirmEpcAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmepcappointment-post
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
      - Confirm
      - Epc
      - Appointment
      - Letter
      - Correspondence
  /api/documentgeneration/cancelmeeting:
    post:
      summary: Generates a cancel a meeting letter correspondence
      description: Generates a cancel a meeting letter correspondence.
      operationId: DocumentGeneration_CancelMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancelmeeting-post
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
      - Cancel
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/confirmmeeting:
    post:
      summary: Generates a confirm a meeting letter correspondence
      description: Generates a confirm a meeting letter correspondence.
      operationId: DocumentGeneration_ConfirmMeetingLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmmeeting-post
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
      - Confirm
      - Meeting
      - Letter
      - Correspondence
  /api/documentgeneration/confirmgeneralappointment:
    post:
      summary: Generates a confirm general appointment letter correspondence
      description: Generates a confirm general appointment letter correspondence.
      operationId: DocumentGeneration_ConfirmGeneralAppointmentLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmgeneralappointment-post
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
      - Confirm
      - General
      - Appointment
      - Letter
      - Correspondence
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