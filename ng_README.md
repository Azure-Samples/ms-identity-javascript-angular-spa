# Angular 11 MSAL Angular 2.x Sample

This developer sample is used to demonstrate how to use MSAL-Angular v2.

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 11.0.1.

## How to run the sample

### Pre-requisites
- Ensure [all pre-requisites](https://github.com/AzureAD/microsoft-authentication-library-for-js/blob/msal-angular-v2/lib/msal-angular/README.md) have been completed to run msal-angular.

### Configure the application
- Open `./src/app/app.modules.ts` in an editor.
- Replace client id with the Application (client) ID from the portal registration, or use the currently configured lab registration. 
  - Optionally, you may replace any of the other parameters, or you can remove them and use the default values.

### Running the sample
- In a command prompt, run `npm start`.
- Navigate to [http://localhost:4200](http://localhost:4200)
- In the web page, click on the "Login" button. The app will automatically reload if you change any of the source files.

## Additional notes
- The default interaction type for the sample is redirect. The sample can be configured to use popups by changing the `interactionType` in `app.module.ts` to `InteractionType.Popup`. 
