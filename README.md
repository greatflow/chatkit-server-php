# Chatkit Retirement Announcement
We are sorry to say that as of April 23 2020, we will be fully retiring our
Chatkit product. We understand that this will be disappointing to customers who
have come to rely on the service, and are very sorry for the disruption that
this will cause for them. Our sales and customer support teams are available at
this time to handle enquiries and will support existing Chatkit customers as
far as they can with transition. All Chatkit billing has now ceased , and
customers will pay no more up to or beyond their usage for the remainder of the
service. You can read more about our decision to retire Chatkit here:
[https://blog.pusher.com/narrowing-our-product-focus](https://blog.pusher.com/narrowing-our-product-focus).
If you are interested in learning about how you can build chat with Pusher
Channels, check out our tutorials.

# Chatkit PHP Server SDK

[![Read the docs](https://img.shields.io/badge/read_the-docs-92A8D1.svg)](https://docs.pusher.com/chatkit/reference/server-php)
[![Twitter](https://img.shields.io/badge/twitter-@Pusher-blue.svg?style=flat)](http://twitter.com/Pusher)
[![GitHub license](https://img.shields.io/badge/license-MIT-lightgrey.svg)](https://github.com/pusher/chatkit-server-php/blob/master/LICENSE.md)
[![PHP version](https://badge.fury.io/ph/pusher%2Fpusher-chatkit-server.svg)](https://badge.fury.io/ph/pusher%2Fpusher-chatkit-server)

Find out more about Chatkit [here](https://pusher.com/chatkit).

## Installation

**We recommend you [use composer](http://getcomposer.org/).**

You can get the Chatkit PHP SDK via a composer package called `pusher-chatkit-server`. See <https://packagist.org/packages/pusher/pusher-chatkit-server>

```bash
$ composer require pusher/pusher-chatkit-server
```

Or add to `composer.json`:

```json
"require": {
    "pusher/pusher-chatkit-server": "^1.1.0"
}
```

and then run `composer update`.

Or you can clone or download the SDK files.

This SDK depends on PHP modules for cURL and JSON. See [cURL module installation instructions](http://php.net/manual/en/curl.installation.php) and [JSON module installation instructions](http://php.net/manual/en/json.installation.php).

## Deprecated versions

 Versions of the library below
 [1.0.0](https://github.com/pusher/chatkit-server-php/releases/tag/1.0.0) are
 deprecated and support for them will soon be dropped.

 It is highly recommended that you upgrade to the latest version if you're on
 an older version. To view a list of changes, please refer to the
 [CHANGELOG](CHANGELOG.md).

## Getting started

Head over to [our documentation](https://docs.pusher.com/chatkit/reference/server-php).

## Running tests

*WARNING* Executing these tests will issue real requests to the configured Chatkit instance, some of which may be destructive. You should NOT run against a live production instance.

Install [PHPUnit](https://phpunit.de/).

Ensure dependencies are up to date:
```
composer update
```

Set instance locator and secret key environment variables (available in the dashboard at dash.pusher.com):
```
export CHATKIT_INSTANCE_LOCATOR="v1:us1:89755518-5782-413d-9446-0d2726dd1e5a"
export CHATKIT_INSTANCE_KEY="2a188376-d4f0-47fa-8954-dd08115ea98c:NDk5YTZkOTgtMzk2ZC00NDlhLTg1MTYtYjNhODYzYWNiMjczCg="
```

Execute tests against a Chatkit instance:
```
/vendor/phpunit/phpunit/phpunit
```
## Release process
1. Update the CHANGELOG
2. On Git, tag with the new version and push
[Packagist](https://packagist.org/packages/pusher/pusher-chatkit-server) automatically releases new versions of the library upon detecting a new Github release.
