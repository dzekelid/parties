{
  "info": {
    "name": "Open Bank Project Get Party",
    "_postman_id": "0a1adc2a-e090-4f52-920a-6843457179a0",
    "description": "Get Party",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Banking",
      "item": [
        {
          "id": "4f7ee629-5618-477f-bb6f-61102ecf8729",
          "name": "CreateAccountRequest",
          "request": {
            "url": "{{default}}/account-requests?No Name=%7B%7D",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4ab5442-7081-4b6c-b436-dc99d1c28381"
            }
          ]
        },
        {
          "id": "fe370655-7672-496b-8428-2c47ae89a767",
          "name": "GetAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d702f57b-3908-4ca6-80a6-3731764100a7"
            }
          ]
        },
        {
          "id": "76fd1b59-69c8-4886-a376-8635e0954580",
          "name": "DeleteAccountRequest",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "account-requests/:AccountRequestId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountRequestId",
                  "value": "AccountRequestId",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete an account request"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b55c620-81af-45e0-b543-f18ec58f34c0"
            }
          ]
        },
        {
          "id": "959483b8-8b9d-4d28-85c4-4f5889b48b87",
          "name": "GetAccounts",
          "request": {
            "url": "{{default}}/accounts?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of accounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6b8d70b-023d-47df-9b51-c853ed81c559"
            }
          ]
        },
        {
          "id": "492a4db6-0cb3-4a64-a46e-4a4400e3b9ce",
          "name": "GetAccount",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56cf4323-328e-41ec-b70a-d14d6031de16"
            }
          ]
        },
        {
          "id": "a71d5cc3-ac65-4566-9d01-34e8e7465af8",
          "name": "GetAccountTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "39b1e4a0-73bb-405e-aae7-4c641a0811a1"
            }
          ]
        },
        {
          "id": "5548783b-d7c6-4ff4-875f-a84982604523",
          "name": "GetAccountBeneficiaries",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/beneficiaries"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbbf5a81-4c71-48a6-97fd-b5cc16611439"
            }
          ]
        },
        {
          "id": "2fce6b74-0b88-49ac-84fa-2002f45805a2",
          "name": "GetAccountBalances",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/balances"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b5380c1-3354-4c3d-83c6-c8a2e03be468"
            }
          ]
        },
        {
          "id": "770b9ff1-6940-4e20-8af4-bde129a011d0",
          "name": "GetAccountDirectDebits",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/direct-debits"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7ce277e-157a-4853-8a7a-8de3bdb9f2d0"
            }
          ]
        },
        {
          "id": "7e001713-93d3-4792-86db-4e7d8525cc62",
          "name": "GetAccountStandingOrders",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/standing-orders"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3633681f-bbc0-492c-9af5-85e13c3fd9b0"
            }
          ]
        },
        {
          "id": "b18e9d4e-10ca-43ec-956c-b190f4879a89",
          "name": "GetAccountProduct",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/product"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Product related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "731f788d-d369-4b7a-8352-b2d9164d879b"
            }
          ]
        },
        {
          "id": "f429c9fa-3621-496e-bdc0-46a2c0799927",
          "name": "GetAccountOffers",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/offers"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ab9b5b4-a641-4651-8026-4eb2c8b7df24"
            }
          ]
        },
        {
          "id": "ba22629e-4233-473c-a29a-fcdc522b31fa",
          "name": "GetAccountParty",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/party"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e54bb0d-d6fc-4e05-8494-65b72ca85406"
            }
          ]
        },
        {
          "id": "963ff091-e537-4543-a3ea-c92ca2413fc0",
          "name": "GetAccountScheduledPayments",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/scheduled-payments"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7b6e9662-ff98-483e-b9f6-8e135e0ede94"
            }
          ]
        },
        {
          "id": "ac3f06f2-9b84-40dc-a99f-d0e89d6c2ba5",
          "name": "GetAccountStatements",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e3c06f1-0da5-4669-bb97-c805b102d19e"
            }
          ]
        },
        {
          "id": "0d691882-2d55-4d11-9c6f-c109a33f0f52",
          "name": "GetAccountStatement",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7a0680a-67b1-4e21-ba64-8074c2030cdc"
            }
          ]
        },
        {
          "id": "dfd2a891-f7a0-4aee-be9d-d8ef17e88f41",
          "name": "GetAccountStatementFile",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/file"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement File related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "388403d4-c7e7-4ad8-9ce1-aa6989f0b8c0"
            }
          ]
        },
        {
          "id": "88066448-c155-4c87-89bc-ce9d531c8769",
          "name": "GetAccountStatementTransactions",
          "request": {
            "url": {
              "host": "{{default}}",
              "path": [
                "accounts/:AccountId/statements/:StatementId/transactions"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "AccountId",
                  "value": "AccountId",
                  "type": "string"
                },
                {
                  "id": "StatementId",
                  "value": "StatementId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statement Transactions related to an account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5007e145-2604-4764-961d-e403ab8ed351"
            }
          ]
        },
        {
          "id": "5e03b1a9-d915-4ece-b325-b83b001837f6",
          "name": "GetStandingOrders",
          "request": {
            "url": "{{default}}/standing-orders?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Standing Orders"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6a032a6-51a4-4bb9-9b08-ed5ac030b7c7"
            }
          ]
        },
        {
          "id": "b60d56e9-d65d-4301-add9-0a8b8ae43960",
          "name": "GetDirectDebits",
          "request": {
            "url": "{{default}}/direct-debits?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Direct Debits"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6fcd7c5d-1e09-4215-b786-21d4b505c27c"
            }
          ]
        },
        {
          "id": "c8d00857-4405-48c8-acbc-76288294300b",
          "name": "GetBeneficiaries",
          "request": {
            "url": "{{default}}/beneficiaries?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Beneficiaries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c34a8909-8975-408d-b95f-92e45245129f"
            }
          ]
        },
        {
          "id": "2a5a575e-11e7-4fec-ab6a-8a002cd21f7f",
          "name": "GetTransactions",
          "request": {
            "url": "{{default}}/transactions?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Transactions"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7139e8c6-5153-4e11-b14f-0dd7e60e23da"
            }
          ]
        },
        {
          "id": "1ef0d44c-35d4-451b-a458-3652e4cce13f",
          "name": "GetBalances",
          "request": {
            "url": "{{default}}/balances?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Balances"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a3a88c9e-c219-436a-ac7e-e578ba164192"
            }
          ]
        },
        {
          "id": "10044076-01b1-4968-862c-1460c1115a53",
          "name": "GetProducts",
          "request": {
            "url": "{{default}}/products?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Products"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c8b3eb65-5d0f-4528-b737-90d29812a3ac"
            }
          ]
        },
        {
          "id": "5176d524-b039-4f89-855c-a0e1743c2aea",
          "name": "GetOffers",
          "request": {
            "url": "{{default}}/offers?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Offers"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "22eadc49-700b-42cf-ac21-1d527f4d365b"
            }
          ]
        },
        {
          "id": "18a794c5-2c94-4dfc-9fda-fc3b91ed7303",
          "name": "GetParty",
          "request": {
            "url": "{{default}}/party?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Party"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98f0b872-c9e8-4407-a775-f8fd0c48d518"
            }
          ]
        },
        {
          "id": "40fec1e1-6206-456e-b657-9d0834eadf0f",
          "name": "GetScheduledPayments",
          "request": {
            "url": "{{default}}/scheduled-payments?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Scheduled Payments"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8fb283f-39bd-4ce4-aa3e-8be468a237e7"
            }
          ]
        },
        {
          "id": "83cf6173-7e3a-47f4-85c0-7e9564fd1f31",
          "name": "GetStatements",
          "request": {
            "url": "{{default}}/statements?No Name=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Statements"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd576c6f-f13b-4faf-876f-b700c82cfa91"
            }
          ]
        }
      ]
    }
  ],
  "variable": [
    {
      "key": "default",
      "value": "http://www.example.com/open-banking/v2.0"
    }
  ]
}