{
  "info": {
    "name": "Zencoder API Get Usage for Live",
    "_postman_id": "2920d5e2-254a-4d93-a13c-e4c2e5375c52",
    "description": "Get Usage for Live",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "29fd046c-a478-40f2-85ff-0059a758dc2e",
          "name": "getAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Account Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7e2c4bc-0b95-411c-9666-595135fc6243"
            }
          ]
        },
        {
          "id": "fe798029-4ad1-4bcc-8dc3-99a20a877951",
          "name": "postAccount",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account?email=%7B%7D&password=%7B%7D&password_confirmation=%7B%7D&terms_of_service=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an Account"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "277ace30-2edc-4bd3-a31f-e9be38efd212"
            }
          ]
        },
        {
          "id": "ac340526-88d6-475d-b261-f728aa050ce1",
          "name": "putAccountIntegration",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/integration?api_key=%7B%7D",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9d1fdd9f-5324-45e5-bea9-7a3443fb3967"
            }
          ]
        },
        {
          "id": "6a58a4cf-5ef3-41e6-9bd8-75afef2d67df",
          "name": "putAccountLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/account/live",
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Integration Mode - Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55cb53b0-131f-44c3-bb7c-8ae1e116028d"
            }
          ]
        }
      ]
    },
    {
      "name": "Inputs",
      "item": [
        {
          "id": "083e4762-7cf8-4321-87e4-a37316714aef",
          "name": "getInupdatesInupdate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Input Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6454615b-7f02-44c9-b452-df9ef89cfa94"
            }
          ]
        },
        {
          "id": "3a13d08c-b243-4295-bd67-8ec258121e5d",
          "name": "getInupdatesInupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "inputs/:input_id/progress"
              ],
              "variable": [
                {
                  "id": "input_id",
                  "value": "input_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaaf2e19-587c-446e-90c0-f307094aeb5f"
            }
          ]
        }
      ]
    },
    {
      "name": "Jobs",
      "item": [
        {
          "id": "89009fe7-0f48-4dd0-ab2b-e06ec0d528ab",
          "name": "getJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "A list of jobs can be obtained by sending an HTTP GET request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1024407-96c6-4849-b54d-69eb527ee3f9"
            }
          ]
        },
        {
          "id": "68f29154-9305-4df1-8c33-2364e13638be",
          "name": "postJobs",
          "request": {
            "url": "http://app.zencoder.com/api/v2/jobs?api_key=%7B%7D&Encoding Settings=%7B%7D&input=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Encoding jobs are created by sending an HTTP POST request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de458325-f08b-4ffc-a91d-cac8055beaba"
            }
          ]
        },
        {
          "id": "b9a2a076-9c9e-4212-b43f-5eb6ea067d71",
          "name": "getJobsJob",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "Get Job Details",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Job Details"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8cd65134-cfa5-4617-a0e2-e64d76e5f56a"
            }
          ]
        },
        {
          "id": "518f83e7-e6b9-400d-8f61-9194502b83e7",
          "name": "putJobsJobCancel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/cancel"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If you wish to cancel a job that has not yet finished processing you may send a request."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89373591-c748-459f-b1e4-e565dcf42cdd"
            }
          ]
        },
        {
          "id": "b8c4c421-50f4-4e34-846e-28443e543238",
          "name": "putJobsJobFinish",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/finish"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Finishes the input on a Live streaming job."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32df5cb1-902a-4140-81fb-f53585cc274f"
            }
          ]
        },
        {
          "id": "f3ef8be7-c705-48f8-919e-ff0fa0851c09",
          "name": "getJobsJobProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/progress"
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "job_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, input, outputs, and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a50255ea-ce08-4521-994c-20bb3c32e21a"
            }
          ]
        },
        {
          "id": "5cab1ae6-6729-416e-83f2-77ea63fdc015",
          "name": "putJobsJobResubmit",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "jobs/:job_id/resubmit"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "job_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "If a job has failed processing you may request that it be attempted again."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "006adae9-d0e7-44ac-a205-807e9dc4f15a"
            }
          ]
        }
      ]
    },
    {
      "name": "Outputs",
      "item": [
        {
          "id": "c554a270-de62-42c7-8909-09624b135608",
          "name": "getOutupdatesOutupdateProgress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.zencoder.com",
              "path": [
                "api",
                "v2",
                "outputs/:output_id/progress"
              ],
              "query": [
                {
                  "key": "api_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "callback",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "output_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The return will contain one or more of the following keys: state, current_event, current_event_progress and progress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a15b6b30-ddad-4530-aa40-3f71a4a9cbc1"
            }
          ]
        }
      ]
    },
    {
      "name": "Reports",
      "item": [
        {
          "id": "b21a757a-aa3c-4ff4-9dae-6d5b5311ff54",
          "name": "getReportsAll",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/all?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for VOD & Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2417b27-ba0f-4280-98d2-5271349ca6e2"
            }
          ]
        },
        {
          "id": "5016e21f-7369-4f50-9f03-0c7c44dd232a",
          "name": "getReportsLive",
          "request": {
            "url": "http://app.zencoder.com/api/v2/reports/live?api_key=%7B%7D&from=%7B%7D&grouping=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get Usage for Live"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aca49156-e242-4a61-9c99-f38da4c48c54"
            }
          ]
        }
      ]
    }
  ]
}