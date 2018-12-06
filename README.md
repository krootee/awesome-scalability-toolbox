# Index
- [Architecture diagrams, API documentation](#architecture-diagrams-api-documentation)
- [Message queues](#message-queues)
- [Load balancers, reverse proxy, accelerators, web servers](#load-balancers-reverse-proxy-accelerators-web-servers)
- [Service mesh](#service-mesh)
- [Structured and unstructured data storage](#structured-and-unstructured-data-storage)
- [Distributed consensus management, service discovery and configuration](#distributed-consensus-management-service-discovery-and-configuration)
- [Containers](#containers)
- [Jsonnet](#jsonnet)
- [Kubernetes](#kubernetes)
- [RPC, Communication between system nodes](#rpc-communication-between-system-nodes)
- [gRPC](#grpc)
- [Service monitoring, metrics collection / graphing](#service-monitoring-metrics-collection--graphing)
- [Infrastructure information management](#infrastructure-information-management)
- [Distributed request tracing](#distributed-request-tracing)
- [Load testing](#load-testing)
- [Log management](#log-management)
- [Feature Flags](#feature-flags)
- [Deployment tools](#deployment-tools)
- [CI (Continuous Integration)](#ci-continuous-integration)
- [CDNs](#cdns)
- [Domain registrars](#domain-registrars)
- [AWS](#aws)
- [Networking](#networking)
- [SDN](#sdn)
- [SRE (Site Reliability Engineering)](#sre-site-reliability-engineering)
- [Disk storage](#disk-storage)
- [TLS](#tls)
- [Authorization](#authorization)
- [Encryption](#encryption)
- [Hashing](#hashing)
- [Videos](#videos)
- [Tools](#tools)
- [Misc](#misc)

# Architecture diagrams, API documentation
[Lucidchart](https://www.lucidchart.com/) <br>
[Mermaid (diagrams from text)](https://mermaidjs.github.io/) <br>
[Cloudcraft (AWS optimized)](https://cloudcraft.co/) <br>
[Swagger](https://swagger.io/) <br>
[Cacoo](https://cacoo.com/) <br>
[Creately](https://creately.com/) <br>
[Draw](https://www.draw.io/) <br>
[Wording](https://www.ietf.org/rfc/rfc2119.txt), [definition syntax](https://www.ietf.org/rfc/rfc5234.txt) and [units](http://unitsofmeasure.org/ucum.html) for RFC specification creation <br>

# Message queues
[Kafka](https://kafka.apache.org/) <br>
[RabbitMQ](https://www.rabbitmq.com/) <br>
[ActiveMQ](http://activemq.apache.org/) <br>
[ZeroMQ](http://zeromq.org/) <br>
[nanomsg](http://nanomsg.org/) <br>
[phxqueue (from Tencent)](https://github.com/Tencent/phxqueue) <br>
[Disque (antirez)](https://github.com/antirez/disque) (Would be part of Redis 4.2) <br>
[HornetQ](http://hornetq.jboss.org/) <br>
[IronMQ (cloud)](https://www.iron.io/platform/ironmq/) <br>

# Load balancers, reverse proxy, accelerators, web servers
- [Varnish](https://varnish-cache.org/)
- [HAProxy](http://www.haproxy.org/)
- [nginx](https://www.nginx.com/), [nginx config](https://nginxconfig.io/)
- [OpenResty](https://openresty.org/en/)
- [Tomcat](https://tomcat.apache.org/)
- [Træfik](https://traefik.io/)
- [Tarantool (mail.ru)](https://tarantool.org/)
- [lightttpd](https://www.lighttpd.net/)
- [katran (BPF/XDP L4 load balancer, Facebook)](https://github.com/facebookincubator/katran)
- [GitHub Load Balancer Director (GUE, ECMP, DPDK)](https://github.com/github/glb-director)

# Service mesh
- [Envoy L3/4/7 proxy (Lyft/Google, C++)](https://www.envoyproxy.io/)
- [Envoy introduction](https://www.youtube.com/watch?v=RVZX4CwKhGE)
- [Learn Envoy](https://www.learnenvoy.io/)
- [Rotor (xDS, Turbine Labs)](https://github.com/turbinelabs/rotor)
- [ModSecurity for Envoy (WAF)](https://github.com/octarinesec/ModSecurity-envoy)
- [Envoy Java control plane](https://github.com/envoyproxy/java-control-plane)
- [Istio service mesh controller](https://istio.io/)
- [Istio introduction](https://www.youtube.com/watch?v=s4qasWn_mFc)
- [linkerd L5 proxy (Finagle based, JVM)](https://linkerd.io/)
- [linkerd introduction](https://www.youtube.com/watch?v=0xYSy6OmjUM)
- [Conduit (Rust, linkerd devs)](https://conduit.io/)
- [Netflix Vizceral (observability)](https://github.com/Netflix/vizceral)
- [Kiali (observability, Istio)](https://kiali.org)
- [Vistio (observability, Istio)](https://github.com/nmnellis/vistio)

# Structured and unstructured data storage
- [PostgreSQL](https://www.postgresql.org/)
- [Postgres Pro (PostgreSQL)](https://postgrespro.ru/)
- [JSON in Postgre 10.x, 11.x, PostgreSQL 9.6 vs Mongo 3.4](https://www.youtube.com/watch?v=SNzOZKvFZ68)
- [Why Uber Engineering Switched from Postgres to MySQL](https://eng.uber.com/mysql-migration/) and [Follow up 1](https://www.slideshare.net/AlexanderKorotkov/our-answer-to-uber/), [2](https://blog.2ndquadrant.com/thoughts-on-ubers-list-of-postgres-limitations/), [3](http://thebuild.com/presentations/uber-perconalive-2017.pdf), [4](https://rhaas.blogspot.gr/2016/08/ubers-move-away-from-postgresql.html), [5](https://devconf.ru/ru/archive/devconf2017/offer/314), [6](https://habr.com/company/devconf/blog/353682/), [7](https://use-the-index-luke.com/blog/2016-07-29/on-ubers-choice-of-databases)
- [Redis](https://redis.io/), [Redis modules (Open Source)](https://goodformcode.com/)
- [Memcached](https://github.com/memcached/memcached/), [extstore storage shim](https://github.com/memcached/memcached/wiki/Extstore), [Caching beyond RAM: the case for NVMe](https://memcached.org/blog/nvm-caching/)
- [FASTER (Microsoft)](https://github.com/Microsoft/FASTER), [official site](https://www.microsoft.com/en-us/research/project/FASTER/)
- [MySQL](https://www.mysql.com/)
- [RocksDB (InnoDB replacement by Facebook)](http://myrocks.io/), [Using NVM in Facebook (RocksDB)](https://dl.acm.org/citation.cfm?id=3190524)
- [Vitess (MySQL auto horizontal scaling)](http://vitess.io/)
- [MariaDB (MySQL)](https://mariadb.com/)
- [Percona (MySQL)](https://www.percona.com/)
- [MongoDB](https://www.mongodb.com/)
- [Scylla (Cassandra on steroids)](http://www.scylladb.com/), [ScyllaDB with Optane](https://www.scylladb.com/2017/08/08/intel-optane-review/)
- [Cassandra](https://cassandra.apache.org/)
- [CockroachDB](https://www.cockroachlabs.com/)
- [Aerospike](http://www.aerospike.com/)
- [Anna (experimental, Berkeley RISE Lab)](https://github.com/fluent-project/fluent/tree/master/kvs), [white paper](https://arxiv.org/abs/1809.00089)
- [LogDevice (Facebook, distributed storage for sequential data)](https://github.com/facebookincubator/LogDevice)
- [OrientDB (graph)](https://orientdb.com/)
- [Database isolation levels](https://en.wikipedia.org/wiki/Isolation_(database_systems))
- [The Log-Structured Merge-Tree (LSM-Tree) whitepaper](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.44.2782&rep=rep1&type=pdf)
- [B+ tree](https://en.wikipedia.org/wiki/B%2B_tree)

# Distributed consensus management, service discovery and configuration
[Raft protocol](https://raft.github.io/) <br>
[Paxos protocol](https://en.wikipedia.org/wiki/Paxos_(computer_science)) <br>
[Paxos made simple](https://lamport.azurewebsites.net/pubs/paxos-simple.pdf) <br>
[Paxos Made Live - An Engineering Perspective](http://www.read.seas.harvard.edu/~kohler/class/08w-dsi/chandra07paxos.pdf) <br>
[Consul](https://www.consul.io/) <br>
[etcd](https://coreos.com/etcd/) <br>
[Vault](https://www.vaultproject.io/) <br>
[Secure Production Identity Framework For Everyone (SPIFFE)](https://github.com/spiffe/spiffe) <br>
[ZooKeeper](https://zookeeper.apache.org/) <br>

# Containers
- [Docker](https://www.docker.com/)
- [Awesome Docker list](https://github.com/veggiemonk/awesome-docker)
- [docker-autoheal (restart on unhealthy event)](https://github.com/willfarrell/docker-autoheal)
- [Kubernetes](https://kubernetes.io/)
- [Container Network Interface](https://github.com/containernetworking/cni)
- [Mesosphere](https://mesosphere.com/)
- [Mesos](https://mesos.apache.org/)
- [gVisor (sandbox runtime)](https://github.com/google/gvisor)
- [Weave Scope (monitoring)](https://github.com/weaveworks/scope)
- [SysDig (monitoring)](https://github.com/draios/sysdig)

# Jsonnet
- [jsonnet](http://jsonnet.org/)
- [jsonnet builds](https://github.com/krootee/jsonnet-releases)
- [Visual Studio Code plugin](https://github.com/heptio/vscode-jsonnet)
- [IntelliJ plugin (alpha)](https://github.com/databricks/intellij-jsonnet)
- [Style guide (Databricks)](https://github.com/databricks/jsonnet-style-guide)

# Kubernetes
[Kompose (Docker Compose to k8s)](http://kompose.io/) <br>
[ksonnet](https://ksonnet.io/) <br>
[kubecfg](https://github.com/ksonnet/kubecfg) <br>
[Kubespray (cluster setup)](https://kubespray.io/) <br>
[Kubeadm (cluster setup)](https://github.com/kubernetes/kubeadm) <br>
[kops (cluster setup)](https://github.com/kubernetes/kops) <br>
[kubectx & kubens (switch clusters and namespaces](https://github.com/ahmetb/kubectx) <br>
[kube-ps1 (prompt info)](https://github.com/jonmosco/kube-ps1) <br>
[stern (pod and container tailing)](https://github.com/wercker/stern) <br>
[click (cli controller)](https://github.com/databricks/click) <br>
[prow (Github hooks)](https://github.com/kubernetes/test-infra/tree/master/prow) <br>
[KubeGPU (Microsoft)](https://github.com/Microsoft/KubeGPU) <br>
[Skaffold](https://github.com/GoogleCloudPlatform/skaffold) <br>
[K8s management tools](https://docs.google.com/spreadsheets/u/1/d/1FCgqz1Ci7_VCz_wdh8vBitZ3giBtac_H8SBw4uxnrsE/htmlview#gid=0) <br>
[Telepresence (fast dev environments)](https://www.telepresence.io/) <br>
[Squash microservice debugger](https://github.com/solo-io/squash) <br>
[AWS VPC Kubernetes CNI driver using IPvlan](https://github.com/lyft/cni-ipvlan-vpc-k8s) <br>
[Helm (package manager)](https://helm.sh/) <br>
[Kedge (Simple, Concise & Declarative Kubernetes Applications)](http://kedgeproject.org/) <br>
[Contour (Ingress controller using Envoy)](https://github.com/heptio/contour) <br>
[Gimbal (Ingress load balancer to many clusters)](https://github.com/heptio/gimbal) <br>
[Cilium](https://github.com/cilium/cilium) <br>
[Calico](https://www.projectcalico.org) <br>
[Vault with Kubernetes](https://github.com/Boostport/kubernetes-vault) and [Video on improvements](https://www.youtube.com/watch?v=IulNdGlQR3A) <br>
[Gitkube](https://gitkube.sh/) <br>
[Guide to Kubernetes networking (part 1)](https://medium.com/@ApsOps/an-illustrated-guide-to-kubernetes-networking-part-1-d1ede3322727), [Part 2](https://medium.com/@ApsOps/an-illustrated-guide-to-kubernetes-networking-part-2-13fdc6c4e24c) <br>
[Kubernetes Security - Best Practice Guide](https://github.com/freach/kubernetes-security-best-practice) <br>
[Weave Scope](https://github.com/weaveworks/scope/) <br>
[Kubernetic (desktop UI client)](https://kubernetic.com/) <br>
[50 Useful Kubernetes Tools](https://caylent.com/50-useful-kubernetes-tools/) <br>

# RPC, Communication between system nodes
[gRPC](https://grpc.io/) <br>
[Dubbo (China version of gRPC)](https://dubbo.apache.org) <br>
[Protocol Buffers](https://developers.google.com/protocol-buffers/) <br>
[Thrift](https://thrift.apache.org/) <br>
[Cap'n Proto](https://capnproto.org/) <br>
[MessagePack](https://msgpack.org/) <br>
[FlatBuffers](https://google.github.io/flatbuffers/) <br>
[Motan](https://github.com/weibocom/motan) <br>
[Aeron](https://github.com/real-logic/aeron) <br>
[ZeroMQ](http://zeromq.org/) <br>
[SMF](https://github.com/senior7515/smf) <br>
[QUIC](https://www.chromium.org/quic) <br>

# gRPC
- [Awesome gRPC list](https://github.com/grpc-ecosystem/awesome-grpc)
- [gRPC status codes](https://github.com/grpc/grpc/blob/master/doc/statuscodes.md)
- [gRPC 2 years in production](https://www.youtube.com/watch?v=7FZ6ZyzGex0)
- [gRPC-Web client](https://github.com/improbable-eng/grpc-web/)

# Service monitoring, metrics collection / graphing
- [Grafana](https://grafana.com/)
- [Grafonnet-lib (generate dashboards for Grafana)](https://github.com/grafana/grafonnet-lib)
- [Graphite](https://graphiteapp.org/)
- [Prometheus](https://prometheus.io/)
- [OpenMetrics](https://github.com/OpenObservability/OpenMetrics)
- [eBPF exporter (Prometheus)](https://github.com/cloudflare/ebpf_exporter)
- [Node Exporter (Prometheus)](https://github.com/prometheus/node_exporter)
- [cAdvisor (container monitoring)](https://github.com/google/cadvisor)
- [ClichHouse (Yandex)](https://clickhouse.yandex/)
- [Druid (Imply)](http://druid.io/)
- [Pinot (Linkedin)](https://github.com/linkedin/pinot/)
- [Architecture analysis of ClickHouse, Druid and Pinot](https://medium.com/@leventov/comparison-of-the-open-source-olap-systems-for-big-data-clickhouse-druid-and-pinot-8e042a5ed1c7)
- [HTTP Analytics for 6M requests per second using ClickHouse](https://blog.cloudflare.com/http-analytics-for-6m-requests-per-second-using-clickhouse/)
- [NetData](https://my-netdata.io)
- [Vector (on-host monitoring)](http://vectoross.io)
- [okmeter](https://okmeter.io)
- [Datadog](https://www.datadoghq.com)
- [TimescaleDB](https://github.com/timescale/timescaledb)
- [KairosDB](https://kairosdb.github.io)
- [Zabbix](https://www.zabbix.com)
- [PagerDuty](https://www.pagerduty.com)
- [NewRelic](https://newrelic.com)

# Infrastructure information management
[Osquery (Facebook)](https://osquery.io/) <br>
[Kolide Fleet (osquery)](http://www.kolide.co/fleet) <br>
[Doorman (osquery)](https://github.com/mwielgoszewski/doorman) <br>
[OSSEC](https://ossec.github.io/) <br>

# Distributed request tracing
[Dapper, a Large-Scale Distributed Systems Tracing Infrastructure (Google)](https://research.google.com/pubs/pub36356.html) <br>
[OpenTracing standard](http://opentracing.io/) <br>
[OpenTracing and Jaeger introduction](https://www.youtube.com/watch?v=fjYAU3jayVo) <br>
[OpenCensus (Google, tracing and stats)](http://opencensus.io/) <br>
[TraceContext propagation format](https://github.com/w3c/distributed-tracing) <br>
[Jaeger (Uber)](https://uber.github.io/jaeger/) <br>
[Zipkin](http://zipkin.io/) <br>
[Lightstep](https://lightstep.com) <br>
[Skywalking](http://skywalking.io/) <br>

# Load testing
[Yandex.Tank (C++, Python, Go)](https://github.com/yandex/yandex-tank) <br>
[Overload (storage for Yandex.Tank results)](https://overload.yandex.net) <br>
[Gatling (Scala)](https://gatling.io/) <br>
[Locust (Python)](https://locust.io/) <br>
[Vegeta (HTTP 1.1/2)](https://github.com/tsenart/vegeta) <br>
[h2load (HTTP 1.1/2)](https://nghttp2.org/documentation/h2load.1.html) <br>
[Selenium (Web UI)](http://www.seleniumhq.org/) <br>
[Selenide (Web UI)](http://selenide.org/) <br>

# Log management
[What you need to know about real-time logs](https://engineering.linkedin.com/distributed-systems/log-what-every-software-engineer-should-know-about-real-time-datas-unifying) <br>
[fluentd](https://www.fluentd.org/) <br>
[Kafka](https://kafka.apache.org/) <br>
[Logstash](https://www.elastic.co/products/logstash) <br>
[Graylog2](https://www.graylog.org/) <br>
[syslog-ng](https://syslog-ng.org/) <br>
[rsyslog](http://www.rsyslog.com/) <br>
[Splunk](https://www.splunk.com/) <br>
[GoAccess](https://goaccess.io/) <br>
[Bookkeeper](https://bookkeeper.apache.org/distributedlog/) <br>
[LogDevice (Facebook)](https://code.facebook.com/posts/357056558062811/logdevice-a-distributed-data-store-for-logs/) <br>
Online solutions: <br>
[Loggly](https://www.loggly.com/) <br>
[Logentries](https://logentries.com/) <br>
[Papertrail](https://papertrailapp.com/) <br>
[Scalyr](https://www.scalyr.com/) <br>
[Sumo Logic](https://www.sumologic.com/) <br>
[Humio](https://humio.com/) <br>

# Feature Flags
[Overview site](http://featureflags.io) <br>
[FF4J](http://ff4j.org/) <br>
[Togglz (Java)](https://www.togglz.org) <br>
[Unleash (simple)](https://github.com/Unleash/unleash) <br>
[LaunchDarkly (cloud provider)](https://launchdarkly.com) <br>

# Deployment tools
[Ansible](https://ansible.com/) <br>
[Salt](https://saltstack.com/) <br>
[Puppet](https://puppet.com/) <br>
[Chef](https://www.chef.io/chef/) <br>
[Teletraan](https://github.com/pinterest/teletraan) <br>

# CI (Continuous Integration)
[TeamCity](https://www.jetbrains.com/teamcity) <br>
[Jenkins](https://jenkins.io) <br>
[Jenkins X (for k8s apps)](https://jenkins-x.io/) <br>
[Concourse](https://concourse.ci) <br>

# CDNs
[Akamai](https://www.akamai.com/) <br>
[Fastly](https://www.fastly.com/) <br>
[Level3](http://www.level3.com/en/products/content-delivery-network/) <br>
[Edgecast](https://www.verizondigitalmedia.com/) <br>
[Traffic Control (Self-hosted CDN)](https://trafficcontrol.apache.org/) <br>

# Domain registrars
- [MarkMonitor](https://www.markmonitor.com/)
- [Cloudflare](https://www.cloudflare.com/registrar/)

# AWS
- [awscli](https://aws.amazon.com/cli/)
- [awless](https://github.com/wallix/awless)
- [S3 Browser](https://s3browser.com/)
- [CloudBerry S3 Explorer](https://www.cloudberrylab.com/explorer/amazon-s3.aspx)
- [Analyze S3 speed from your location](https://cloudharmony.com/speedtest-for-aws:s3)
- [Analyze AWS S3 and CloudFront logs](https://github.com/nagyv/s3stat) + [GoAccess](https://goaccess.io/)
- [EC2 instance cheat sheet](https://www.ec2instances.info/)
- [S3 meta information](https://github.com/whitfin/s3-meta)

# Networking
[BPF introduction](https://qmonnet.github.io/whirl-offload/2016/09/01/dive-into-bpf/) <br>
[XDP](https://www.iovisor.org/technology/xdp) <br>
[BPFd (remote BPF by Google)](https://github.com/joelagnel/bpfd) <br>
[bpftrace (high-level langauge for writing eBPF programs)](https://github.com/iovisor/bpftrace) <br>
[BCC (Tools for BPF-based Linux IO analysis, networking, monitoring, and more)](https://github.com/iovisor/bcc) <br>
[How to achieve low latency with 10Gbps Ethernet (Cloudflare)](https://blog.cloudflare.com/how-to-achieve-low-latency/) <br>
[BBR: Congestion-based congestion control](https://blog.acolyer.org/2017/03/31/bbr-congestion-based-congestion-control/), [BBR, the new kid on the TCP block](https://blog.apnic.net/2017/05/09/bbr-new-kid-tcp-block/) <br>
[Making Linux TCP Fast](https://netdevconf.org/1.2/papers/bbr-netdev-1.2.new.new.pdf) <br>
[SYN packet handling in the wild (Cloudflare)](https://blog.cloudflare.com/syn-packet-handling-in-the-wild/) <br>
[How TCP backlog works in Linux](https://veithen.github.io/2014/01/01/how-tcp-backlog-works-in-linux.html) <br>
[Understanding TCP close states](https://benohead.com/tcp-about-fin_wait_2-time_wait-and-close_wait/) <br>
[Bind before connect](https://idea.popcount.org/2014-04-03-bind-before-connect/) <br>
[SYNC Cookies](https://www.giac.org/paper/gsec/2013/syn-cookies-exploration/103486) <br>
[On SO_REUSEADDR and SO_REUSEPORT](https://stackoverflow.com/questions/14388706/socket-options-so-reuseaddr-and-so-reuseport-how-do-they-differ-do-they-mean-t/14388707#14388707) <br>
[On Linux history of poll(), select() and epoll()](https://idea.popcount.org/2017-02-20-epoll-is-fundamentally-broken-12/), [More on Linux epoll](https://habr.com/post/416669/) <br>
[Monitoring and Tuning the Linux Networking Stack: Receiving Data](https://blog.packagecloud.io/eng/2016/06/22/monitoring-tuning-linux-networking-stack-receiving-data/) <br>
[Monitoring and Tuning the Linux Networking Stack: Sending Data](https://blog.packagecloud.io/eng/2017/02/06/monitoring-tuning-linux-networking-stack-sending-data/) <br>
[MIT's TCP ex Machina: Computer-Generated Congestion Control](http://web.mit.edu/remy/) <br>
[Introduction to modern network load balancing and proxying (Envoy)](https://blog.envoyproxy.io/introduction-to-modern-network-load-balancing-and-proxying-a57f6ff80236) <br>
[BGP in 2017](http://www.potaroo.net/ispcol/2018-01/bgp2017.html) <br>
[CoreDNS](https://github.com/coredns/coredns) <br>
[Knot DNS](https://gitlab.labs.nic.cz/knot/knot-dns) <br>
[Knot Resolver](https://gitlab.labs.nic.cz/knot/knot-resolver) <br>
[Maglev: A Fast and Reliable Software Network Load Balancer](https://research.google.com/pubs/pub44824.html) <br>
[MaxMind GeoIP databases](https://dev.maxmind.com/geoip/geoip2/downloadable/) <br>
[IPVS](http://www.linuxvirtualserver.org/software/ipvs.html) <br>
[Open vSwitch](http://www.openvswitch.org/) <br>
[kTLS in Linux (TLS in kernel space 4.13+)](https://github.com/ktls), [white paper](https://netdevconf.org/1.2/papers/ktls.pdf) and [Intro in Go](https://blog.filippo.io/playing-with-kernel-tls-in-linux-4-13-and-go/)<br>
[DPDK](http://dpdk.org/) <br>
[FD.io](https://fd.io/) <br>
[RIPE NCC network information](https://atlas.ripe.net/) <br>
[JLS2009: Generic receive offload](https://lwn.net/Articles/358910/) <br>
[High-Speed Trading: Lines, Radios, and Cables – Oh My](https://tabbforum.com/opinions/high-speed-trading-lines-radios-and-cables-oh-my) <br>
[Solving problem with Nagle's algorithm and delayed ACK using TCP_NODELAY](http://www.stuartcheshire.org/papers/NagleDelayedAck/) <br>
[IPFS](https://ipfs.io/) <br>
[S/Kademlia: A Practicable Approach Towards Secure Key-Based Routing](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.68.4986) <br>
[Linux AnyIP](https://blog.widodh.nl/2016/04/anyip-bind-a-whole-subnet-to-your-linux-machine/) <br>
[Listen on all ports for AnyIP range on the server](https://blog.cloudflare.com/how-we-built-spectrum/) <br>
[TCP Tracepoints (Linux 4.15/6+)](http://www.brendangregg.com/blog/2018-03-22/tcp-tracepoints.html) <br>
[Kernel Connection Multiplexor (KCM)](https://lwn.net/Articles/657970/) and [more details](https://lwn.net/Articles/657999/) <br>
[Blocking-resistant communication through domain fronting](https://www.bamsoftware.com/papers/fronting/) <br>
[Anatomy of Linux DNS lookup](https://zwischenzugs.com/2018/06/08/anatomy-of-a-linux-dns-lookup-part-i/), [part 2](https://zwischenzugs.com/2018/06/18/anatomy-of-a-linux-dns-lookup-part-ii/), [part 3](https://zwischenzugs.com/2018/07/06/anatomy-of-a-linux-dns-lookup-part-iii/), [part 4](https://zwischenzugs.com/2018/08/06/anatomy-of-a-linux-dns-lookup-part-iv/), [part 5](https://zwischenzugs.com/2018/09/13/anatomy-of-a-linux-dns-lookup-part-v-two-debug-nightmares/) <br>
[Equal-cost multi-path routing (ECMP)](https://en.wikipedia.org/wiki/Equal-cost_multi-path_routing) <br>
[How LinkedIn used TCP Anycast to make the site faster](https://www.slideshare.net/shawnzandi/how-linkedin-used-tcp-anycast-to-make-the-site-faster) <br>
[Roughtime protocol](https://roughtime.googlesource.com/roughtime) <br>

# SDN
[Stratum](https://stratumproject.org/) <br>
[p4 language](https://p4.org/) <br>
[p4 Runtime](https://p4.org/p4-runtime/) <br>
[OpenFlow](https://www.opennetworking.org/software-defined-standards/specifications/) <br>
[SAI (Switch Abstraction Interface)](https://github.com/opencomputeproject/SAI) <br>
[ONOS](https://onosproject.org/) <br>
[OpenNFP](https://open-nfp.org/) <br>
[OpenConfig](http://openconfig.net/) <br>

# SRE (Site Reliability Engineering)
[Google Site Reliability Engineering book](https://landing.google.com/sre/book.html) <br>
[High Performance Browser Networking book](https://hpbn.co/) <br>
[The Docker Book](https://www.dockerbook.com/) <br>
[Site Reliability Engineer HandBook](https://s905060.gitbooks.io/site-reliability-engineer-handbook/) <br>
[Linux Performance tools and materials](http://www.brendangregg.com/linuxperf.html) <br>
[U2F devices review](https://github.com/hillbrad/U2FReviews) <br>
[A self-service CA for OpenSSH](https://github.com/nsheridan/cashier) <br>
[Optimizing web servers for high throughput and low latency (Dropbox)](https://blogs.dropbox.com/tech/2017/09/optimizing-web-servers-for-high-throughput-and-low-latency/) <br>
[Shipilev Close Encounters of The Java Memory Model Kind](https://shipilev.net/blog/2016/close-encounters-of-jmm-kind/) <br>
[Shipilev JVM Anatomy Park](https://shipilev.net/jvm-anatomy-park/) <br>
[On disk IO - part 1](https://medium.com/@ifesdjeen/on-disk-io-part-1-flavours-of-io-8e1ace1de017), [part 2](https://medium.com/@ifesdjeen/on-disk-io-part-2-more-flavours-of-io-c945db3edb13), [part 3](https://medium.com/@ifesdjeen/on-disk-io-part-3-lsm-trees-8b2da218496f), [part 4](https://medium.com/@ifesdjeen/on-disk-storage-part-4-b-trees-30791060741), [part 5](https://medium.com/@ifesdjeen/on-disk-io-access-patterns-in-lsm-trees-2ba8dffc05f9) <br>
[Transparent Hugepages: measuring the performance impact](https://alexandrnikitin.github.io/blog/transparent-hugepages-measuring-the-performance-impact/) <br>
[Introduction 2016 NUMA Deep Dive Series](http://frankdenneman.nl/2016/07/06/introduction-2016-numa-deep-dive-series/) <br>
[Understanding PCIe Configuration for Maximum Performance](https://community.mellanox.com/docs/DOC-2496) <br>
[Netflix Serving 100 Gbps from an Open Connect Appliance](https://medium.com/netflix-techblog/serving-100-gbps-from-an-open-connect-appliance-cdb51dda3b99) <br>
[Aphyr Hermitage - info and testing of database isolation levels](https://github.com/aphyr/hermitage) <br>
[A collection of postmortems](https://github.com/danluu/post-mortems) <br>
[Jeff Dean's latency numbers plotted over time](https://github.com/colin-scott/interactive_latencies) <br>
[Sakila test DB](https://dev.mysql.com/doc/sakila/en/) <br>
[Monitoring in the time of Cloud Native](https://medium.com/@copyconstruct/monitoring-in-the-time-of-cloud-native-c87c7a5bfa3e) <br>
[Tyler McMullen - Load Balancing is Impossible](https://www.youtube.com/watch?v=kpvbOzHUakA) <br>
[What every programmer should know about memory](https://www.akkadia.org/drepper/cpumemory.pdf) <br>
[What every programmer should know about floating point](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html), [floating points format explained](http://fabiensanglard.net/floating_point_visually_explained/), [Floating point GUI site](http://floating-point-gui.de/), [shorter explanation](http://blog.reverberate.org/2014/09/what-every-computer-programmer-should.html) <br>
[Chaos Engineering information map](https://coggle.it/diagram/5a229c7860c0c20001ae6caf/1960e86c369b09c4deac3227885bb073ae258e637b1b9e57be274125ac6e57b2) <br>
[A Gentle Introduction to Erasure Codes](https://www.akalin.com/intro-erasure-codes) <br>
[The PMCs of EC2: Measuring IPC](http://www.brendangregg.com/blog/2017-05-04/the-pmcs-of-ec2.html) <br>
[AWS EC2 Virtualization evolution](http://www.brendangregg.com/blog/2017-11-29/aws-ec2-virtualization-2017.html) <br>
[DNS zone visualization](http://dnsviz.net/) <br>
[How Netflix Tunes EC2](http://www.brendangregg.com/blog/2017-12-31/reinvent-netflix-ec2-tuning.html) <br>
[Write-Behind Logging](http://www.vldb.org/pvldb/vol10/p337-arulraj.pdf) <br>
[Cache-Oblivious Algorithms and Data Structures](http://erikdemaine.org/papers/BRICS2002/paper.pdf) <br>
[Oracle Graal (Hotspot replacement)](https://github.com/oracle/graal) <br>
[Understanding How Graal Works - a Java JIT Compiler Written in Java](http://chrisseaton.com/truffleruby/jokerconf17/) <br>
[Understanding disk usage in Linux](https://ownyourbits.com/2018/05/02/understanding-disk-usage-in-linux/) <br>
[On time and UTC](https://zachholman.com/talk/utc-is-enough-for-everyone-right) <br>
[The tail at scale (reducing latency long tail)](https://www2.cs.duke.edu/courses/cps296.4/fall13/838-CloudPapers/dean_longtail.pdf) <br>
[Optimizing ScyllaDB to run inside Docker container](https://www.scylladb.com/2018/08/09/cost-containerization-scylla/) <br>

# Disk storage
[libzbc (direct disk access)](https://github.com/hgst/libzbc) <br>
[SMR drives at Dropbox](https://blogs.dropbox.com/tech/2018/06/extending-magic-pocket-innovation-with-the-first-petabyte-scale-smr-drive-deployment/) <br>
[Intel VROC overview and performance testing](https://www.storagereview.com/intel_virtual_raid_on_cpu_vroc_review) <br>
[Blb (distributed object storage system developed by Upthere)](https://github.com/westerndigitalcorporation/blb) <br>

# TLS
- [The Illustrated TLS Connection](https://tls.ulfheim.net/)
- [Sonar](https://sonarwhal.com/)
- [TLS information](https://istlsfastyet.com/)
- [Mutuals TLS (mTLS)](https://www.codeproject.com/Articles/326574/An-Introduction-to-Mutual-SSL-Authentication)
- [Mozilla server side TLS information](https://wiki.mozilla.org/Security/Server_Side_TLS)
- [testssl.sh](https://github.com/drwetter/testssl.sh)
- [Mozilla Observatory](https://observatory.mozilla.org/)
- [HTTP security headers testing](https://securityheaders.io/)
- [Qualys SSL tests](https://www.ssllabs.com/ssltest)
- [High-Tech Bridge SSL test](https://www.htbridge.com/ssl/)
- [HTTP security tools](https://report-uri.io/home/tools)
- [HSTS preloading](https://hstspreload.org)
- [SRI hash generator](https://www.srihash.org/)
- [Client side TLS test](https://www.howsmyssl.com/)
- [DNS CAA helper](https://sslmate.com/caa/)
- [DNS over TLS](https://tools.ietf.org/html/rfc7858)
- [Encrypted SNI standard](https://tools.ietf.org/html/draft-ietf-tls-esni-01)

# Authorization
- [The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749)
- [OAuth 2.0 introduction](https://github.com/trimstray/sandmap)
- [JSON Web Token (JWT)](https://tools.ietf.org/html/rfc7519)
- [JSON Web Signature (JWS)](https://tools.ietf.org/html/rfc7515)
- [JSON Web Encryption (JWE)](https://tools.ietf.org/html/rfc7516)
- [JWT playground](https://jwt.io/)

# Encryption
[OpenSSL](https://www.openssl.org/) <br>
[BoringSSL (Google)](https://boringssl.googlesource.com/boringssl/) <br>
[s2n (AWS)](https://github.com/awslabs/s2n) <br>
[LibreSSL (OpenBSD OpenSSL fork)](https://github.com/libressl-portable/portable) <br>
[Google Tink](https://github.com/google/tink) <br>
[Thesis (encryption framework)](https://github.com/cossacklabs/themis) <br>
[Acra (DB encryption proxy)](https://github.com/cossacklabs/acra) <br>
[Cryptography Engineering: Design Principles and Practical Applications (book)](https://www.amazon.com/Cryptography-Engineering-Principles-Practical-Applications/dp/0470474246) <br>
[Introduction to Modern Cryptography, Second Edition (book)](https://www.amazon.com/Introduction-Cryptography-Chapman-Network-Security/dp/1466570261) <br>
[Security Engineering, 2nd edition (book)](https://www.amazon.com/Security-Engineering-Building-Dependable-Distributed/dp/0470068523) <br>
[Crypto 101 (concepts, book)](https://www.crypto101.io/) <br>
[Applied Cryptography Engineering](https://sockpuppet.org/blog/2013/07/22/applied-practical-cryptography/) <br>
[Ensuring Randomness with Linux's Random Number Generator](https://blog.cloudflare.com/ensuring-randomness-with-linuxs-random-number-generator/) <br>
[Should we MAC-then-encrypt or encrypt-then-MAC?](https://crypto.stackexchange.com/questions/202/should-we-mac-then-encrypt-or-encrypt-then-mac) <br>
[Authenticated Encryption: Relations among notions and analysis of the generic composition paradigm](http://cseweb.ucsd.edu/~mihir/papers/oem.html) <br>
[How to choose an Authenticated Encryption mode](https://blog.cryptographyengineering.com/2012/05/19/how-to-choose-authenticated-encryption/) <br>
[Awesome cryptography repository](https://github.com/sobolevn/awesome-cryptography) <br>
[Mind Your Keys? A Security Evaluation of Java Keystores](http://wp.internetsociety.org/ndss/wp-content/uploads/sites/25/2018/02/ndss2018_02B-1_Focardi_paper.pdf) <br>
[Hash-based message authentication code](https://en.wikipedia.org/wiki/Hash-based_message_authentication_code) <br>
[Authenticated Encryption with Associated Data (AEAD)](https://en.wikipedia.org/wiki/Authenticated_encryption) <br>
[AES-GCM (AEAD)](https://tools.ietf.org/html/rfc5288) <br>
[AES-GCM-SIV](https://github.com/Shay-Gueron/AES-GCM-SIV) <br>
[GCM blockcipher mode](https://en.wikipedia.org/wiki/Galois/Counter_Mode) <br>
[OCB blockcipher mode](http://web.cs.ucdavis.edu/~rogaway/ocb/) <br>
[ChaCha20 design (stream)](http://loup-vaillant.fr/tutorials/chacha20-design) <br>
[Poly1305 (MAC)](https://cr.yp.to/mac.html) <br>
[ChaCha20 and Poly1305 (AEAD)](https://tools.ietf.org/html/rfc7539) <br>
[Understanding RSA terms](https://security.stackexchange.com/questions/68822/trying-to-understand-rsa-and-its-terminology/68836#68836) <br>
[Elliptic curve introduction](https://www.imperialviolet.org/2010/12/04/ecc.html) <br>
[Elliptic Curve Cryptography: a gentle introduction](http://andrea.corbellini.name/2015/05/17/elliptic-curve-cryptography-a-gentle-introduction/) <br>
[Safe elliptic curvers](https://safecurves.cr.yp.to/) <br>
[Curve25519](https://cr.yp.to/ecdh/curve25519-20060209.pdf) <br>

# Hashing
- [smhasher testing suite](https://github.com/rurban/smhasher)
- [Fast Positive Hash](https://github.com/leo-yuriev/t1ha)
- [Meow hash](https://github.com/cmuratori/meow_hash)
- [HighwayHash and SipHash (Google)](https://github.com/google/highwayhash/)
- [SipHash (original)](https://131002.net/siphash/)
- [Blade2 (crypto)](https://blake2.net/)
- [xxHash](http://www.xxhash.com/)
- [MurmurHash3](https://github.com/aappleby/smhasher)
- [Dieharder: A Random Number Test Suite](http://webhome.phy.duke.edu/~rgb/General/dieharder.php)

# Videos
- [Kafka 2017 Summit](https://www.confluent.io/kafka-summit-sf17/resource/) <br>
- [CppCon 2017](https://www.youtube.com/playlist?list=PLHTh1InhhwT6bwIpRk0ZbCA0N2p1taxd6) <br>
- [@Scale 2017](https://atscaleconference.com/videos-articles/) <br>
- [Strange Loop 2017](https://www.youtube.com/channel/UC_QIfHvN9auy2CoOdSfMWDw) <br>
- [FOSDEM 2018](https://www.youtube.com/user/fosdemtalks/videos) <br>
- [Computer Architecture course taught at ETH Zürich in Fall 2017](https://www.youtube.com/playlist?list=PL5Q2soXY2Zi9OhoVQBXYFIZywZXCPl4M_) <br>
- [GrafanaCon 2018](https://www.youtube.com/playlist?list=PLDGkOdUX1UjpXR6BexaDoOIc0ksE2MzFI) <br>
- [SREcon 2018](https://www.youtube.com/playlist?list=PLbRoZ5Rrl5lcszsvhnb4P9Ds4pSmVtkfp) <br>
- [KubeCon + CloudNativeCon 2018](https://www.youtube.com/playlist?list=PLj6h78yzYM2N8GdbjmhVU65KYm_68qBmo)
- [Networking @Scale 2018](https://code.fb.com/core-data/networking-scale-2018-recap/)

# Tools
- [htop](https://github.com/hishamhm/htop)
- [gtop](https://github.com/aksakalli/gtop)
- [nvtop](https://github.com/Syllo/nvtop)
- [k6 (load testing)](https://k6.io/)
- [dnstrace](https://github.com/rs/dnstrace)
- [upx](https://upx.github.io/)
- [bat](https://github.com/sharkdp/bat)
- [httpie](https://github.com/jakubroztocil/httpie)
- [smenu](https://github.com/p-gen/smenu)
- [awesome tmux](https://github.com/rothgar/awesome-tmux)
- [py-spy (python profiler)](https://github.com/benfred/py-spy)
- [kubespy](https://github.com/pulumi/kubespy)
- [up](https://github.com/akavel/up)
- [doh](https://github.com/picatz/doh)
- [fx](https://github.com/antonmedv/fx)
- [jid](https://github.com/simeji/jid)
- [dive](https://github.com/wagoodman/dive)
- [nnn](https://github.com/jarun/nnn)
- [ethr](https://github.com/Microsoft/Ethr)

# Misc
[High Scalability/Availability/Stability articles list](https://github.com/binhnguyennus/awesome-scalability) <br>
[Another github repo](https://github.com/rShetty/awesome-distributed-systems) <br>
