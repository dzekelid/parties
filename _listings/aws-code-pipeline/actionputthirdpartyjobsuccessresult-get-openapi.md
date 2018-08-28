---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API Put Third Party Job Success Result
  version: 1.0.0
  description: |-
    Represents the success of a third party job as returned to the pipeline by a job
                worker.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcknowledgeThirdPartyJob:
    get:
      summary: Acknowledge Third Party Job
      description: Confirms a job worker has received the specified job.
      operationId: acknowledgeThirdPartyJob
      x-api-path-slug: actionacknowledgethirdpartyjob-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID of the job
        type: string
      - in: query
        name: nonce
        description: A system-generated random number that AWS CodePipeline uses to
          ensure that the job            is being worked on by only one job worker
        type: string
      - in: query
        name: VolumeId
        description: The ID of the volume
        type: string
      responses:
        200:
          description: OK
      tags:
      - Acknowledge
      - Third
      - Party
      - Job
  /?Action=GetThirdPartyJobDetails:
    get:
      summary: Get Third Party Job Details
      description: Requests the details of a job for a third party action.
      operationId: getThirdPartyJobDetails
      x-api-path-slug: actiongetthirdpartyjobdetails-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: Domain
        description: Set to vpc to allocate the address for use with instances in
          a VPC
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: jobId
        description: The unique system-generated ID used for identifying the job
        type: string
      responses:
        200:
          description: OK
      tags:
      - Third
      - Party
      - Job
      - Details
  /?Action=PollForThirdPartyJobs:
    get:
      summary: Poll For Third Party Jobs
      description: Determines whether there are any third party jobs for a job worker
        to act on.
      operationId: pollForThirdPartyJobs
      x-api-path-slug: actionpollforthirdpartyjobs-get
      parameters:
      - in: query
        name: actionTypeId
        description: Represents information about an action type
        type: string
      - in: query
        name: AssociationId
        description: '[EC2-VPC] The association ID'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: maxBatchSize
        description: The maximum number of jobs to return in a poll for jobs call
        type: string
      - in: query
        name: PublicIp
        description: '[EC2-Classic] The Elastic IP address'
        type: string
      responses:
        200:
          description: OK
      tags:
      - PollThird
      - Party
      - Jobs
  /?Action=PutThirdPartyJobFailureResult:
    get:
      summary: Put Third Party Job Failure Result
      description: |-
        Represents the failure of a third party job as returned to the pipeline by a job
                    worker.
      operationId: putThirdPartyJobFailureResult
      x-api-path-slug: actionputthirdpartyjobfailureresult-get
      parameters:
      - in: query
        name: AllowReassignment
        description: Indicates whether to allow an IP address that is already assigned
          to another network interface or instance to be reassigned to the specified
          network interface
        type: string
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: failureDetails
        description: Represents information about failure details
        type: string
      - in: query
        name: jobId
        description: The ID of the job that failed
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      - in: query
        name: PrivateIpAddress.N
        description: One or more IP addresses to be assigned as a secondary private
          IP address to the network interface
        type: string
      - in: query
        name: SecondaryPrivateIpAddressCount
        description: The number of secondary IP addresses to assign to the network
          interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Third
      - Party
      - Job
      - Failure
      - Result
  /?Action=PutThirdPartyJobSuccessResult:
    get:
      summary: Put Third Party Job Success Result
      description: |-
        Represents the success of a third party job as returned to the pipeline by a job
                    worker.
      operationId: putThirdPartyJobSuccessResult
      x-api-path-slug: actionputthirdpartyjobsuccessresult-get
      parameters:
      - in: query
        name: clientToken
        description: The clientToken portion of the clientId and clientToken pair
          used to verify that            the calling entity is allowed access to the
          job and its details
        type: string
      - in: query
        name: continuationToken
        description: A token generated by a job worker, such as an AWS CodeDeploy
          deployment ID, that a            successful job provides to identify a partner
          action in progress
        type: string
      - in: query
        name: currentRevision
        description: Represents information about a current revision
        type: string
      - in: query
        name: DeviceIndex
        description: The index of the device for the network interface attachment
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: executionDetails
        description: The details of the actions taken and results produced on an artifact
          as it passes            through stages in the pipeline
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: jobId
        description: The ID of the job that successfully completed
        type: string
      - in: query
        name: NetworkInterfaceId
        description: The ID of the network interface
        type: string
      responses:
        200:
          description: OK
      tags:
      - Put
      - Third
      - Party
      - Job
      - Success
      - Result
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