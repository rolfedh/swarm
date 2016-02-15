$ docker run swarm join --help
Usage: swarm join [OPTIONS] <discovery>

join a docker cluster

Arguments:
   <discovery>    discovery service to use [$SWARM_DISCOVERY]
                   * token://<token>
                   * consul://<ip>/<path>
                   * etcd://<ip1>,<ip2>/<path>
                   * file://path/to/file
                   * zk://<ip1>,<ip2>/<path>
                   * [nodes://]<ip1>,<ip2>

Options:
   --advertise, --addr 							Address of the Docker Engine joining the cluster. Swarm manager(s) MUST be able to reach the Docker Engine at this address. [$SWARM_ADVERTISE]
   --heartbeat "60s"							period between each heartbeat
   --ttl "180s"								sets the expiration of an ephemeral node
   --delay "0s"								add a random delay in [0s,delay] to avoid synchronized registration
   --discovery-opt [--discovery-opt option --discovery-opt option]	discovery options


rolfedlugy-hegwer at RsMBP in ~
$
