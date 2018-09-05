# NGINX Docker Image - PHP FastCGI
Custom NGINX Docker image for use with PHP FastCGI containers. Based on Alpine.

## Limitations
The PHP application you are talking to must support a `try_files` directive that looks like
`try_files $uri $uri/ /index.php?$args;`. WordPress supports this configuration, but not all
applications are guaranteed to do so.
