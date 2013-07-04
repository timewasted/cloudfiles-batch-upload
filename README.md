cloudfiles-batch-upload
=======================

This is a quick hack to upload a directory structure to Rackspace's Cloud Files.  It preserves the appearance of a directory structure by including the directory name as part of the file name.  For example, if you were to batch upload `/tmp`, the file `/tmp/store/images/products/1.jpg` would be uploaded to Cloud Files as `store/images/products/1.jpg`.

Usage:
------

Clone both this repository and Rackspace's [php-cloudfiles](https://github.com/rackerlabs/php-cloudfiles) repository or alternatively update the submodule.  Move `cloudfiles-batch-upload.php` into the `php-cloudfiles` directory (optionally change the `require('./cloudfiles.php');` line in `cloudfiles-batch-upload.php` to point to the correct location).  Edit the variables defined at the top of `cloudfiles-batch-upload.php`, then run the script.


