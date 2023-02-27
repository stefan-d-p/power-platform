# Aleph Alpha API Connector

“Aleph Alpha’s mission is to enable the accessibility, usability and integration of large, European multilanguage and multimodal AI models following the likes of GPT-3 and DALL-E, driving innovation for the explainability, alignment and integration. The funds significantly accelerate the process of bringing the latest generation of AI technology into application and secure the digital sovereignty for public and private sector partners in Europe and beyond.”

Jonas Andrulis, CEO and founder of Aleph Alpha

> This is an **unoffical Aleph Alpha API custom connector**. Iam not affiliated with Aleph Alpha.

## Prerequisites

- A Microsoft Power Apps or Power Automate plan with custom connector feature
- A [Aleph Alpha](https://www.aleph-alpha.com) API account

## How to get credentials

The connection item requires your Aleph Alpha Authentication Key. You can retrieve your key from your account page.

## Getting started

- Download the apiDefinition.swagger.json
- Add a new custom connector and select import from OpenAPI
- Provide an Icon and background color for the connector
- Click **Create Connector**

Visit the official [Aleph Alpha API documentation](https://docs.aleph-alpha.com/api/) for further details on the various actions and parameters.

## Known issues and limitations

The current version only features a subset of the available endpoints. Current features:

- Complete texts
- Summarize texts or Microsoft Word documents

## Operations

- `CompletePrompt`: Will complete a prompt using a specific Luminous model
- `SummarizeDocument`: Will summarize a document using a specific Luminous model.
- `GetVersion`: Returns the current API version
- `GetUserTokens`: Returns all active tokens configured in the Aleph Alpha account page.
- `CreateUserToken`: Creates a new token
- `DeleteToken`: Deletes an existing token from the account
- `GetAvailableModels`: Returns all available Luminous models. This operation acts as a dynamic input for other operations.

## FAQ
