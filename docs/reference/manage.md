$ docker run swarm manage --help
Usage: swarm manage [OPTIONS] <discovery>

Manage a docker cluster

Arguments:
   <discovery>    discovery service to use [$SWARM_DISCOVERY]
                   * token://<token>
                   * consul://<ip>/<path>
                   * etcd://<ip1>,<ip2>/<path>
                   * file://path/to/file
                   * zk://<ip1>,<ip2>/<path>
                   * [nodes://]<ip1>,<ip2>

Options:
   --strategy "spread"							placement strategy to use [spread, binpack, random]
   --filter, -f [--filter option --filter option]			filter to use [health, port, dependency, affinity, constraint]
   --host, -H [--host option --host option]				ip/socket to listen on [$SWARM_HOST]
   --replication							Enable Swarm manager replication
   --replication-ttl "15s"						Leader lock release time on failure
   --advertise, --addr 							Address of the swarm manager joining the cluster. Other swarm manager(s) MUST be able to reach the swarm manager at this address. [$SWARM_ADVERTISE]
   --tls								use TLS; implied by --tlsverify=true
   --tlscacert 								trust only remotes providing a certificate signed by the CA given here
   --tlscert 								path to TLS certificate file
   --tlskey 								path to TLS key file
   --tlsverify								use TLS and verify the remote
   --engine-refresh-min-interval "30s"					set engine refresh minimum interval
   --engine-refresh-max-interval "60s"					set engine refresh maximum interval
   --engine-failure-retry "3"						set engine failure retry count
   --engine-refresh-retry "3"						deprecated; replaced by --engine-failure-retry
   --heartbeat "60s"							period between each heartbeat
   --api-enable-cors, --cors						enable CORS headers in the remote API
   --cluster-driver, -c "swarm"						cluster driver to use [swarm, mesos-experimental]
   --discovery-opt [--discovery-opt option --discovery-opt option]	discovery options
   --cluster-opt [--cluster-opt option --cluster-opt option]		cluster driver options
		 * swarm.overcommit=0.05		overcommit to apply on resources
		 * swarm.createretry=0			container create retry count after initial failure
		 * mesos.address=			address to bind on [$SWARM_MESOS_ADDRESS]
		 * mesos.checkpointfailover=false	checkpointing allows a restarted slave to reconnect with old executors and recover status updates, at the cost of disk I/O [$SWARM_MESOS_CHECKPOINT_FAILOVER]
		 * mesos.port=				port to bind on [$SWARM_MESOS_PORT]
		 * mesos.offertimeout=30s		timeout for offers [$SWARM_MESOS_OFFER_TIMEOUT]
		 * mesos.offerrefusetimeout=5s		seconds to consider unused resources refused [$SWARM_MESOS_OFFER_REFUSE_TIMEOUT]
		 * mesos.tasktimeout=5s			timeout for task creation [$SWARM_MESOS_TASK_TIMEOUT]
		 * mesos.user=				framework user [$SWARM_MESOS_USER]

rolfedlugy-hegwer at RsMBP in ~
$
