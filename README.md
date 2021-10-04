# Moodle Update Script
To automate __our environment__ we wrote this shell script. It may won't work in your environment, but maybe you get some ideas for your own script.


## Usage

* Without any parameter: `./update-moodle`

* New version: `./update-moodle 3.5`

* New version + explicit file: `./update-moodle 3.5 https://example.com/moodle-3.5.2.zip`


## Missing plugin sources
If Moodle is missing some plugin folders, run this command (adapted to your language) to find missing folders:

`diff -qr moodle_3.10 moodle_3.10_2021-10-01_09-49-12 | grep "Nur in moodle_3.10_"`


## Setup
1. Clone the repository.
1. Create a symlink from there to `/var/www/moodle-update`
1. Make it executable: `chmod +x moodle-update`

### Configs
If you don't create your own `.conf` files, the script will create it for you and use __our__ settings and plugins:

1. Copy plugins file: `cp plugins.conf.dist plugins.conf`
1. Copy settings file: `cp settings.conf.dist settings.conf`
