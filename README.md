# Architecture diagrams, API documentation #
[Lucidchart](https://www.lucidchart.com/) <br>
[Mermaid (diagrams from text)](https://mermaidjs.github.io/) <br>
[Cloudcraft (AWS optimized)](https://cloudcraft.co/) <br>
[Swagger](https://swagger.io/) <br>
[Cacoo](https://cacoo.com/) <br>
[Creately](https://creately.com/) <br>
[Draw](https://www.draw.io/) <br>

# Message queues #
[Kafka](https://kafka.apache.org/) <br>
[RabbitMQ](https://www.rabbitmq.com/) <br>
[ActiveMQ](http://activemq.apache.org/) <br>
[NATS](https://nats.io/) <br>
[ZeroMQ](http://zeromq.org/) <br>
[nanomsg](http://nanomsg.org/) <br>
[phxqueue (from Tencent)](https://github.com/Tencent/phxqueue) <br>
[Disque (antirez)](https://github.com/antirez/disque) (Would be part of Redis 4.2) <br>
[HornetQ](http://hornetq.jboss.org/) <br>
[IronMQ (cloud)](https://www.iron.io/platform/ironmq/) <br>

# Load balancers, reverse proxy, accelerators, web servers #
[Varnish](https://varnish-cache.org/) <br>
[HAProxy](http://www.haproxy.org/) <br>
[nginx](https://www.nginx.com/) <br>
[OpenResty](https://openresty.org/en/) <br>
[Tomcat](https://tomcat.apache.org/) <br>
[Træfik](https://traefik.io/) <br>
[Tarantool (mail.ru)](https://tarantool.org/) <br>
[lightttpd](https://www.lighttpd.net/) <br>

# Service mesh #
[Envoy L3/4/7 proxy (Lyft/Google, C++)](https://www.envoyproxy.io/) <br>
[Envoy introduction](https://www.youtube.com/watch?v=RVZX4CwKhGE) <br>
[Istio service mesh controller](https://istio.io/) <br>
[Istio introduction](https://www.youtube.com/watch?v=s4qasWn_mFc) <br>
[linkerd L5 proxy (Finagle based, JVM)](https://linkerd.io/) <br>
[linkerd introduction](https://www.youtube.com/watch?v=0xYSy6OmjUM) <br>
[Conduit (Rust, linkerd devs)](https://conduit.io/) <br>

# Structured and unstructured data storage #
[PostgreSQL](https://www.postgresql.org/) <br>
[Postgres Pro (PostgreSQL)](https://postgrespro.ru/) <br>
[JSON in Postgre 10.x, 11.x, PostgreSQL 9.6 vs Mongo 3.4](https://www.youtube.com/watch?v=SNzOZKvFZ68) <br>
[Redis](https://redis.io/) <br>
[MySQL](https://www.mysql.com/) <br>
[RocksDB (InnoDB replacement by Facebook)](http://myrocks.io/) <br>
[MariaDB (MySQL)](https://mariadb.com/) <br>
[Percona (MySQL)](https://www.percona.com/) <br>
[MongoDB](https://www.mongodb.com/) <br>
[Scylla (Cassandra on steroids)](http://www.scylladb.com/) <br>
[Cassandra](https://cassandra.apache.org/) <br>
[CockroachDB](https://www.cockroachlabs.com/) <br>
[Aerospike](http://www.aerospike.com/) <br>
[OrientDB (graph)](https://orientdb.com/) <br>

# Distributed consensus management, service discovery and configuration #
[Raft protocol](https://raft.github.io/) <br>
[Paxos protocol](https://en.wikipedia.org/wiki/Paxos_(computer_science)) <br>
[Consul](https://www.consul.io/) <br>
[etcd](https://coreos.com/etcd/) <br>
[Vault](https://www.vaultproject.io/) <br>
[Secure Production Identity Framework For Everyone (SPIFFE)](https://github.com/spiffe/spiffe) <br>
[ZooKeeper](https://zookeeper.apache.org/) <br>

# Containers #
[Docker](https://www.docker.com/) <br>
[Kubernetes](https://kubernetes.io/) <br>
[Mesosphere](https://mesosphere.com/) <br>
[Mesos](https://mesos.apache.org/) <br>
[Container Network Interface](https://github.com/containernetworking/cni) <br>
[Cilium](https://github.com/cilium/cilium) <br>
[Calico](https://www.projectcalico.org) <br>
[Vault with Kubernetes](https://github.com/Boostport/kubernetes-vault) and [Video on improvements](https://www.youtube.com/watch?v=IulNdGlQR3A) <br>
[Weave Scope (monitoring)](https://github.com/weaveworks/scope) <br>
[Telepresence (fast dev environments for Kubernetes)](https://www.telepresence.io/) <br>

# RPC, Communication between system nodes #
[gRPC](https://grpc.io/) <br>
[gRPC 2 years in production](https://www.youtube.com/watch?v=7FZ6ZyzGex0) <br>
[Protocol Buffers](https://developers.google.com/protocol-buffers/) <br>
[Thrift](https://thrift.apache.org/) <br>
[Cap'n Proto](https://capnproto.org/) <br>
[MessagePack](https://msgpack.org/) <br>
[FlatBuffers](https://google.github.io/flatbuffers/) <br>
[Motan](https://github.com/weibocom/motan) <br>
[ZeroMQ](http://zeromq.org/) <br>
[SMF](https://github.com/senior7515/smf) <br>
[QUIC](https://www.chromium.org/quic) <br>

# Service monitoring, metrics collection / graphing #
[Grafana](https://grafana.com/) <br>
[Graphite](https://graphiteapp.org/) <br>
[Prometheus](https://prometheus.io/) <br>
[NetData](https://my-netdata.io/) <br>
[okmeter](https://okmeter.io) <br>
[Datadog](https://www.datadoghq.com/) <br>
[ClichHouse](https://clickhouse.yandex/) <br>
[TimescaleDB](https://github.com/timescale/timescaledb) <br>
[Druid](http://druid.io/) <br>
[Zabbix](https://www.zabbix.com/) <br>
[PagerDuty](https://www.pagerduty.com/) <br>
[NewRelic](https://newrelic.com/) <br>

# Distributed request tracing #
[Dapper, a Large-Scale Distributed Systems Tracing Infrastructure (Google)](https://research.google.com/pubs/pub36356.html) <br>
[OpenTracing standard](http://opentracing.io/) <br>
[OpenTracing and Jaeger introduction](https://www.youtube.com/watch?v=fjYAU3jayVo) <br>
[Jaeger (Uber)](https://uber.github.io/jaeger/) <br>
[Zipkin](http://zipkin.io/) <br>
[Lightstep](https://lightstep.com) <br>
[Skywalking](http://skywalking.io/) <br>

# Log management #
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

# Feature Flags #
[Overview site](http://featureflags.io) <br>
[FF4J](http://ff4j.org/) <br>
[Togglz (Java)](https://www.togglz.org) <br>
[Unleash (simple)](https://github.com/Unleash/unleash) <br>
[LaunchDarkly (cloud provider)](https://launchdarkly.com) <br>

# Deployment tools #
[Ansible](https://ansible.com/) <br>
[Salt](https://saltstack.com/) <br>
[Puppet](https://puppet.com/) <br>
[Chef](https://www.chef.io/chef/) <br>
[Teletraan](https://github.com/pinterest/teletraan) <br>

# CI (Continuous Integration) #
[TeamCity](https://www.jetbrains.com/teamcity) <br>
[Jenkins](https://jenkins.io) <br>
[Concourse](https://concourse.ci) <br>

# CDNs #
[Akamai](https://www.akamai.com/) <br>
[Fastly](https://www.fastly.com/) <br>
[Level3](http://www.level3.com/en/products/content-delivery-network/) <br>
[Edgecast](https://www.verizondigitalmedia.com/) <br>

# AWS #
[awscli](https://aws.amazon.com/cli/) <br>
[S3 Browser](https://s3browser.com/) <br>
[CloudBerry S3 Explorer](https://www.cloudberrylab.com/explorer/amazon-s3.aspx) <br>
[Analyze AWS S3 and CloudFront logs](https://github.com/nagyv/s3stat) + [GoAccess](https://goaccess.io/) <br>

# Networking #
[How to achieve low latency with 10Gbps Ethernet (Cloudflare)](https://blog.cloudflare.com/how-to-achieve-low-latency/) <br>
[BBR, the new kid on the TCP block](https://blog.apnic.net/2017/05/09/bbr-new-kid-tcp-block/) <br>
[Making Linux TCP Fast](https://netdevconf.org/1.2/papers/bbr-netdev-1.2.new.new.pdf) <br>
[Monitoring and Tuning the Linux Networking Stack: Receiving Data](https://blog.packagecloud.io/eng/2016/06/22/monitoring-tuning-linux-networking-stack-receiving-data/) <br>
[Monitoring and Tuning the Linux Networking Stack: Sending Data](https://blog.packagecloud.io/eng/2017/02/06/monitoring-tuning-linux-networking-stack-sending-data/) <br>
[MIT's TCP ex Machina: Computer-Generated Congestion Control](http://web.mit.edu/remy/) <br>
[CoreDNS](https://github.com/coredns/coredns) <br>
[MaxMind GeoIP databases](https://dev.maxmind.com/geoip/geoip2/downloadable/) <br>
[RIPE NCC network information](https://atlas.ripe.net/) <br>
[JLS2009: Generic receive offload](https://lwn.net/Articles/358910/) <br>

# SRE (Site Reliability Engineering)
[Google Site Reliability Engineering book](https://landing.google.com/sre/book.html) <br>
[High Performance Browser Networking book](https://hpbn.co/) <br>
[The Docker Book](https://www.dockerbook.com/) <br>
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
[What every programmer should know about floating point](https://docs.oracle.com/cd/E19957-01/806-3568/ncg_goldberg.html), [Floating point GUI site](http://floating-point-gui.de/), [shorter explanation](http://blog.reverberate.org/2014/09/what-every-computer-programmer-should.html) <br>

# TLS/SSL verification #
[Sonar](https://sonarwhal.com/) <br>
[TLS information](https://istlsfastyet.com/) <br>
[Mozilla server side TLS information](https://wiki.mozilla.org/Security/Server_Side_TLS) <br>
[Mozilla Observatory](https://observatory.mozilla.org/) <br>
[HTTP security headers testing](https://securityheaders.io/) <br>
[SSL testing](https://www.ssllabs.com/ssltest) <br>
[High-Tech Bridge SSL test](https://www.htbridge.com/ssl/) <br>
[HTTP security tools](https://report-uri.io/home/tools) <br>
[HSTS preloading](https://hstspreload.org) <br>
[SRI hash generator](https://www.srihash.org/) <br>
[Client side TLS test](https://www.howsmyssl.com/) <br>
[DNS CAA helper](https://sslmate.com/caa/) <br>

# Authorization #
[The OAuth 2.0 Authorization Framework](https://tools.ietf.org/html/rfc6749) <br>
[JSON Web Token (JWT)](https://tools.ietf.org/html/rfc7519) <br>
[JSON Web Signature (JWS)](https://tools.ietf.org/html/rfc7515) <br>
[JSON Web Encryption (JWE)](https://tools.ietf.org/html/rfc7516) <br>
[JWT playground](https://jwt.io/) <br>

# Encryption, hashing #
[OpenSSL](https://www.openssl.org/) <br>
[BoringSSL (Google)](https://boringssl.googlesource.com/boringssl/) <br>
[s2n (AWS)](https://github.com/awslabs/s2n) <br>
[Cryptography Engineering: Design Principles and Practical Applications](https://www.amazon.com/Cryptography-Engineering-Principles-Practical-Applications/dp/0470474246) <br>
[Introduction to Modern Cryptography, Second Edition](https://www.amazon.com/Introduction-Cryptography-Chapman-Network-Security/dp/1466570261) <br>
[Security Engineering, 2nd edition](https://www.amazon.com/Security-Engineering-Building-Dependable-Distributed/dp/0470068523) <br>
[Ensuring Randomness with Linux's Random Number Generator](https://blog.cloudflare.com/ensuring-randomness-with-linuxs-random-number-generator/) <br>
[Should we MAC-then-encrypt or encrypt-then-MAC?](https://crypto.stackexchange.com/questions/202/should-we-mac-then-encrypt-or-encrypt-then-mac) <br>
[Authenticated Encryption: Relations among notions and analysis of the generic composition paradigm](http://cseweb.ucsd.edu/~mihir/papers/oem.html) <br>
[How to choose an Authenticated Encryption mode](https://blog.cryptographyengineering.com/2012/05/19/how-to-choose-authenticated-encryption/) <br>
[Hash-based message authentication code](https://en.wikipedia.org/wiki/Hash-based_message_authentication_code) <br>
[Authenticated Encryption with Associated Data (AEAD)](https://en.wikipedia.org/wiki/Authenticated_encryption) <br>
[AES-GCM (AEAD)](https://tools.ietf.org/html/rfc5288) <br>
[AES-GCM-SIV](https://github.com/Shay-Gueron/AES-GCM-SIV) <br>
[GCM blockcipher mode](https://en.wikipedia.org/wiki/Galois/Counter_Mode) <br>
[OCB blockcipher mode](http://web.cs.ucdavis.edu/~rogaway/ocb/) <br>
[ChaCha20 and Poly1305 (AEAD)](https://tools.ietf.org/html/rfc7539) <br>
[ChaCha20 design](http://loup-vaillant.fr/tutorials/chacha20-design) <br>
[Understanding RSA terms](https://security.stackexchange.com/questions/68822/trying-to-understand-rsa-and-its-terminology/68836#68836) <br>
[Elliptic curve introduction](https://www.imperialviolet.org/2010/12/04/ecc.html) <br>
[Elliptic Curve Cryptography: a gentle introduction](http://andrea.corbellini.name/2015/05/17/elliptic-curve-cryptography-a-gentle-introduction/) <br>
[Safe elliptic curvers](https://safecurves.cr.yp.to/) <br>
[Curve25519](https://cr.yp.to/ecdh/curve25519-20060209.pdf) <br>
[Blade2 (crypto)](https://blake2.net/) <br>
[xxHash](http://www.xxhash.com/) <br>
[MurmurHash3](https://github.com/aappleby/smhasher) <br>
[Dieharder: A Random Number Test Suite](http://webhome.phy.duke.edu/~rgb/General/dieharder.php) <br>

# Videos #
[Kafka 2017 Summit](https://www.confluent.io/kafka-summit-sf17/resource/) <br>
[CppCon 2017](https://www.youtube.com/playlist?list=PLHTh1InhhwT6bwIpRk0ZbCA0N2p1taxd6) <br>
[@Scale 2017](https://atscaleconference.com/videos-articles/) <br>
[Strange Loop 2017](https://www.youtube.com/channel/UC_QIfHvN9auy2CoOdSfMWDw) <br>

# Tools #
[htop](https://github.com/hishamhm/htop) <br>
[gtop](https://github.com/aksakalli/gtop) <br>
[k6 (load testing)](https://k6.io/) <br>
