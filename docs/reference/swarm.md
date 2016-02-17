<!--[metadata]>
+++
title = "Command line reference"
description = "Docker Swarm Commands Overview"
keywords = ["Swarm, cluster, commands"]
[menu.main]
identifier="smn_swarm_subcmds"
parent="workw_swarm"
weight=80
+++
<![end-metadata]-->

# Swarm — A Docker-native clustering system

The `swarm` command runs a Swarm container on a Docker Engine host. You can use `swarm` to create a Swarm manager or nodes in a cluster.

## Syntax

    $ docker run swarm [OPTIONS] COMMAND [arg...]

## Options:
* `--debug` — Enable debug mode. Displays messages that you can use to debug a Swarm node. The environmental variable for this option is `[$DEBUG]`.
* `--log-level "<value>"` or `-l "<value>"` — Set the log level. Where `<value>` is: `debug`, `info`, `warn`, `error`, `fatal`, or `panic`. The default value is `info`.
* `--experimental` — Enable experimental features.
* `--help` or `-h` — Display help.
*  `--version` or `-v` — Display the version. For example:
        $ docker run swarm --version
        swarm version 1.1.0 (a0fd82b)

## Commands:
- [create, c](create.md) - Create a discovery token
- [list, l](list.md) - List the nodes in a Docker cluster
- [manage, m](manage.md) - Create a Swarm manager
- [join, j](join.md) - Create a Swarm node
- [help](help.md) - Display a list of Swarm commands, or help for one command

Run 'swarm COMMAND --help' for more information on a command.
