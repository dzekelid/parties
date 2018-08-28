{
  "info": {
    "name": "AWS Code Pipeline API Acknowledge Third Party Job",
    "_postman_id": "71fa3d79-dc07-4dd3-8b59-c6daad16ab9d",
    "description": "Confirms a job worker has received the specified job.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Acknowledge",
      "item": [
        {
          "id": "82cda1a8-970b-40ea-a504-e38c28e83ef4",
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
              "id": "6e1d2331-b90c-49ad-972d-f71911cd98db"
            }
          ]
        },
        {
          "id": "0eb70882-2f2c-4396-b87b-a939c1c8793b",
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
              "id": "ae922959-3997-46b7-b561-0adf0dfa9c90"
            }
          ]
        }
      ]
    }
  ]
}