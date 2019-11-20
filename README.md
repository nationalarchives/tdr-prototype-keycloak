# Keycloak TDR Prototype

We are considering using [keycloak](https://www.keycloak.org/) for our user management and as an OpenId connect provider for Cognito. The reasons will be stored elsewhere, this repo is for configuring the docker image to run this service.

The [standalone-ha.xml](standalone-ha.xml) file is the configuration of the server. At the moment, it is only used to configure keycloak to sit behind a reverse proxy but we may want to add more configuratioin in the future. 

The govuk folder contains a theme which is built from [this repository](https://github.com/UKGovernmentBEIS/keycloak-theme-govuk) This means that all of our login forms look like the GDS design system.

The remainder of the files are used for adding sms two factor auth to the browser login. This is built from [this repository](https://github.com/UKGovernmentBEIS/keycloak-sms-authenticator-sns).