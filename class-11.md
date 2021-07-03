## What is OAuth? 
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.

## OAuth examples
- when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

## How OAuth works?
- he first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- The first site gives this token and secret to the initiating user’s client software.
- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
- The user approves (or their software silently approves) a particular transaction type at the first website.
- The user is given an approved access token (notice it’s no longer a request token).
- The user gives the approved access token to the first website.
- The first website gives the access token to the second website as proof of authentication on behalf of the user.
- The second website lets the first website access their site on behalf of the user.
- The user sees a successfully completed transaction occurring.
- OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. 



## What is OpenID?

**"OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."**

OpenID began life in 2005 as a means for logging into the then-popular LiveJournal blogging site but quickly spread to other sites. The idea, in the early days of Web 2.0, was that rather than having multiple logins for multiple websites, OpenID would serve as a single sign-in, vouching for the identities of users. But in practice OpenID was difficult to implement on the developer side, and never really became that appealing to users, especially as there was competition in that space.

## Authentication and Authorization Flows
Auth0 uses the OpenID Connect (OIDC) Protocol and OAuth 2.0 Authorization Framework to authenticate users and get their authorization to access protected resources. 

![img](https://techdifferences.com/wp-content/uploads/2018/01/Untitled-4.jpg)

Authorization code flow is used to obtain an access token to authorize API requests.

## The Authorization Code Flow  PKCE 
is an OpenId Connect flow specifically designed to authenticate native or mobile application users. This flow is considered best practice when using Single Page Apps (SPA) or Mobile Apps. 

## What is Implicit Flow with Form Post?
mplicit Flow with Form Post flow uses OIDC to implement web sign-in that is very similar to the way SAML and WS-Federation operates. 