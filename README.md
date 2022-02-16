# Pantheon prototype

[![CircleCI](https://circleci.com/gh/MITLibraries/mitlib-prototype/tree/master.svg?style=svg)](https://circleci.com/gh/MITLibraries/mitlib-prototype/tree/master)
[![Dashboard mitlib-prototype](https://img.shields.io/badge/dashboard-mitlib_prototype-yellow.svg)](https://dashboard.pantheon.io/sites/6f00abf5-3d86-46ac-93c6-43eab1f5c8aa#dev/code)
[![Dev Site mitlib-prototype](https://img.shields.io/badge/site-mitlib_prototype-blue.svg)](http://dev-mitlib-prototype.pantheonsite.io/)

This is a prototype WordPress site.

## Tooling

If you are reading this page on GitHub, you likely need to have the following
tooling available to you:

* [Composer](https://getcomposer.org/)
* [Terminus CLI tool](https://pantheon.io/docs/terminus)
  * [Build Tools plugin](https://github.com/pantheon-systems/terminus-build-tools-plugin)
  * [Composer plugin](https://github.com/pantheon-systems/terminus-composer-plugin)
  * [Secrets plugin](https://github.com/pantheon-systems/terminus-secrets-plugin)

## Environment variables / secrets

The following environment variables need to be defined for the site to
function as expected:

`SENTRY_DNS` - The project key to route exception information to Sentry. See
the configuration in `web/wp-config.php` for information on what errors are
sent.

`WPMS_SMTP_PASS` - The password for the account on the MIT email gateway

`WPMS_SMTP_USER` - The username for the account on the MIT email gateway
