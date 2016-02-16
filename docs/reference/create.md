<!--[metadata]>
+++
title = "create"
description = "Create a Swarm manager."
keywords = ["swarm, create"]
[menu.main]
identifier="swarm.create"
parent="smn_swarm_subcmds"
+++
<![end-metadata]-->

# create

The `create` command uses Docker Hub's hosted discovery service to create a unique *discovery token* for your cluster. For example:

    $ docker run --rm  swarm create
    86222732d62b6868d441d430aee4f055

> Warning: Docker Hub's hosted discovery service is not recommended for production use. It’s intended to be used for testing/development. See the discovery backends for production use.

Later, when you create Swarm managers and nodes, you use the `<discovery>` argument to specify the token (e.g., `token://86222732d62b6868d441d430aee4f055`). The discovery service registers each new Swarm manager and node that uses the token as a member of your cluster.

Some documentation also refers to the discovery token as *cluster_id*.

For more information and examples, see the [Docker Swarm Discovery](../discovery.md) topic.
