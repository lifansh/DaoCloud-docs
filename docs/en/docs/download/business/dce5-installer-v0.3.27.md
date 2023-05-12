# DCE 5.0 Commercial Release v0.3.27

This page can download the offline installation package and verification file of DCE 5.0 Commercial release.

## Download

| File name | Package |
| ------------------- | ----------------------------- -------------------------------------------------- --------------------- |
| offline-v0.3.27.tar | [:arrow_down: Download](https://proxy-qiniu-download-public.daocloud.io/DaoCloud_Enterprise/dce5/offline-v0.3.27.tar) |

## Validation

Go to the download directory of the offline installation package. Run the following command to verify the installation package:

```sh
echo "f637ec103af6e77d1af85bf0708bef71aee123ce4ac71c4a0adef539492cdbb1661a479d3e999cd51aa7cb47d49e001565908b237ef7999140e3435f6219bb08 offline -v0.3.27.tar" | sha512sum -c
```

If the validation is successful, it will print:

```none
offline-v0.3.27.tar: OK
```

## Install

After successfully verifying the offline package, please refer to [Commercial release installation process](../../install/commercial/start-install.md) to install.

After successful installation, please contact us for authorization: email info@daocloud.io or call 400 002 6898.

## Modules

The DCE 5.0 Commercial Release includes the following modules, which are plug-and-play on-demand to meet various application scenarios:

| Modules | Introduction | What's New |
| ---------- | -------------------------------------- ---------------------------------- | --------------- ---------------------------------------------- |
| Global Management | Responsible for user access control, permissions, enterprise space, audit logs, personalized appearance settings, etc. | [Release Notes](../../release/rn5.0.md#_4) |
| Container Management | Manage K8s core functions such as clusters, nodes, workloads, Helm applications, CRDs, and namespaces | [v0.12.0](../../kpanda/intro/release-notes.md#v0120) |
| Observability | Provide rich graphic information such as dashboards, scene monitoring, data query, and alarms | [v0.11.1](../../insight/intro/releasenote.md#v0111) |
| App Workbench | A container-based DevOps application platform that supports pipeline operations such as Jenkins, Tekton, GitOps, etc. | [Release Notes](../../amamba/intro/release-notes.md) |
| Multi-cloud orchestration | Centralized management of application orchestration of multi-cloud, hybrid cloud, and cross-cloud resources, with multi-cloud disaster recovery and fault recovery capabilities | [v0.3.0](../../kairship/intro/release-notes.md) |
| Microservice Engine | Provides governance capabilities such as registration discovery, service governance, configuration management, and microservice gateway | [Release Notes](../../release/rn5.0.md) |
| Service Mesh | A next-generation service mesh for cloud-native applications based on Istio open source technology | [v0.10.0](../../mspider/intro/release-notes.md) |
| Middleware | Contains selected middleware such as RabbitMQ, Kafka, Elasticsearch, MySQL, Redis, MinIO, etc. | [Release Notes](../../release/rn5.0.md) |
| Image Registry | Images for storing K8s, DevOps, and container application development | [Release Notes](../../release/rn5.0.md) |
| Network | Support multiple CNI combinations for different Linux kernels | [Release Notes](../../release/rn5.0.md) |
| Storage | Provide unified data storage services, support files, objects, blocks, and local storage, and easily access storage vendor solutions | [Release Notes](../../release/rn5.0.md) |

## More

- [Online Documentation](../../dce/what.md)
- [Report a bug](https://github.com/DaoCloud/DaoCloud-docs/issues)