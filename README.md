<p align="center">
  <a href="https://roots.io/bedrock/">
    <img alt="Bedrock" src="https://cdn.roots.io/app/uploads/logo-bedrock.svg" height="100">
  </a>
</p>

<p align="center">
  <a href="LICENSE.md">
    <img alt="MIT License" src="https://img.shields.io/github/license/roots/bedrock?color=%23525ddc&style=flat-square" />
  </a>

  <a href="https://packagist.org/packages/roots/bedrock">
    <img alt="Packagist" src="https://img.shields.io/packagist/v/roots/bedrock.svg?style=flat-square" />
  </a>

  <a href="https://circleci.com/gh/roots/bedrock">
    <img alt="Build Status" src="https://img.shields.io/circleci/build/gh/roots/bedrock?style=flat-square" />
  </a>

  <a href="https://twitter.com/rootswp">
    <img alt="Follow Roots" src="https://img.shields.io/twitter/follow/rootswp.svg?style=flat-square&color=1da1f2" />
  </a>
</p>

<p align="center">
  <strong>A modern WordPress stack</strong>
  <br />
  Built with ❤️
</p>

<p align="center">
  <a href="https://roots.io">Official Website</a> | <a href="https://roots.io/docs/bedrock/master/installation/">Documentation</a> | <a href="CHANGELOG.md">Change Log</a>
</p>

## Supporting

**Bedrock** is an open source project and completely free to use.

However, the amount of effort needed to maintain and develop new features and products within the Roots ecosystem is not sustainable without proper financial backing. If you have the capability, please consider donating using the links below:

<div align="center">

[![Donate via Patreon](https://img.shields.io/badge/donate-patreon-orange.svg?style=flat-square&logo=patreon")](https://www.patreon.com/rootsdev)
[![Donate via PayPal](https://img.shields.io/badge/donate-paypal-blue.svg?style=flat-square&logo=paypal)](https://www.paypal.me/rootsdev)

</div>

## Overview

Bedrock is a modern WordPress stack that helps you get started with the best development tools and project structure.

Much of the philosophy behind Bedrock is inspired by the [Twelve-Factor App](http://12factor.net/) methodology including the [WordPress specific version](https://roots.io/twelve-factor-wordpress/).

## Features

- Better folder structure
- Dependency management with [Composer](https://getcomposer.org)
- Easy WordPress configuration with environment specific files
- Environment variables with [Dotenv](https://github.com/vlucas/phpdotenv)
- Autoloader for mu-plugins (use regular plugins as mu-plugins)
- Enhanced security (separated web root and secure passwords with [wp-password-bcrypt](https://github.com/roots/wp-password-bcrypt))

## Requirements

- PHP >= 7.1
- Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

## Installation

1. Download the repo and create a new project in your IDE
2. Create a .env file in the root folder and update environment variables 
    `DB_CONNECTION=mysql`
    `DB_HOST=localhost`
    `DB_PORT=3306`
    `DB_NAME=nubis`
    `DB_USER=YOUR_USERNAME`
    `DB_PASSWORD=YOUR_PASSWORD`

    `WP_ENV=development`
    `WP_HOME=http://localhost:8000`
    `WP_SITEURL="${WP_HOME}/wp"`
    `WP_DEBUG_LOG=/path/to/debug.log`

# Generate your keys here: https://roots.io/salts.html Use this link and copy the result (Env format) into your .env file and save the file

3. Go to the nubis theme folder with `cd web/app/themes/nubis` and run `yarn`
4. Then run `yarn start`
5. Open a 2nd terminal, check if your in the root folder and run `composer install`
6. Then run `php -S 0.0.0.0:8000 -t web`
7. Go to `localhost:8000` and install WordPress there
8. Now you're good to go!

Everytime you want to start working: open 2 terminals and run `yarn start` and `php -S 0.0.0.0:8000 -t web`.


## Documentation

Bedrock documentation is available at [https://roots.io/docs/bedrock/master/installation/](https://roots.io/docs/bedrock/master/installation/).

## Contributing

Contributions are welcome from everyone. We have [contributing guidelines](https://github.com/roots/guidelines/blob/master/CONTRIBUTING.md) to help you get started.

## Bedrock sponsors

Help support our open-source development efforts by [becoming a patron](https://www.patreon.com/rootsdev).

<a href="https://kinsta.com/?kaid=OFDHAJIXUDIV"><img src="https://cdn.roots.io/app/uploads/kinsta.svg" alt="Kinsta" width="200" height="150"></a> <a href="https://k-m.com/"><img src="https://cdn.roots.io/app/uploads/km-digital.svg" alt="KM Digital" width="200" height="150"></a>

## Community

Keep track of development and community news.

- Participate on the [Roots Discourse](https://discourse.roots.io/)
- Follow [@rootswp on Twitter](https://twitter.com/rootswp)
- Read and subscribe to the [Roots Blog](https://roots.io/blog/)
- Subscribe to the [Roots Newsletter](https://roots.io/subscribe/)
- Listen to the [Roots Radio podcast](https://roots.io/podcast/)
