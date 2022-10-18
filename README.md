# selfhosted-authentication-table
List of SelfHosted apps, with information about their support for OpenID / SAML / LDAP / Proxy Auth

✔️ - Supported - all functionality works including mobile apps (if any)  
😔 - Supported, but breaks some features, mobile apps, users have to still be added manually or not maintained  
❌ - Unsupported  
❔ - Not known yet, to be added  

Proxy Auth theoretically works on all of them, but it will break functionality, display double logins etc.   
So only those explicitly working great with it will be marked as such. Otherwise it will be unsupported.  

| **Project**                                                       | **OpenID** | **LDAP** | **Proxy Auth** | **Additional Info**                                                                                                                                                                                                                                                                           |
|-------------------------------------------------------------------|------------|----------|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [nextcloud](https://nextcloud.com)                                | ✔️          | ✔️        | ❌              | Install OpenID or LDAP plugin from interface to enable support                                                                                                                                                                                                                                |
| [hedgedoc](https://hedgedoc.org)                                  | ✔️          | ✔️        | ❌              |                                                                                                                                                                                                                                                                                               |
| [matrix synapse](https://matrix.org/docs/projects/server/synapse) | ✔️          | ✔️        | ❌              | LDAP Provided by additional module; openid supported natively                                                                                                                                                                                                                                 |
| [matrix dendrite](https://github.com/matrix-org/dendrite)         | ❌          | ❌        | ❌              | Some work on SSO in [this PR](https://github.com/matrix-org/dendrite/pull/2492), some work on LDAP [here](https://github.com/matrix-org/dendrite/pull/1877) but abandoned                                                                                                                     |
| [home assistant](https://www.home-assistant.io)                   | ❌          | 😔        | 😔              | [hass-proxy-auth](https://github.com/BeryJu/hass-auth-header) for proxy auth, but for some people it breaks mobile app, [hacky scripts](https://gist.github.com/rechner/57c123d243b8adb83ccb1dc94c80847f) for LDAP. {More Info](https://www.home-assistant.io/docs/authentication/providers/) |
