# Moodle Update Script
To automate __our environment__ we wrote this shell script. It may won't work in your environment, but maybe you get some ideas for your own script.


## Usage

* Without any parameter: `./update-moodle`

* New version: `./update-moodle 3.5`

* New version + explicit file: `./update-moodle 3.5 https://example.com/moodle-3.5.2.zip`


## Setup
1. Clone the repository.
1. Create a symlink from there to `/var/www/moodle-update`
1. Make it executable: `chmod +x moodle-update`

### Plugins
At the top of the script you have to check the list of folders which shall be used in the new moodle version. It's the `FOLDER[]`-Array. Modify it to your needs.
