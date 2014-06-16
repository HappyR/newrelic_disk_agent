## New Relic Disk Plugin

Monitors server's disk

### Requirements

In order to use this plugin, you must have an active New Relic account.

Plugin should work on any generic Unix environment with the following
software components installed:

  - Ruby (>= 1.8.7)
  - bundler for Ruby: https://github.com/carlhuda/bundler

### Instructions for running the agent

1. run `bundle install` to install required gems
2. Edit `config/newrelic_plugin.yml` and replace "YOUR_LICENSE_KEY_HERE" with your New Relic license key
3. Running the plugin

Plugin can  be started as a daemon using the following command:

  ./newrelic_disk_agent.daemon start

In this case you can check its status by running

  ./newrelic_disk_agent.daemon status

and stop it with

  ./newrelic_disk_agent.daemon stop

### Fork information
This is a fork from Steven Eksteen and his plugin [newrelic_sidekiq_agent](https://github.com/mscifo/newrelic_sidekiq_agent).