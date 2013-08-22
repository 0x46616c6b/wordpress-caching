# Better Wordpress Caching

1. Install [WP Super Cache Plugin](http://wordpress.org/plugins/wp-super-cache/)
2. Activate and configure the plugin
3. Install `.htaccess` with rewrite rules from the plugin or copy the example [htaccess.txt](/htaccess.txt) from this repository
4. Add additional tweaks for caching assets (already added in the example `.htaccess` file)

**Important:** To use all enhancements you must activate headers, deflate and expire module from Apache.

**Info:** For better performance and reduce of disk I/O include your `.htaccess` to server config