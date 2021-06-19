# OAuth

## What is OAuth?
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

## Give an example of what using OAuth would look like.
- when you go to log on a website via another website’s.
- user sending cloud-stored files to another user via email,

## How does OAuth work? What are the steps that it takes to authenticate the user?
- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
- The first site gives this token and secret to the initiating user’s client software.
- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
- The user approves (or their software silently approves) a particular transaction type at the first website.
- The user is given an approved access token.
- The user gives the approved access token to the first website.
- The first website gives the access token to the second website as proof of authentication on behalf of the user.
- The second website lets the first website access their site on behalf of the user.
- The user sees a successfully completed transaction occurring.

## What is OpenID?
 allows you to use an existing account to sign in to multiple websites, without needing to create new passwords

# authorization and authentication

## What is the difference between authorization and authentication?
authentication | authorization
---------|-------------------
Determines whether users are who they claim to be   | Determines what users can and cannot access
Challenges the user to validate credentials (for example, through passwords, answers to security questions, or facial recognition)   | Verifies whether access is allowed through policies and rules
Usually done before authorization  | Generally, transmits info through an Access Token
Generally governed by the OpenID Connect (OIDC) protocol   | Generally governed by the OAuth 2.0 framework
Example: Employees in a company are required to authenticate through the network before accessing their company email  | Example: After an employee successfully authenticates, the system determines what information the employees are allowed to access

## What is Authorization Code Flow?
 use for server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow (defined in OAuth 2.0 RFC 6749, section 4.1), which exchanges an Authorization Code for a token.
## What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE).
## What is Implicit Flow with Form Post?
OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets.
## What is Client Credentials Flow?
With machine-to-machine (M2M) applications
## What is Device Authorization Flow?
With input-constrained devices that connect to the internet, rather than authenticate the user directly,
## What is Resource Owner Password Flow?
highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.