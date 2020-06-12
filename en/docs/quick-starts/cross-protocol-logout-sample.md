# Cross-Protocol Logout 

This page demonstrates [cross-protocol logout](TODO) across different protocols using two sample applications that use SAML and OpenID Connect. 

----

If you have your own applications, click the button below.

<a class="samplebtn_a" href="../../guides/login/cross-protocol-logout"   rel="nofollow noopener">I have my own applications</a>

----

{!fragments/pickup-dispatch-saml.md!}

----

{!fragments/pickup-manager-oidc.md!}

----

## Try it out

1. Access <http://wso2is.local:8080/saml2-web-app-pickup-dispatch.com> on your browser and click **Login**.

2. You will be redirected to the login page of WSO2 IS. Log in using your WSO2 IS credentials (admin/admin). Provide the required consent. You will be redirected to the Pickup Dispatch application home page.

3. Now, if you access <http://wso2is.local:8080/pickup-manager> and click **Login**, you can see that user has been automatically logged in to this application without being prompted for user credentials.

4. Click **Admin** on the top-right corner and click **Logout** to log out of the OIDC Pickup Manager application. 

5. Switch to the SAML Pickup Dispatch app on your browser. You will see that you have been logged out of the SAML application as well. 

You have successfully tried out cross-protocol logout between a SAML application and an OIDC application. 