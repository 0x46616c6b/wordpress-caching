# Better Wordpress Caching

## Install

- Download the plugin [WP Super Cache Plugin](http://wordpress.org/plugins/wp-super-cache/)
- Extract the plugin and copy to `wp-content/plugins/`

## Update your wp-config.php

- Enable `WP_CACHE` and set `WPCACHEHOME` in your `wp-config.php`

        define('WP_CACHE', true);
        define('WPCACHEHOME', __DIR__ . '/wp-content/plugins/wp-super-cache/');

## Activate and configure the plugin

- Enable the plugin
- Go to settings page (find under Settings > WP Super Cache)
- Enable Caching
- Go to Advanced Tab, use mod_rewrite to deliver the cache files
- Install `.htaccess` with rewrite rules from the plugin or copy the example [htaccess.txt](/htaccess.txt) from this repository (**Note:** The rules depend on your cache configuration!)
- Activate Preloading for Cache files
- Add additional tweaks for caching assets (already added in the example `.htaccess` file)

**Important:** To use all enhancements you must activate headers, deflate and expire module from Apache.

**Info:** For better performance and reduce of disk I/O include your `.htaccess` to server config