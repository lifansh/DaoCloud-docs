# Mirror acceleration station

Many mirrors are located overseas, such as gcr. Downloading from these mirrors from within China can be very slow and requires acceleration.

DaoCloud provides a domestic mirror acceleration service that makes it easy to pull these images from within China.

## How to use

- Add a prefix (recommended):

    ```bash
    k8s.gcr.io/coredns/coredns => m.daocloud.io/k8s.gcr.io/coredns/coredns
    ```

- Modify the prefix of the image repository:

    ```bash
    k8s.gcr.io/coredns/coredns => k8s-gcr.m.daocloud.io/coredns/coredns
    ```

## Supported image list

At present, DaoCloud has collected more than 600 overseas images for the convenience of Chinese users. You can always [provide PR](https://github.com/DaoCloud/public-image-mirror/pulls) to add more mirror addresses.

??? note "Click here to see the included mirror images."

    ```bash
    docker.elastic.co/eck/eck-operator
    docker.elastic.co/elasticsearch/elasticsearch
    docker.elastic.co/kibana/kibana
    docker.elastic.co/kibana/kibana-oss
    docker.io/alpine
    docker.io/alpine/helm
    docker.io/amazon/aws-alb-ingress-controller
    docker.io/amazon/aws-ebs-csi-driver
    docker.io/apache/skywalking-java-agent
    docker.io/apache/skywalking-oap-server
    docker.io/apache/skywalking-ui
    docker.io/aquasec/kube-bench
    docker.io/aquasec/kube-hunter
    docker.io/aquasec/trivy
    docker.io/arey/mysql-client
    docker.io/bitnami/bitnami-shell
    docker.io/bitnami/contour
    docker.io/bitnami/elasticsearch
    docker.io/bitnami/elasticsearch-curator
    docker.io/bitnami/elasticsearch-exporter
    docker.io/bitnami/envoy
    docker.io/bitnami/grafana
    docker.io/bitnami/grafana-operator
    docker.io/bitnami/kubeapps-apis
    docker.io/bitnami/kubeapps-apprepository-controller
    docker.io/bitnami/kubeapps-dashboard
    docker.io/bitnami/kubeapps-kubeops
    docker.io/bitnami/kubectl
    docker.io/bitnami/kubernetes-event-exporter
    docker.io/bitnami/mariadb
    docker.io/bitnami/minideb
    docker.io/bitnami/nginx
    docker.io/bitnami/postgresql
    docker.io/bitnami/wordpress
    docker.io/bitpoke/mysql-operator
    docker.io/bitpoke/mysql-operator-orchestrator
    docker.io/bitpoke/mysql-operator-sidecar-5.7
    docker.io/bitpoke/mysql-operator-sidecar-8.0
    docker.io/busybox
    docker.io/byrnedo/alpine-curl
    docker.io/caddy
    docker.io/calico/apiserver
    docker.io/calico/cni
    docker.io/calico/csi
    docker.io/calico/kube-controllers
    docker.io/calico/node
    docker.io/calico/node-driver-registrar
    docker.io/calico/pod2daemon-flexvol
    docker.io/calico/typha
    docker.io/cdkbot/hostpath-provisioner-amd64
    docker.io/cdkbot/registry-amd64
    docker.io/centos
    docker.io/cfmanteiga/alpine-bash-curl-jq
    docker.io/cfssl/cfssl
    docker.io/cilium/json-mock
    docker.io/clickhouse/clickhouse-server
    docker.io/clickhouse/integration-helper
    docker.io/cloudnativelabs/kube-router
    docker.io/coredns/coredns
    docker.io/csiplugin/snapshot-controller
    docker.io/curlimages/curl
    docker.io/datawire/ambassador
    docker.io/datawire/ambassador-operator
    docker.io/debian
    docker.io/directxman12/k8s-prometheus-adapter
    docker.io/docker
    docker.io/elastic/filebeat
    docker.io/envoyproxy/envoy
    docker.io/envoyproxy/envoy-distroless
    docker.io/envoyproxy/nighthawk-dev
    docker.io/f5networks/f5-ipam-controller
    docker.io/f5networks/k8s-bigip-ctlr
    docker.io/fabulousjohn/kafka-manager
    docker.io/falcosecurity/event-generator
    docker.io/falcosecurity/falco-driver-loader
    docker.io/falcosecurity/falco-exporter
    docker.io/falcosecurity/falco-no-driver
    docker.io/falcosecurity/falcosidekick
    docker.io/falcosecurity/falcosidekick-ui
    docker.io/fellah/gitbook
    docker.io/flannelcni/flannel-cni-plugin
    docker.io/flant/shell-operator
    docker.io/fluent/fluent-bit
    docker.io/fluent/fluentd
    docker.io/fortio/fortio
    docker.io/foxdalas/kafka-manager
    docker.io/frrouting/frr
    docker.io/goharbor/chartmuseum-photon
    docker.io/goharbor/harbor-core
    docker.io/goharbor/harbor-db
    docker.io/goharbor/harbor-exporter
    docker.io/goharbor/harbor-jobservice
    docker.io/goharbor/harbor-portal
    docker.io/goharbor/harbor-registryctl
    docker.io/goharbor/nginx-photon
    docker.io/goharbor/notary-server-photon
    docker.io/goharbor/notary-signer-photon
    docker.io/goharbor/redis-photon
    docker.io/goharbor/registry-photon
    docker.io/goharbor/trivy-adapter-photon
    docker.io/golang
    docker.io/grafana/grafana
    docker.io/grafana/tempo
    docker.io/halverneus/static-file-server
    docker.io/haproxy
    docker.io/honkit/honkit
    docker.io/integratedcloudnative/ovn4nfv-k8s-plugin
    docker.io/istio/citadel
    docker.io/istio/examples-bookinfo-details-v1
    docker.io/istio/examples-bookinfo-productpage-v1
    docker.io/istio/examples-bookinfo-ratings-v1
    docker.io/istio/examples-bookinfo-reviews-v1
    docker.io/istio/examples-bookinfo-reviews-v2
    docker.io/istio/examples-bookinfo-reviews-v3
    docker.io/istio/examples-helloworld-v1
    docker.io/istio/examples-helloworld-v2
    docker.io/istio/galley
    docker.io/istio/install-cni
    docker.io/istio/kubectl
    docker.io/istio/mixer
    docker.io/istio/operator
    docker.io/istio/pilot
    docker.io/istio/proxyv2
    docker.io/istio/sidecar_injector
    docker.io/jaegertracing/all-in-one
    docker.io/jaegertracing/jaeger-agent
    docker.io/jaegertracing/jaeger-collector
    docker.io/jaegertracing/jaeger-es-index-cleaner
    docker.io/jaegertracing/jaeger-es-rollover
    docker.io/jaegertracing/jaeger-operator
    docker.io/jaegertracing/jaeger-query
    docker.io/jaegertracing/spark-dependencies
    docker.io/java
    docker.io/jboss/keycloak
    docker.io/jenkins/jnlp-slave
    docker.io/jimmidyson/configmap-reload
    docker.io/joosthofman/wget
    docker.io/joseluisq/static-web-server
    docker.io/jujusolutions/juju-db
    docker.io/jujusolutions/jujud-operator
    docker.io/k8scloudprovider/cinder-csi-plugin
    docker.io/karmada/karmada-agent
    docker.io/karmada/karmada-aggregated-apiserver
    docker.io/karmada/karmada-controller-manager
    docker.io/karmada/karmada-descheduler
    docker.io/karmada/karmada-scheduler
    docker.io/karmada/karmada-scheduler-estimator
    docker.io/karmada/karmada-search
    docker.io/karmada/karmada-webhook
    docker.io/kedacore/keda
    docker.io/kedacore/keda-metrics-apiserver
    docker.io/kennethreitz/httpbin
    docker.io/keyval/otel-go-agent
    docker.io/kindest/base
    docker.io/kindest/haproxy
    docker.io/kindest/node
    docker.io/kiwigrid/k8s-sidecar
    docker.io/kubeedge/cloudcore
    docker.io/kubeovn/kube-ovn
    docker.io/kuberhealthy/dns-resolution-check
    docker.io/kuberhealthy/kuberhealthy
    docker.io/kubernetesui/dashboard
    docker.io/kubernetesui/dashboard-amd64
    docker.io/kubernetesui/metrics-scraper
    docker.io/library/alpine
    docker.io/library/busybox
    docker.io/library/caddy
    docker.io/library/centos
    docker.io/library/debian
    docker.io/library/docker
    docker.io/library/golang
    docker.io/library/haproxy
    docker.io/library/java
    docker.io/library/mariadb
    docker.io/library/mysql
    docker.io/library/nats-streaming
    docker.io/library/nginx
    docker.io/library/node
    docker.io/library/openjdk
    docker.io/library/percona
    docker.io/library/perl
    docker.io/library/phpmyadmin
    docker.io/library/postgres
    docker.io/library/python
    docker.io/library/rabbitmq
    docker.io/library/redis
    docker.io/library/registry
    docker.io/library/traefik
    docker.io/library/ubuntu
    docker.io/library/wordpress
    docker.io/library/zookeeper
    docker.io/longhornio/backing-image-manager
    docker.io/longhornio/csi-attacher
    docker.io/longhornio/csi-node-driver-registrar
    docker.io/longhornio/csi-provisioner
    docker.io/longhornio/csi-resizer
    docker.io/longhornio/csi-snapshotter
    docker.io/longhornio/longhorn-engine
    docker.io/longhornio/longhorn-instance-manager
    docker.io/longhornio/longhorn-manager
    docker.io/longhornio/longhorn-share-manager
    docker.io/longhornio/longhorn-ui
    docker.io/mariadb
    docker.io/merbridge/merbridge
    docker.io/metallb/controller
    docker.io/metallb/speaker
    docker.io/minio/console
    docker.io/minio/kes
    docker.io/minio/logsearchapi
    docker.io/minio/mc
    docker.io/minio/minio
    docker.io/minio/operator
    docker.io/mirantis/k8s-netchecker-agent
    docker.io/mirantis/k8s-netchecker-server
    docker.io/mirrorgooglecontainers/defaultbackend-amd64
    docker.io/mirrorgooglecontainers/hpa-example
    docker.io/moby/buildkit
    docker.io/multiarch/qemu-user-static
    docker.io/mysql
    docker.io/n8nio/n8n
    docker.io/nacos/nacos-server
    docker.io/nats-streaming
    docker.io/neuvector/controller
    docker.io/neuvector/enforcer
    docker.io/neuvector/manager
    docker.io/neuvector/scanner
    docker.io/neuvector/updater
    docker.io/nfvpe/multus
    docker.io/nginx
    docker.io/nginxdemos/hello
    docker.io/node
    docker.io/oamdev/cluster-gateway
    docker.io/oamdev/kube-webhook-certgen
    docker.io/oamdev/terraform-controller
    docker.io/oamdev/vela-apiserver
    docker.io/oamdev/vela-core
    docker.io/oamdev/vela-rollout
    docker.io/oamdev/velaux
    docker.io/oliver006/redis_exporter
    docker.io/openebs/admission-server
    docker.io/openebs/linux-utils
    docker.io/openebs/m-apiserver
    docker.io/openebs/node-disk-manager
    docker.io/openebs/node-disk-operator
    docker.io/openebs/openebs-k8s-provisioner
    docker.io/openebs/provisioner-localpv
    docker.io/openebs/snapshot-controller
    docker.io/openebs/snapshot-provisioner
    docker.io/openjdk
    docker.io/openpolicyagent/gatekeeper
    docker.io/openstorage/stork
    docker.io/openzipkin/zipkin
    docker.io/osixia/openldap
    docker.io/otel/demo
    docker.io/otel/opentelemetry-collector
    docker.io/otel/opentelemetry-collector-contrib
    docker.io/percona
    docker.io/perl
    docker.io/phpmyadmin
    docker.io/phpmyadmin/phpmyadmin
    docker.io/portainer/portainer-ce
    docker.io/postgres
    docker.io/prom/alertmanager
    docker.io/prom/mysqld-exporter
    docker.io/prom/node-exporter
    docker.io/prom/prometheus
    docker.io/python
    docker.io/rabbitmq
    docker.io/rabbitmqoperator/cluster-operator
    docker.io/rancher/helm-controller
    docker.io/rancher/k3d-tools
    docker.io/rancher/k3s
    docker.io/rancher/kubectl
    docker.io/rancher/local-path-provisioner
    docker.io/redis
    docker.io/redislabs/redisearch
    docker.io/registry
    docker.io/sonobuoy/cluster-inventory
    docker.io/sonobuoy/kube-bench
    docker.io/sonobuoy/sonobuoy
    docker.io/sonobuoy/systemd-logs
    docker.io/squidfunk/mkdocs-material
    docker.io/swaggerapi/swagger-codegen-cli
    docker.io/tgagor/centos-stream
    docker.io/thanosio/thanos
    docker.io/traefik
    docker.io/ubuntu
    docker.io/velero/velero
    docker.io/victoriametrics/operator
    docker.io/victoriametrics/vmagent
    docker.io/victoriametrics/vmalert
    docker.io/victoriametrics/vminsert
    docker.io/victoriametrics/vmselect
    docker.io/victoriametrics/vmstorage
    docker.io/weaveworks/scope
    docker.io/weaveworks/weave-kube
    docker.io/weaveworks/weave-npc
    docker.io/wordpress
    docker.io/xueshanf/install-socat
    docker.io/zenko/kafka-manager
    docker.io/zookeeper
    gcr.io/cadvisor/cadvisor
    gcr.io/distroless/base
    gcr.io/distroless/static
    gcr.io/distroless/static-debian11
    gcr.io/google-containers/pause
    gcr.io/google.com/cloudsdktool/cloud-sdk
    gcr.io/google_containers/hyperkube
    gcr.io/heptio-images/ks-guestbook-demo
    gcr.io/istio-release/app_sidecar_base_centos_7
    gcr.io/istio-release/app_sidecar_base_centos_8
    gcr.io/istio-release/base
    gcr.io/istio-release/distroless
    gcr.io/istio-release/iptables
    gcr.io/istio-testing/app
    gcr.io/istio-testing/build-tools
    gcr.io/istio-testing/buildkit
    gcr.io/istio-testing/dotdotpwn
    gcr.io/istio-testing/ext-authz
    gcr.io/istio-testing/fake-gce-metadata
    gcr.io/istio-testing/fake-stackdriver
    gcr.io/istio-testing/fuzz_tomcat
    gcr.io/istio-testing/jwttool
    gcr.io/istio-testing/kind-node
    gcr.io/istio-testing/kindest/node
    gcr.io/istio-testing/mynewproxy
    gcr.io/istio-testing/myproxy
    gcr.io/istio-testing/operator
    gcr.io/istio-testing/pilot
    gcr.io/istio-testing/proxyv2
    gcr.io/k8s-staging-etcd/etcd
    gcr.io/k8s-staging-gateway-api/admission-server
    gcr.io/k8s-staging-kube-state-metrics/kube-state-metrics
    gcr.io/k8s-staging-nfd/node-feature-discovery
    gcr.io/k8s-staging-test-infra/krte
    gcr.io/kaniko-project/executor
    gcr.io/knative-releases/knative.dev/client/cmd/kn
    gcr.io/knative-releases/knative.dev/eventing/cmd/apiserver_receive_adapter
    gcr.io/knative-releases/knative.dev/eventing/cmd/controller
    gcr.io/knative-releases/knative.dev/eventing/cmd/in_memory/channel_controller
    gcr.io/knative-releases/knative.dev/eventing/cmd/in_memory/channel_dispatcher
    gcr.io/knative-releases/knative.dev/eventing/cmd/mtbroker/filter
    gcr.io/knative-releases/knative.dev/eventing/cmd/mtbroker/ingress
    gcr.io/knative-releases/knative.dev/eventing/cmd/mtchannel_broker
    gcr.io/knative-releases/knative.dev/eventing/cmd/mtping
    gcr.io/knative-releases/knative.dev/eventing/cmd/webhook
    gcr.io/knative-releases/knative.dev/net-istio/cmd/controller
    gcr.io/knative-releases/knative.dev/net-istio/cmd/webhook
    gcr.io/knative-releases/knative.dev/net-kourier/cmd/kourier
    gcr.io/knative-releases/knative.dev/serving/cmd/activator
    gcr.io/knative-releases/knative.dev/serving/cmd/autoscaler
    gcr.io/knative-releases/knative.dev/serving/cmd/controller
    gcr.io/knative-releases/knative.dev/serving/cmd/default-domain
    gcr.io/knative-releases/knative.dev/serving/cmd/domain-mapping
    gcr.io/knative-releases/knative.dev/serving/cmd/domain-mapping-webhook
    gcr.io/knative-releases/knative.dev/serving/cmd/queue
    gcr.io/knative-releases/knative.dev/serving/cmd/webhook
    gcr.io/kuar-demo/kuard-amd64
    gcr.io/kubebuilder/kube-rbac-proxy
    gcr.io/kubecost1/cost-model
    gcr.io/kubecost1/frontend
    gcr.io/tekton-releases/github.com/tektoncd/dashboard/cmd/dashboard
    gcr.io/tekton-releases/github.com/tektoncd/operator/cmd/kubernetes/operator
    gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/controller
    gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/entrypoint
    gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/git-init
    gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/imagedigestexporter
    gcr.io/tekton-releases/github.com/tektoncd/pipeline/cmd/webhook
    gcr.io/tekton-releases/github.com/tektoncd/results/cmd/api
    gcr.io/tekton-releases/github.com/tektoncd/results/cmd/watcher
    gcr.io/tekton-releases/github.com/tektoncd/triggers/cmd/controllers
    gcr.io/tekton-releases/github.com/tektoncd/triggers/cmd/webhook
    ghcr.io/aquasecurity/trivy
    ghcr.io/aquasecurity/trivy-db
    ghcr.io/clusterpedia-io/clusterpedia/apiserver
    ghcr.io/clusterpedia-io/clusterpedia/clustersynchro-manager
    ghcr.io/daocloud/ckube
    ghcr.io/daocloud/dao-2048
    ghcr.io/dependabot/dependabot-core
    ghcr.io/dependabot/dependabot-core-development
    ghcr.io/dexidp/dex
    ghcr.io/dtzar/helm-kubectl
    ghcr.io/ferryproxy/ferry/ferry-controller
    ghcr.io/ferryproxy/ferry/ferry-tunnel
    ghcr.io/fluxcd/helm-controller
    ghcr.io/fluxcd/kustomize-controller
    ghcr.io/fluxcd/notification-controller
    ghcr.io/fluxcd/source-controller
    ghcr.io/helm/chartmuseum
    ghcr.io/hwameistor/admission
    ghcr.io/hwameistor/apiserver
    ghcr.io/hwameistor/drbd-reactor
    ghcr.io/hwameistor/drbd9-bionic
    ghcr.io/hwameistor/drbd9-focal
    ghcr.io/hwameistor/drbd9-jammy
    ghcr.io/hwameistor/drbd9-rhel7
    ghcr.io/hwameistor/drbd9-rhel8
    ghcr.io/hwameistor/drbd9-shipper
    ghcr.io/hwameistor/evictor
    ghcr.io/hwameistor/local-disk-manager
    ghcr.io/hwameistor/local-storage
    ghcr.io/hwameistor/scheduler
    ghcr.io/hwameistor/self-signed
    ghcr.io/jaredtan95/openinsight
    ghcr.io/jaredtan95/tailing-sidecar
    ghcr.io/jaredtan95/tailing-sidecar-operator
    ghcr.io/k8snetworkplumbingwg/multus-cni
    ghcr.io/k8snetworkplumbingwg/sriov-cni
    ghcr.io/k8snetworkplumbingwg/sriov-network-device-plugin
    ghcr.io/klts-io/kubernetes-lts/coredns
    ghcr.io/klts-io/kubernetes-lts/etcd
    ghcr.io/klts-io/kubernetes-lts/kube-apiserver
    ghcr.io/klts-io/kubernetes-lts/kube-controller-manager
    ghcr.io/klts-io/kubernetes-lts/kube-proxy
    ghcr.io/klts-io/kubernetes-lts/kube-scheduler
    ghcr.io/klts-io/kubernetes-lts/pause
    ghcr.io/kube-vip/kube-vip
    ghcr.io/kubean-io/kubean-operator
    ghcr.io/kubean-io/kubespray
    ghcr.io/kubean-io/spray-job
    ghcr.io/open-telemetry/demo
    ghcr.io/open-telemetry/opentelemetry-operator/autoinstrumentation-dotnet
    ghcr.io/open-telemetry/opentelemetry-operator/autoinstrumentation-java
    ghcr.io/open-telemetry/opentelemetry-operator/autoinstrumentation-nodejs
    ghcr.io/open-telemetry/opentelemetry-operator/autoinstrumentation-python
    ghcr.io/open-telemetry/opentelemetry-operator/opentelemetry-operator
    ghcr.io/openfaas/basic-auth
    ghcr.io/openfaas/faas-netes
    ghcr.io/openfaas/gateway
    ghcr.io/openfaas/queue-worker
    ghcr.io/openinsight-proj/openinsight
    ghcr.io/openinsight-proj/opentelemetry-demo-helm-chart/adservice
    ghcr.io/openinsight-proj/opentelemetry-demo-helm-chart/sentinel
    ghcr.io/projectcontour/contour
    ghcr.io/pterodactyl/yolks
    ghcr.io/scholzj/zoo-entrance
    ghcr.io/spidernet-io/cni-plugins/meta-plugins
    ghcr.io/spidernet-io/spiderdoctor-agent
    ghcr.io/spidernet-io/spiderdoctor-controller
    ghcr.io/spidernet-io/spiderpool/spiderpool-agent
    ghcr.io/spidernet-io/spiderpool/spiderpool-base
    ghcr.io/spidernet-io/spiderpool/spiderpool-controller
    ghcr.io/sumologic/tailing-sidecar
    ghcr.io/sumologic/tailing-sidecar-operator
    quay.io/argoproj/argo-events
    quay.io/argoproj/argo-rollouts
    quay.io/argoproj/argocd
    quay.io/argoproj/argocd-applicationset
    quay.io/argoproj/argocli
    quay.io/argoproj/argoexec
    quay.io/argoproj/kubectl-argo-rollouts
    quay.io/argoproj/workflow-controller
    quay.io/argoprojlabs/argocd-image-updater
    quay.io/brancz/kube-rbac-proxy
    quay.io/calico/apiserver
    quay.io/calico/cni
    quay.io/calico/ctl
    quay.io/calico/kube-controllers
    quay.io/calico/node
    quay.io/calico/pod2daemon-flexvol
    quay.io/calico/typha
    quay.io/cilium/certgen
    quay.io/cilium/cilium
    quay.io/cilium/cilium-etcd-operator
    quay.io/cilium/cilium-init
    quay.io/cilium/clustermesh-apiserver
    quay.io/cilium/hubble-relay
    quay.io/cilium/hubble-ui
    quay.io/cilium/hubble-ui-backend
    quay.io/cilium/json-mock
    quay.io/cilium/operator
    quay.io/cilium/operator-generic
    quay.io/cilium/startup-script
    quay.io/containers/skopeo
    quay.io/coreos/etcd
    quay.io/coreos/flannel
    quay.io/datawire/ambassador-operator
    quay.io/external_storage/cephfs-provisioner
    quay.io/external_storage/local-volume-provisioner
    quay.io/external_storage/nfs-client-provisioner
    quay.io/external_storage/rbd-provisioner
    quay.io/fluentd_elasticsearch/elasticsearch
    quay.io/fluentd_elasticsearch/fluentd
    quay.io/goswagger/swagger
    quay.io/grafana-operator/grafana_plugins_init
    quay.io/iovisor/bcc
    quay.io/jaegertracing/jaeger-operator
    quay.io/jetstack/cert-manager-cainjector
    quay.io/jetstack/cert-manager-controller
    quay.io/jetstack/cert-manager-ctl
    quay.io/jetstack/cert-manager-webhook
    quay.io/k8scsi/csi-attacher
    quay.io/k8scsi/csi-node-driver-registrar
    quay.io/k8scsi/csi-provisioner
    quay.io/k8scsi/csi-resizer
    quay.io/k8scsi/csi-snapshotter
    quay.io/k8scsi/livenessprobe
    quay.io/k8scsi/snapshot-controller
    quay.io/keycloak/keycloak
    quay.io/kiali/kiali
    quay.io/kiwigrid/k8s-sidecar
    quay.io/kubespray/kubespray
    quay.io/l23network/k8s-netchecker-agent
    quay.io/l23network/k8s-netchecker-server
    quay.io/metallb/controller
    quay.io/metallb/speaker
    quay.io/minio/minio
    quay.io/mongodb/mongodb-agent
    quay.io/mongodb/mongodb-kubernetes-operator
    quay.io/mongodb/mongodb-kubernetes-operator-version-upgrade-post-start-hook
    quay.io/mongodb/mongodb-kubernetes-readinessprobe
    quay.io/nmstate/kubernetes-nmstate-handler
    quay.io/nmstate/kubernetes-nmstate-operator
    quay.io/opstree/redis
    quay.io/opstree/redis-exporter
    quay.io/opstree/redis-operator
    quay.io/piraeusdatastore/drbd-reactor
    quay.io/piraeusdatastore/drbd9-centos7
    quay.io/piraeusdatastore/piraeus-client
    quay.io/piraeusdatastore/piraeus-csi
    quay.io/piraeusdatastore/piraeus-ha-controller
    quay.io/piraeusdatastore/piraeus-operator
    quay.io/prometheus-operator/prometheus-config-reloader
    quay.io/prometheus-operator/prometheus-operator
    quay.io/prometheus/alertmanager
    quay.io/prometheus/blackbox-exporter
    quay.io/prometheus/node-exporter
    quay.io/prometheus/prometheus
    quay.io/prometheuscommunity/elasticsearch-exporter
    quay.io/spotahome/redis-operator
    quay.io/strimzi/jmxtrans
    quay.io/strimzi/kafka
    quay.io/strimzi/kafka-bridge
    quay.io/strimzi/kaniko-executor
    quay.io/strimzi/maven-builder
    quay.io/strimzi/operator             
    quay.io/submariner/submariner
    quay.io/submariner/submariner-gateway
    quay.io/submariner/submariner-globalnet
    quay.io/submariner/submariner-networkplugin-syncer
    quay.io/submariner/submariner-operator
    quay.io/submariner/submariner-operator-index
    quay.io/submariner/submariner-route-agent
    quay.io/tigera/operator
    registry.k8s.io/addon-resizer
    registry.k8s.io/build-image/debian-iptables
    registry.k8s.io/build-image/go-runner
    registry.k8s.io/build-image/kube-cross
    registry.k8s.io/cluster-api/cluster-api-controller
    registry.k8s.io/cluster-api/kubeadm-bootstrap-controller
    registry.k8s.io/cluster-api/kubeadm-control-plane-controller
    registry.k8s.io/conformance
    registry.k8s.io/coredns
    registry.k8s.io/coredns/coredns
    registry.k8s.io/cpa/cluster-proportional-autoscaler
    registry.k8s.io/cpa/cluster-proportional-autoscaler-amd64
    registry.k8s.io/cpa/cluster-proportional-autoscaler-arm64
    registry.k8s.io/debian-base
    registry.k8s.io/dns/k8s-dns-node-cache
    registry.k8s.io/etcd
    registry.k8s.io/etcd/etcd
    registry.k8s.io/ingress-nginx/controller
    registry.k8s.io/ingress-nginx/e2e-test-runner
    registry.k8s.io/ingress-nginx/kube-webhook-certgen
    registry.k8s.io/kube-apiserver
    registry.k8s.io/kube-apiserver-amd64
    registry.k8s.io/kube-controller-manager
    registry.k8s.io/kube-controller-manager-amd64
    registry.k8s.io/kube-proxy
    registry.k8s.io/kube-proxy-amd64
    registry.k8s.io/kube-registry-proxy
    registry.k8s.io/kube-scheduler
    registry.k8s.io/kube-scheduler-amd64
    registry.k8s.io/kube-state-metrics/kube-state-metrics
    registry.k8s.io/kueue/kueue
    registry.k8s.io/kwok/kwok
    registry.k8s.io/metrics-server
    registry.k8s.io/metrics-server-amd64
    registry.k8s.io/metrics-server/metrics-server
    registry.k8s.io/metrics-server/metrics-server-amd64
    registry.k8s.io/nfd/node-feature-discovery
    registry.k8s.io/node-problem-detector/node-problem-detector
    registry.k8s.io/node-test
    registry.k8s.io/node-test-amd64
    registry.k8s.io/pause
    registry.k8s.io/prometheus-adapter/prometheus-adapter
    registry.k8s.io/sig-storage/csi-attacher
    registry.k8s.io/sig-storage/csi-node-driver-registrar
    registry.k8s.io/sig-storage/csi-provisioner
    registry.k8s.io/sig-storage/csi-resizer
    registry.k8s.io/sig-storage/csi-snapshotter
    registry.k8s.io/sig-storage/livenessprobe
    registry.k8s.io/sig-storage/local-volume-provisioner
    registry.k8s.io/sig-storage/nfs-subdir-external-provisioner
    registry.k8s.io/sig-storage/snapshot-controller
    registry.opensource.zalan.do/acid/logical-backup
    registry.opensource.zalan.do/acid/pgbouncer
    registry.opensource.zalan.do/acid/postgres-operator
    registry.opensource.zalan.do/acid/spilo-14
    ```

[Mirror repo on GitHub](https://github.com/DaoCloud/public-image-mirror){ .md-button }