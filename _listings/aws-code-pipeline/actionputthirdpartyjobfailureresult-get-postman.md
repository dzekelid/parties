{
  "info": {
    "name": "AWS Code Pipeline API Put Third Party Job Failure Result",
    "_postman_id": "c766021a-8858-432d-9f96-131a1e3878dc",
    "description": "Represents the failure of a third party job as returned to the pipeline by a job\n            worker.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "4180d599-b469-4f2a-ac76-9bba4425cb02",
          "name": "acknowledgeJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeJob?DryRun=DryRun&jobId=jobId&nonce=nonce&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a specified job and whether that job has been received by\n            the job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba9918ef-6bb0-46d7-baad-86672b8b7055"
            }
          ]
        },
        {
          "id": "49ad3f0e-1905-4770-ae0b-185dd31642b9",
          "name": "acknowledgeThirdPartyJob",
          "request": {
            "url": "http://example.com/api/?Action=AcknowledgeThirdPartyJob?clientToken=clientToken&DryRun=DryRun&jobId=jobId&nonce=nonce&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Confirms a job worker has received the specified job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62d5650d-b6ef-415e-b7e7-e0eb4991c5f7"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "d8c315ea-dc23-43fe-ab55-c82c0da59529",
          "name": "createCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=CreateCustomActionType?Attribute=Attribute&category=category&configurationProperties=configurationProperties&DryRun=DryRun&inputArtifactDetails=inputArtifactDetails&outputArtifactDetails=outputArtifactDetails&provider=provider&settings=settings&SnapshotId=SnapshotId&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new custom action that can be used in all pipelines associated with the\n            AWS account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7f5a5c3-e6fc-486f-9d6b-9efc19a81534"
            }
          ]
        },
        {
          "id": "0e7b6dab-3d92-48c2-bae6-9fe0c0bf26e6",
          "name": "deleteCustomActionType",
          "request": {
            "url": "http://example.com/api/?Action=DeleteCustomActionType?Attribute=Attribute&category=category&DryRun=DryRun&provider=provider&version=version&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a custom action as deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e23f3b6-bdc3-4472-a6fe-c9351e6bbb73"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "7eb05232-d09e-451b-afcc-bb7c1c4c0dd7",
          "name": "createPipeline",
          "request": {
            "url": "http://example.com/api/?Action=CreatePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&Owner.N=Owner.N&pipeline=pipeline&RestorableBy.N=RestorableBy.N&SnapshotId.N=SnapshotId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5ed20557-6291-4093-8461-6d540c0a8c85"
            }
          ]
        },
        {
          "id": "b0245cb1-0786-4155-89b4-5d0f6b8a4962",
          "name": "deletePipeline",
          "request": {
            "url": "http://example.com/api/?Action=DeletePipeline?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&name=name&NextToken=NextToken&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the specified pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82380c10-7b16-4438-a4d6-f038b049b37f"
            }
          ]
        },
        {
          "id": "591b02b6-685b-442f-aa09-5eb63036d67e",
          "name": "getPipeline",
          "request": {
            "url": "http://example.com/api/?Action=GetPipeline?Attribute=Attribute&CreateVolumePermission=CreateVolumePermission&DryRun=DryRun&name=name&OperationType=OperationType&SnapshotId=SnapshotId&UserGroup.N=UserGroup.N&UserId.N=UserId.N&version=version",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the metadata, structure, stages, and actions of a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "45dc5948-6fc6-4cb2-bf66-c96581a31062"
            }
          ]
        },
        {
          "id": "ba3ccfdb-f9e6-4053-b80d-a94889d871a2",
          "name": "getPipelineExecution",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineExecution?AutoEnableIO=AutoEnableIO&DryRun=DryRun&pipelineExecutionId=pipelineExecutionId&pipelineName=pipelineName&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about an execution of a pipeline, including details about\n            artifacts, the pipeline execution ID, and the name, version, and status of the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b70124b-5635-4a45-9ee5-919a80c7793c"
            }
          ]
        },
        {
          "id": "e3d639c7-9fcb-49cf-9856-488969a551ac",
          "name": "getPipelineState",
          "request": {
            "url": "http://example.com/api/?Action=GetPipelineState?Attribute=Attribute&DryRun=DryRun&name=name&SnapshotId=SnapshotId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about the state of a pipeline, including the stages and\n            actions."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03cafd4a-7859-4e11-94a2-a303a1039372"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "4d91aa5e-330d-4a81-8263-9a09a44cd904",
          "name": "disableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=DisableStageTransition?DryRun=DryRun&Filter.N=Filter.N&MaxResults=MaxResults&NextToken=NextToken&pipelineName=pipelineName&reason=reason&stageName=stageName&transitionType=transitionType&VolumeId.N=VolumeId.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Prevents artifacts in a pipeline from transitioning to the next stage in the\n            pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e8b6a75-3f09-492b-999b-6c7d1fc4c4fb"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "908f981a-2c17-4dda-ab7b-6c984c6ee9d9",
          "name": "enableStageTransition",
          "request": {
            "url": "http://example.com/api/?Action=EnableStageTransition?Device=Device&DryRun=DryRun&Force=Force&InstanceId=InstanceId&pipelineName=pipelineName&stageName=stageName&transitionType=transitionType&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Enables artifacts in a pipeline to transition to a stage in a pipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e608aaa0-4015-461c-b81a-1c1fe716d118"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "7736e0e8-fa1b-4945-847c-d915465f5c64",
          "name": "getJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetJobDetails?DryRun=DryRun&jobId=jobId&VolumeId=VolumeId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "033061c4-0109-443e-95d3-842a2e67d7de"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "0dbb83fb-646c-4859-9770-48f847572630",
          "name": "getThirdPartyJobDetails",
          "request": {
            "url": "http://example.com/api/?Action=GetThirdPartyJobDetails?clientToken=clientToken&Domain=Domain&DryRun=DryRun&jobId=jobId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Requests the details of a job for a third party action."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "302864b3-99f8-473d-a137-fe53902a90b9"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "3b59e210-b830-42c2-ab87-43bd7d05f908",
          "name": "listActionTypes",
          "request": {
            "url": "http://example.com/api/?Action=ListActionTypes?actionOwnerFilter=actionOwnerFilter&AllocationId=AllocationId&AllowReassociation=AllowReassociation&DryRun=DryRun&InstanceId=InstanceId&NetworkInterfaceId=NetworkInterfaceId&nextToken=nextToken&PrivateIpAddress=PrivateIpAddress&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all AWS CodePipeline action types associated with your\n            account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4d4bbb17-e59e-46aa-9e65-2437b1caa341"
            }
          ]
        },
        {
          "id": "b903c828-626e-4987-9dd9-f1cffe2c4448",
          "name": "listPipelines",
          "request": {
            "url": "http://example.com/api/?Action=ListPipelines?AllocationId.N=AllocationId.N&DryRun=DryRun&Filter.N=Filter.N&nextToken=nextToken&PublicIp.N=PublicIp.N",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a summary of all of the pipelines associated with your account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "02b66995-361d-4b33-b05c-33e2d7047abc"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "aec16ca9-25ca-40c3-94e1-d950bcd5be0a",
          "name": "pollForJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForJobs?actionTypeId=actionTypeId&DryRun=DryRun&Filter.N=Filter.N&maxBatchSize=maxBatchSize&MaxResults=MaxResults&NextToken=NextToken&PublicIp.N=PublicIp.N&queryParam=queryParam",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about any jobs for AWS CodePipeline to act upon."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3a7afa9-af2d-4424-8609-10b1b25e093f"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "08916116-a8b1-408b-aeac-8c5f4235a74e",
          "name": "pollForThirdPartyJobs",
          "request": {
            "url": "http://example.com/api/?Action=PollForThirdPartyJobs?actionTypeId=actionTypeId&AssociationId=AssociationId&DryRun=DryRun&maxBatchSize=maxBatchSize&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Determines whether there are any third party jobs for a job worker to act on."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f05d15f-83dc-4251-b9f8-cc03e93141a0"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "87e50b91-8ca4-4a09-a4b6-dde20f9b8c61",
          "name": "putActionRevision",
          "request": {
            "url": "http://example.com/api/?Action=PutActionRevision?actionName=actionName&actionRevision=actionRevision&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&stageName=stageName",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides information to AWS CodePipeline about new revisions to a source."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85c5ac92-d290-4cfe-bce6-19b8fd9d2002"
            }
          ]
        },
        {
          "id": "21afb559-e47b-48e1-ac80-8f04f520c982",
          "name": "putApprovalResult",
          "request": {
            "url": "http://example.com/api/?Action=PutApprovalResult?actionName=actionName&AllocationId=AllocationId&DryRun=DryRun&pipelineName=pipelineName&PublicIp=PublicIp&result=result&stageName=stageName&token=token",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Provides the response to a manual approval request to AWS CodePipeline."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a8df88d-fc07-4c5f-9eb6-7b752ac25dcd"
            }
          ]
        },
        {
          "id": "f9f2e9fa-5ae5-4b15-be07-c4865aaff03f",
          "name": "putJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobFailureResult?DryRun=DryRun&failureDetails=failureDetails&jobId=jobId&PublicIp=PublicIp",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0fa3b3df-220d-4aba-a677-7a34c97b4601"
            }
          ]
        },
        {
          "id": "b7065eb2-cb0e-4374-bb4c-58c6f1628a3e",
          "name": "putJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutJobSuccessResult?continuationToken=continuationToken&currentRevision=currentRevision&executionDetails=executionDetails&Ipv6AddressCount=Ipv6AddressCount&Ipv6Addresses.N=Ipv6Addresses.N&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a job as returned to the pipeline by a job worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cf53e23-2b5c-4296-bd38-f57e4fa236e9"
            }
          ]
        },
        {
          "id": "6b4081df-d52a-48a2-b16a-8c77f5c1cb7d",
          "name": "putThirdPartyJobFailureResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobFailureResult?AllowReassignment=AllowReassignment&clientToken=clientToken&failureDetails=failureDetails&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId&PrivateIpAddress.N=PrivateIpAddress.N&SecondaryPrivateIpAddressCount=SecondaryPrivateIpAddressCount",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the failure of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "610fd7f4-0877-4465-a0d0-71068e1098fa"
            }
          ]
        }
      ]
    }
  ]
}