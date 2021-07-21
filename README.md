---
page_type: sample
languages:
- javascript
- typescript
products:
- angular
- ms-graph
- azure-active-directory
description: "Demonstrates how to use MSAL Angular v2 to login, logout, protect a route, and acquire an access token for a protected resource such as Microsoft Graph."
urlFragment: "ms-identity-javascript-angular-spa"
---

# Angular single-page application built with MSAL Angular v2 and Microsoft identity platform

This sample demonstrates how to use MSAL Angular v2 to login, logout, conditionally render components to authenticated users, and acquire an access token for a protected resource such as Microsoft Graph.

## Features

This sample demonstrates the following MSAL Angular concepts:

* Configuration
* Login
* Logout
* Protecting a route
* Acquiring an access token and calling Microsoft Graph

## Contents

| File/folder       | Description                                |
|-------------------|--------------------------------------------|
| `AppCreationScripts` | Contains automation scripts for Powershell users (can be safely removed if desired). |
| `src`             | Sample source code.                        |
| `.editorconfig`   | Defines editor config settings.            |
| `.gitignore`      | Define what to ignore at commit time.      |
| `angular.json`    | Angular configuration file.                |
| `browserslist`    | BrowsersList configuration file.           |
| `CHANGELOG.md`    | List of changes to the sample.             |
| `CONTRIBUTING.md` | Guidelines for contributing to the sample. |
| `karma.conf.js`   | Configuration for the karma test runner.   |
| `LICENSE`         | The license for the sample.                |
| `ng_README.md`    | README describing how to run the sample    |
| `package.json`    | Package manifest for npm.                  |
| `README.md`       | This README file.                          |
| `tsconfig.*.json` | TypeScript configuration files.            |
| `tslint.json`     | TS Lint configuration files.               |

**Note:** This sample's structure was generated with the [Angular CLI](https://cli.angular.io/).

## Getting Started

### Prerequisites

[Node.js](https://nodejs.org/en/) must be installed to run this sample.

### Setup

1. [Register a new application](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration) in the [Azure Portal](https://portal.azure.com). Ensure that the application is enabled for the [authorization code flow with PKCE](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow). This will require that you redirect URI configured in the portal is of type `SPA`.
1. Clone this repository `git clone https://github.com/Azure-Samples/ms-identity-javascript-angular-spa.git`
1. Open the [/src/app/app.module.ts](./src/app/app.module.ts) file and provide the required configuration values.
    1. Replace the string `"Enter_the_Application_Id_Here"` with your app/client ID on AAD Portal.
    1. Replace the string `"Enter_the_Cloud_Instance_Id_HereEnter_the_Tenant_Info_Here"` with `"https://login.microsoftonline.com/common/"`
    > :information_source: if you would like to sign-in users with your tenant only, use your tenant ID instead of `common`.
    1. Replace the string `"Enter_the_Redirect_Uri_Here"` with the redirect uri you setup on AAD Portal.
    1. Replace the string `"Enter_the_Graph_Endpoint_Herev1.0/me"` with `"https://graph.microsoft.com/v1.0/me"`
1. Open the [/src/app/profile/profile.component.ts](./src/app/profile/profile.component.ts) file and provide the required configuration value.
    1. Replace the string `"Enter_the_Graph_Endpoint_Herev1.0/me"` with `"https://graph.microsoft.com/v1.0/me"`
1. On the command line, navigate to the root of the repository, and run `npm install` to install the project dependencies via npm.

> :information_source: To configure this app for tenants on Sovereign/National clouds, see: [Use MSAL in a national cloud environment](https://docs.microsoft.com/azure/active-directory/develop/msal-national-cloud)

## Run the sample

1. Start the sample application with `npm start`.
2. In your browser, navigate to [http://localhost:4200](http://localhost:4200).

## Contributing

If you'd like to contribute to this sample, see [CONTRIBUTING.MD](./CONTRIBUTING.md).

## Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.
