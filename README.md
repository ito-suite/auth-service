# sso - Single Sign On

Central Auth Service for all Members of ito-suite

This service creates unique evercookie tokens for anonymous devices, and allows the consolidation of various evercookie tokens into one registered user account. Users can remain "anonymous", become registered, become invited to join organizations or de delegated as admins. Furthermore, any registered user may request api-level access which can only be approved by domain-level admins.

### Features

* csrf protection
* controls domain access
* requires https in production
* manages api tokens
* CLI Tools for user management and analysis
* salt & hash password protection
* picpass integration

### Endpoints

* create /:version/SSO/register/:domain
* post /:version/SSO/confirm
* post /:version/SSO/reset
* post /:version/SSO/login
* post /:version/SSO/logout
* post /:version/SSO/evercookie
* post /:version/SSO/token/:domain

### Tests

* pass / fail endpoint testing
* see https://certsimple.com/blog/a-plus-node-js-ssl
