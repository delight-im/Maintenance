# Maintenance

Simple and effective maintenance page for websites

## Requirements

 * PHP 5.6.0+

## Usage

 * Copy the file [`Source/maintenance.php`](Source/maintenance.php) to some subfolder of your website
 * During actual maintenance (or for testing), just redirect *all* requests to `maintenance.php`

   * Apache (in `.htaccess` or `httpd.conf`)

     ```
     RewriteEngine On
     RewriteRule . maintenance.php [L]
     ```

   * Nginx (in `nginx.conf`)

     ```
     try_files $uri /maintenance.php;
     ```

## Contributing

All contributions are welcome! If you wish to contribute, please create an issue first so that your feature, problem or question can be discussed.

## License

This project is licensed under the terms of the [MIT License](https://opensource.org/licenses/MIT).
