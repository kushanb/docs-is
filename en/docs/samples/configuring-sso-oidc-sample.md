# Configuring Single Sign On Using OpenID Connect

This page guides you through configuring single sign on authentication between two OAuth/OpenID Connect web applications using two **sample applications** called Pickup Dispatch and Pickup Manager. 

----

## Scenario

Pickup is a cab company that has two SAML web applications called pickup-dispatch and pickup-manager. Both applications use WSO2 IS as the identity provider. When SSO is configured for both these applications, a user is only required to provide their credentials to the first application and the user will be automatically logged in to the second application.

![oidc-sso-scenario](../assets/img/samples/oidc-sso-scenario-diagram.png)

Follow the steps below to deploy two sample applications and see how this works. 

----

## Set up Pickup Dispatch sample

{!samples/pickup-dispatch-oidc.md!}

----

## Set up Pickup Manager sample

{!samples/pickup-manager-oidc.md!}

You are now ready to try out OpenID Connect SSO with the Pickup Dispatch and Pickup Manager sample web applications.

----

## Try it out

1. Navigate to <http://wso2is.local:8080/pickup-dispatch> on your browser and click **Login**.

    ![dispatch-login](../assets/img/samples/dispatch-login.png)

2. You will be redirected to the login page of WSO2 Identity Server. Log in using your WSO2 Identity Server credentials (admin/admin). Provide the required consent.
You will be redirected to the Pickup Dispatch application home page.

3. Now, if you navigate to <http://wso2is.local:8080/pickup-manager> and click **Login**, you can see that user has been automatically logged in to this application without being prompted for user credentials.

You have successfully configured OpenID Connect Single Sign-On for two web applications using WSO2 Identity Server as the identity provider. 