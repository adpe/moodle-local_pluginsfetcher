# Moodle Plugins Fetcher Plugin [![Build Status](https://travis-ci.org/adpe/moodle-local_pluginsfetcher.svg?branch=master)](https://travis-ci.org/adpe/moodle-local_pluginsfetcher)

This plugin install a new webservice `local_pluginsfetcher_get_information` which can be use to retrieve information about installed plugins.

## Main features

There are two optional parameters which can be combined to fetch only given data:

| key         | value  | description                             |
|-------------|--------|-----------------------------------------|
| type        | string | Only given plugin types will be fetched |
| contribonly | int    | Only additional plugins will be fetched |

## Installation
1. Copy this plugin to the `local` directory of your Moodle instance: `git clone https://github.com/adpe/moodle-local_pluginsfetcher.git local/pluginsfetcher`
2. Visit the notifications page to complete the install process

For more information, visit [MoodleDocs](https://docs.moodle.org/37/en/Installing_plugins#Installing_manually_at_the_server) for installing contributed modules and plugins.

## Configuration
Please create a `token` for this new created service `Plugins fetcher` using [Site administration](https://FQDN/admin/settings.php?section=webservicetokens). It's important that the user has the capability `moodle/site:config`.
