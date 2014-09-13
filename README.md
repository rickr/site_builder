Nice and easy bash script to generate static websites from templates

Usage

Initialize a work directory
    $ site_builder init <work dir>

Edit your templates:
    vi <work_dir>/templates/head.html
    vi <work_dir>/templates/foot.html

Add content:
    vi <work_dir/content/<your page>.html

If required edit the post script: 
    vi <work_dir>/post_script.sh

This script is passed one argument - the path of the compiled page.
This is intended so you can do somewhat dynamic content like setting
a nav element active based on the $1 value.


Compile your site
    $ site_builder compile <work_dir>

Compiled site is located in
    <work_dir>/compiled

Upload to your webserver:
    scp <work_dir>/compiled/* www.example.com:/var/www/html


