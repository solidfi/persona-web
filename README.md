# persona-web
Persona Sample for Web

## Table of contents

- [Overview](#overview)
- [Run the app](#run-the-app)
- [Parameters](#Parameters)
- [Internals](#internals)

## Overview
The purpose of this app is to show how to use the Persona JavaScript SDK.For complete information about the API, head to the [docs](https://docs.withpersona.com/docs).

## Run the app
To Run the app run `npx serve`. then open `http://localhost:5000` in browser.

## Parameters

| Parameters    | Description   |
| ------------- | ------------- |
| templateId    | This template ID corresponds to a pre-set configuration and determines how the flow is customized. To get the `templateId` check [persona docs](https://docs.withpersona.com/docs/getting-an-api-key)           |
| personId/referrenceId  | Current logged in user id  |
| environment  | The Persona API environment on which to create inquiries. For sandbox and production, use `sandbox` and `production` respectively.  |

## Internals

- Loads [persona sdk](https://docs.withpersona.com/docs/quickstart-embedded-flow) using bellow code
 ```<script src="https://cdn.withpersona.com/dist/persona-v4.0.0.js"></script>```
- The `verify` function collects all information from input fields.and it will call persona client methods.
- In a real-life integration, the `templateId` and `environment` would have to be requested from `idv-template` api.
