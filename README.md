# Moodle Update Script
To automate __our environment__ we wrote this shell script. It may wont work in your environment, but maybe you get some ideas for your own script.

## Setup
1. Download the _moodle-update_ file into _/var/www_
2. Make it executable ("chmod u+x")

## Plugins
At the top of the script you have to check the list of folders which shall be used in the new moodle version. It's the __FOLDER[]__-Array. Modify it to your needs.

## Usage
You can run the script with a moodle version paramter: __./update-moodle 3.5__ or without it.
