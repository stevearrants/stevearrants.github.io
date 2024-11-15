# Request Body[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-body_1)

The body of the request must contain:

{

"name": "{connectorName}",

"version": "{connectorVersion}"

}

where

- {connectorName}: The name of the connector
- {connectorVersion}: The version of the connector

## Response[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#response_1)

The body of the response will contain a JSON string with the IDs, key, and secret required for the connector manifest file. For example:

{

"status": true,

"operation": "Register a connector",

"id": "4471",

"key": "6d093654-d...2-10cad6797d6e",

"secret": "3673e11b-f...d-5e3f3ad796d5",

"endpointEntityId": "2370701",

"functionEntityStartId": "2370702",

"functionEntityEndId": "2370800"

}

## List registered connectors[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#list-registered-connectors)

Lists all custom connectors (those created with either the Connector SDK or the Connector Builder) registered with a particular organization.

GET {baseURL}/orgs/{orgId}/connector

where

- {baseURL}: The base URL, as [described above](https://developer.jitterbit.com/connector-sdk/apis/#base-url)
- {orgId}: Organization ID of the Harmony org in which the connector is registered

## Request headers[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-headers_3)

- authToken: Authorization token obtained from [logging in to Harmony](https://developer.jitterbit.com/connector-sdk/apis/#log-in-to-jitterbit-harmony)

## Response[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#response_2)

The body of the response will contain a JSON string with a list of registered connectors. This example shows an org with the example Dropbox connector registered:

{

"status": true,

"operation": "List registered connectors",

"registeredConnectorList": \[

{

"id": "4471",

"name": "Dropbox",

"version": "1.0.0",

"key": "6d093654-d...2-10cad6797d6e",

"secret": "3673e11b-f...d-5e3f3ad796d5",

"endpointEntityId": "2370701",

"functionEntityStartId": "2370702",

"functionEntityEndId": "2370800"

}

\]

}

# Delete a connector registration[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#delete-a-connector-registration)

Deletes the registration of a custom connector. This API will succeed only if the connector is not used in any projects in the organization. To delete the JSON payload (the JSON file describing the UI, given in the manifest entry Jitterbit-Connector-UI) of a custom connector, use the API to [delete a connector payload](https://developer.jitterbit.com/connector-sdk/apis/#delete-a-connector-payload).

DELETE {baseURL}/orgs/{orgId}/connector/{connectorId}

where

- {baseURL}: The base URL, as [described above](https://developer.jitterbit.com/connector-sdk/apis/#base-url)
- {orgId}: Organization ID of the Harmony org in which the connector is registered
- {connectorId}: Connector ID, obtained when the connector was registered

## Request headers[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-headers_4)

- authToken: Authorization token obtained from [logging in to Harmony](https://developer.jitterbit.com/connector-sdk/apis/#log-in-to-jitterbit-harmony)

# Delete a connector payload[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#delete-a-connector-payload)

Deletes the JSON payload (the JSON file describing the UI, given in the manifest entry Jitterbit-Connector-UI) of a custom connector. The payload is cached at Harmony in order to render the Integration Studio UI of the connector. This API will succeed only if the connector is not used in any projects in the organization. To delete the registation of a custom connector, use the API to [delete a connector registration](https://developer.jitterbit.com/connector-sdk/apis/#delete-a-connector-registration).

DELETE {baseURL}/orgs/{orgId}/connector/{connectorId}/sdk/delete

where

- {baseURL}: The base URL, as [described above](https://developer.jitterbit.com/connector-sdk/apis/#base-url)
- {orgId}: Organization ID of the Harmony org in which the connector is registered
- {connectorId}: Connector ID, obtained when the connector was registered

## Request headers[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-headers_5)

- authToken: Authorization token obtained from [logging in to Harmony](https://developer.jitterbit.com/connector-sdk/apis/#log-in-to-jitterbit-harmony)

# Validate a connector key and secret[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#validate-a-connector-key-and-secret)

Validates a connector key and secret pair.

PUT {baseURL}/orgs/{orgId}/connector/validate/securityinfo

where

- {baseURL}: The base URL, as [described above](https://developer.jitterbit.com/connector-sdk/apis/#base-url)
- {orgId}: Organization ID of the Harmony org in which the connector is registered

## Request headers[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-headers_6)

- authToken: Authorization token obtained from [logging in to Harmony](https://developer.jitterbit.com/connector-sdk/apis/#log-in-to-jitterbit-harmony)

## Request body[**¶**](https://developer.jitterbit.com/connector-sdk/apis/#request-body_2)

The body of the request must contain:

{

"name": "{connectorName}",

"key": "{key}",

"secret": "{secret}"

}

where

- {connectorName}: The name of the connector
- {key}: The key associated with the connector of that name
- {secret}: The secret associated with the connector of that name