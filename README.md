# itsec-local-qr-code

itsec-local-qr-code is a WordPress plugin available to Security users. It hooks into the existing QR generation functionality for customers who do not want to contact our remote API to generate QR codes.

## Installation

We recommend [LocalWP](https://localwp.com/), [Lando](https://lando.dev), [Docker](https://www.docker.com/), [VVV](https://github.com/Varying-Vagrant-Vagrants/VVV), or another flavor of local development that's cool too!

Using LocalWP you will need to perform the following steps:

1. Create a new WordPress site with `example.test` as the URL (or whatever URL you'd like..)
2. Open up a terminal window and `cd` into your local plugins directory: `/path/to/wp-content/plugins/`
3. Fork this repository from GitHub and then clone that into your plugins directory in the `itsec-local-qr-code` directory
4. In the repository directory, run `git submodule update --init --recursive`
5. In the WordPress admin, activate the plugin

That's it. You're now ready to start development.

**Development Notes**

* Ensure that you have `SCRIPT_DEBUG` enabled within your wp-config.php file. Here's a good example of wp-config.php for debugging:
```
 // Enable WP_DEBUG mode
define( 'WP_DEBUG', true );

// Enable Debug logging to the /wp-content/debug.log file
define( 'WP_DEBUG_LOG', true );

// Loads unminified core files
define( 'SCRIPT_DEBUG', true );
```
