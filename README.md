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
| enquiry-url   | Persona enquiry url          |


## Internals

- The `start` function collects all information from input fields.and it will start persona verification.
- In a real-life integration, the `enquiry-url`  would have to be requested from `idv-submit` api.
