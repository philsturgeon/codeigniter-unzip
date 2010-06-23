CodeIgniter-Unzip
============

Extract ZIP files in CodeIgniter without installing any PECL extensions for PHP.


Requirements
------------

1. PHP 5.1+
2. CodeIgniter 1.6.x - 2.0-dev
3. ZLib extension enabled


Usage
-----

    $this->load->library('unzip');

    // Optional: Only take out these files, anything else is ignored
    $this->unzip->allow(array('css', 'js', 'png', 'gif', 'jpeg', 'jpg', 'tpl', 'html', 'swf'));

    // Give it one parameter and it will extract to the same folder
    $this->unzip->extract('uploads/my_archive.zip');

    // or specify a destination directory
    $this->unzip->extract('uploads/my_archive.zip', '/path/to/directory/);

Simple as that!


To-do
-----

- Add extract_file() to extract a specific file from your ZIP.