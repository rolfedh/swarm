$ docker run swarm list --help
Usage: swarm list [OPTIONS] <discovery>

List nodes in a cluster

Arguments:
   <discovery>    discovery service to use [$SWARM_DISCOVERY]
                   * token://<token>
                   * consul://<ip>/<path>
                   * etcd://<ip1>,<ip2>/<path>
                   * file://path/to/file
                   * zk://<ip1>,<ip2>/<path>
                   * [nodes://]<ip1>,<ip2>

Options:
   --timeout "10s"							timeout period
   --discovery-opt [--discovery-opt option --discovery-opt option]	discovery options
