# sso - Single Sign On

Central Auth Service for all Members of ito-suite

This service creates unique evercookie tokens for anonymous devices, and allows the consolidation of various evercookie tokens into one account.

### Features

* csrf protection
* controls domain access
* manages service access
* requires https in production
* manages api tokens

### Endpoints

* create /:version/SSO/register/:domain
* post /:version/SSO/confirm
* post /:version/SSO/reset
* post /:version/SSO/login
* post /:version/SSO/logout
* post /:version/SSO/evercookie

### Tests

* see https://certsimple.com/blog/a-plus-node-js-ssl
