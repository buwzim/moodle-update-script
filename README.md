# Moodle Update Script
To automate __our environment__ we wrote this shell script. It may wont work in your environment, but maybe you get some ideas for your own script.

## Setup
1. Download the _moodle-update_ file into _/var/www_
2. Make it executable ("chmod u+x")

## Plugins
At the top of the script you have to check the list of folders which shall be used in the new moodle version. It's the __FOLDER[]__-Array. Modify it to your needs.

## Usage
* You can run the script with or without a moodle version paramter to install the latest version: __./update-moodle 3.5__
* You can also add an URL as 2nd parameter to specify the download source: __./update-moodle 3.5 https://example.com/moodle-3.5.2.zip__
* If a newer version is available, the script will inform you about it.

## Restore
* To restore a backup use: _moodle-restore foldername_
* It has to be the same version (x.y) as in use.
