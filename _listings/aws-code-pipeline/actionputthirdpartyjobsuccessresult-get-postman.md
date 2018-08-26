{
  "info": {
    "name": "AWS Code Pipeline API Put Third Party Job Success Result",
    "_postman_id": "f078d0b6-4249-4848-9c7a-4a7c4bf951be",
    "description": "Represents the success of a third party job as returned to the pipeline by a job\n            worker.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "7476171f-7d34-4e10-af69-40b51b6fdb41",
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
              "id": "2f8f5cc2-6ea5-452c-95cb-dc46ea4f5078"
            }
          ]
        },
        {
          "id": "147902a9-b3aa-4211-a263-2deea23a9f3a",
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
              "id": "e2fc5cdb-1e72-49a8-88e7-827c9ddac445"
            }
          ]
        }
      ]
    },
    {
      "name": "Custom",
      "item": [
        {
          "id": "84f9700f-f591-4548-913e-b6a81936ff4c",
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
              "id": "99fd7aab-fbf8-467a-a432-2b1572d9a986"
            }
          ]
        },
        {
          "id": "bece68eb-0692-4e99-93fc-c74122b577ef",
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
              "id": "7cfe9435-5539-41a1-826d-24d18e393659"
            }
          ]
        }
      ]
    },
    {
      "name": "Pipeline",
      "item": [
        {
          "id": "409157f4-62c2-4756-9d72-93e1c9e30426",
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
              "id": "de087b4a-f279-46a9-a908-79768906e818"
            }
          ]
        },
        {
          "id": "f68d8598-aa24-4cd2-9e7d-63be071a9526",
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
              "id": "2c6d0064-badf-4eeb-a9b8-e02b2239d490"
            }
          ]
        },
        {
          "id": "42afbd04-4cf4-4403-8dbe-4162d68034d8",
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
              "id": "2c00465d-b30e-4061-b479-0db0eea65b1d"
            }
          ]
        },
        {
          "id": "05d13331-3fe6-4c9c-85f2-223781bcb970",
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
              "id": "588e6f58-8e29-44e4-8035-c2947a77c9c4"
            }
          ]
        },
        {
          "id": "32fcbb7e-b03c-42e1-aa8f-b948dcf989b6",
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
              "id": "2db4b2b5-7077-4d73-8aae-e60215dbcc15"
            }
          ]
        }
      ]
    },
    {
      "name": "Disable",
      "item": [
        {
          "id": "189e44b8-4c74-495b-bde2-ef6a1750089a",
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
              "id": "453db652-5841-4ae1-aa60-af1334534f54"
            }
          ]
        }
      ]
    },
    {
      "name": "Enable",
      "item": [
        {
          "id": "4a561d8c-0a2c-47d6-941b-22c9389e21be",
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
              "id": "28a18fb8-404f-48ec-9652-1b8b994f9e6a"
            }
          ]
        }
      ]
    },
    {
      "name": "Job",
      "item": [
        {
          "id": "874c7726-56db-4f87-8a50-e6313c788028",
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
              "id": "c4053ff6-8695-4c4d-ac15-46f72fdf4428"
            }
          ]
        }
      ]
    },
    {
      "name": "Third",
      "item": [
        {
          "id": "77fbb63b-009d-4c07-8630-b6f5d77f6fda",
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
              "id": "af4da1cb-9681-4c89-b979-50407e28e0ef"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "330b2f1d-9be5-43e9-a23e-59fd94fb1ae9",
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
              "id": "f61d052f-518d-4cd7-a47c-e03233148e7b"
            }
          ]
        },
        {
          "id": "9e9d81ea-d03c-40a5-afe8-434369deb944",
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
              "id": "92fb9d6d-b9c9-4d9d-b393-d997691c212b"
            }
          ]
        }
      ]
    },
    {
      "name": "PollJobs",
      "item": [
        {
          "id": "cae3cdf2-b923-48a0-a1e7-00dfee8345e2",
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
              "id": "79610dc8-dedf-4e12-bcde-3dc10a1e11a1"
            }
          ]
        }
      ]
    },
    {
      "name": "PollThird",
      "item": [
        {
          "id": "4950844e-e494-44e3-992a-56029208de46",
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
              "id": "cd3537e8-4450-48c3-b595-6e7a7dc7bb3a"
            }
          ]
        }
      ]
    },
    {
      "name": "Put",
      "item": [
        {
          "id": "75d72928-fd96-4160-9b48-41b10f27ba87",
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
              "id": "6c69a397-c72f-4887-b93d-2763723ea30b"
            }
          ]
        },
        {
          "id": "fa725e49-bda7-4a9b-89e5-b6ce1971b004",
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
              "id": "35e30e55-c31f-42a5-80df-088509e46f0b"
            }
          ]
        },
        {
          "id": "7562b4ec-2bb2-4224-b23a-0eae7fffdc47",
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
              "id": "59c75cf2-5ebb-4622-a15d-46da88d53994"
            }
          ]
        },
        {
          "id": "ea9785ad-2ead-4b2c-8683-06bbf8ca45ee",
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
              "id": "faabc400-e56b-43ce-85b9-09c2ac4add10"
            }
          ]
        },
        {
          "id": "ee57cbf9-7b83-4411-8c8a-5b8dacbf3495",
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
              "id": "8edf5c89-aec4-4695-8560-013ed05b4b39"
            }
          ]
        },
        {
          "id": "92d59d8d-ea8f-40ab-b934-b0ed7419cbc5",
          "name": "putThirdPartyJobSuccessResult",
          "request": {
            "url": "http://example.com/api/?Action=PutThirdPartyJobSuccessResult?clientToken=clientToken&continuationToken=continuationToken&currentRevision=currentRevision&DeviceIndex=DeviceIndex&DryRun=DryRun&executionDetails=executionDetails&InstanceId=InstanceId&jobId=jobId&NetworkInterfaceId=NetworkInterfaceId",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Represents the success of a third party job as returned to the pipeline by a job\n            worker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6354a87a-9488-4051-84d0-465c7c71c9ed"
            }
          ]
        }
      ]
    }
  ]
}