---
hide:
  - toc
---

# DaoCloud Enterprise 5.0

DaoCloud Enterprise 5.0 is a high-performance, scalable cloud-native operating system. It can provide a consistent and stable experience in any infrastructure and environment, supporting heterogeneous clouds, edge clouds, and multi-cloud orchestration. DCE 5.0 integrates the latest service mesh and microservice technologies, which can track the entire lifecycle of each traffic, help you understand the detailed metrics of clusters, nodes, applications, and services, and visualize the health status of applications through dynamic dashboards and topology maps.

DCE 5.0 natively supports the DevOps development and operation mode, which can realize the standardization and automation of the entire application delivery process, and integrates various selected databases and middleware to make operation and maintenance governance more efficient. Each product module is independently decoupled, supports flexible upgrades, has no impact on business, and can be docked with many cloud-native ecological products to provide a complete solution system. It has been tested in production scenarios by nearly a thousand industry customers, building a solid and reliable digital foundation, helping enterprises define digital boundaries, and unleashing cloud-native productivity.

<div class="grid cards" markdown>

- :fontawesome-solid-jet-fighter-up: **Installation** [Install Community and Commercial releases](../install/intro.md)
- :octicons-container-16: **Container Management** [Manage multi-cluster containers and pods](../kpanda/intro/WhatisKPanda.md)
- :fontawesome-solid-user-group: **Global Management** [Login, user and access, appearance](../ghippo/intro/what.md)
- :material-monitor-dashboard: **Observability** [One-stop graphical dashboard](../insight/intro/WhatisInsight.md)
- :material-microsoft-azure-devops: **Workbench** [CI/CD pipeline](../amamba/intro/WhatisAmamba.md)
- :material-cloud-check: **Multicloud Orchestration** [Manage multi-cloud instances, workloads, policies](kairship/01product/whatiskairship.md)
- :material-engine: **Microservice Engine** [Microservice registry and gateway](../skoala/intro/features.md)
- :material-table-refresh: **Service Mesh** [Non-intrusive service governance](../mspider/intro/WhatismSpider.md)
- :material-middleware: **Middleware** [ES, Kafka, MinIO, MySQL, etc.](../middleware/midware.md)
- :material-warehouse: **Container Registry** [Integrate and manage registries](../kangaroo/intro.md)
- :material-dot-net: **Network** [Multi-CNI fusion solution](../network/intro/what-is-net.md)
- :floppy_disk: **Storage** [Comprehensive solution for containerized storage](../storage/intro/what.md)

</div>

![modules](../images/dce-modules04.jpg)

In the past eight years, DaoCloud has invested huge to explore and develop a cloud-native operating system with custom and scalable modules to facilitate your business digitalization. You can use each module like a LEGO brick, with zero downtime while upgrading any module. DCE 5.0 is also easy to integrate with hundreds of cloud-native ecological plugins, so you can simply customize solutions for different scenarios. Things go better with such a kind of modular style to grow day by day.

=== "Multicloud Orchestration"

    **Applicable scenarios**: The deployment of multicloud and multi-cluster in an enterprise has become the norm, and it is hoped to have the capabilities of multicloud app release and cross-cloud disaster recovery.

    **Benefits**: Using innovative technologies to orchestrate disaster recovery (DR) across clouds, this solution has high concurrent performance of cross-cloud resource retrieval, and can help your IT departments quickly plan and implement DR capabilities in combination with the capabilities of the Container Management to adapt to various scenarios such as edge and Xinchuang.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdcloud Orchestration](../kairsh../kairship/intro/whatiskairship.mdrk](../network/intro/what-is-net.md), Storage, cloud to edge continuum, Xinchuang Heterogeneous

    ![multi-cloud](../images/01multi-cloud.jpg)

=== "Middleware Service"

    **Applicable scenarios**: An enterprise has an app architecture that relies on mainstream middleware capabilities. It is hoped to run and maintain middleware in a unified manner and get more professional support capabilities for middleware planning, operation, and maintenance (O&M).

    **Benefits**: This solution has selected middlewares with a consistent UI to manage, with the help of HwameiStor capabilities designed for stateful applications, providing features of multi-tenant, deployment, observation, backup, operation and maintenance of the whole lifecycle of middleware management capabilities.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdrk](../network/intro/what-is-net.md), Storage, [Middleware](../middleware/midware.md)

    ![data](../images/02data.png)

=== "Microservice Governance"

    **Applicable scenarios**

    An enterprise decides to adopt a microservice architecture or has already adopted microservices, hopes to obtain a full range of technical support and O&M capabilities such as a microservice framework, or hopes to use service mesh technologies, and tries to achieve smoothness in the process of digital transformation.

    - The enterprise doesn't want to change anything, but just wants to view various service states via a panoramic view, and hopes to easily troubleshoot faults with traces and logs.
    - The enterprise has the idea of tranforming from the traditional microservice framework to service mesh, but it is more conservative. It is hoped that there will be a transition period for the gradual transformation. At this time, it is more suitable to use a service mesh solution.
    - The enterprise hopes to directly tranform to service mesh. In this case, it is a good idea to remove Eureka-related components and directly use the microservice engine and service mesh.
    - The enterprise does not want to tranform from traditional microservices to mesh, but wants to do east-west traffic management.

    **Benefits**

    Seamless integrate with legacy and popular microservice technologies, such as the first-generation microservices represented by SpringCloud and Dubbo and the new generation of microservices represented by Istio service mesh, with the lifecycle management capabilities of development, deployment, joining, exposing to external, observation, and O&M. Seamlessly add the existing microservice system of the enterprise, provide the complete capabilities of managed microservice governance, and offer the high-performance cloud-native microservice gateway.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdservice Engine](../skoala/intro/features.md), [Service Mesh](../mspider/01Intro../mspider/intro/WhatismSpider.mdsight/intro/WhatisInsight.md), [App Workbench](../amamba/intro/WhatisAmamba.md), [Network](../network/intro/what-is-net.md), Storage

    ![微服务](../images/03msgov.png)

=== "Insight"

    **Applicable scenarios**: An enterprise has a weak capability to watch running applications, and hopes to complete the Insight through a lightweight or unmodified method, to get a panaramic view for current apps with logs, metrics, traces.

    **Benefits**: This solution provides in-depth and subtle observation of the current app status. With a comprehensive dashboard, you can query all cluster and workload data. It supports for microservice architecture, service mesh, eBPF-based network, and other observation capabilities.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdht](../insight/intro/WhatisInsight.md), [Network](../network/intro/what-is-net.md), Storage

    ![观测](../images/04insight.png)

=== "App Store"

    **Applicable scenarios**: An enterprise wants to obtain out-of-the-box cloud native apps capabilities for some exclusive scenarios

    **Benefits**: This solution provides the ecological capabilities including software products from partners,  with a complete software stack to meet the actual business needs. Where, you can easily find, test, and deploy middlewares running on DaoCloud Enterprise 5.0 with a development process of low-code or no-code.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdrk](../network/intro/what-is-net.md), Storage, App Store, Product Ecosystem

=== "App Delivery"

    **Applicable scenarios**: An enterprise adopts cloud-native technology on a large scale, and expects to promote cloud-native technology to a wider range by combining with DevOps concepts.

    **Benefits**: With a consistent workflow to deliver apps, this solution supports a hierarchical multi-tenant system, seamlessly adapts to the user's organizational structure to plan resource allocation, automates app build and deployment with the CI/CD pipelines, and innovatively introduces the GitOps progressive delivery capability.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mdorkbench](../amamba/intro/WhatisAmamba.md), [Registry](../kangaroo/intro.md), [Network](../network/intro/what-is-net.md), Storage

    ![应用交付](../images/06appdeliv.png)

=== "Cloud Native Base"

    **Applicable scenarios**: The O&M team of an enterprise needs to undertake tasks to maintain thousands of clusters, and the cluster network needs to meet the traditional network supervision requirements.

    **Benefits**: 

    Breaking through the performance bottleneck of Kubernetes API, this solution supports for ultra-large scale clusters concurrently, and provides full life-cycle management capabilities from deployment, rolling update, certificate management, configuration settings, and garbage collection.

    - MacVLAN solution
    - SR-IOV smart network acceleration solution
    - SpiderPool IPAM solution
    - Clilum eBPF-based network solution
    - Underlay and Overlay network continuum

    All clusters and workloads are managed through Clusterpedia. This solution is compatible with joining standard Kubernetes clusters, breaking through the performance bottleneck of Kubernetes API and supporting thousands of users using it at the same time.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mder lifecycle manager](../community/kubean.md), [Network](../network/intro/what-is-net.md), Storage,

=== "Heterogeneous architecture"

    **Applicable scenarios**: An enterprise needs to set up heterogeneous infrastructure. For example, the CPU processor must be from one of Loongson, Hygon, Phytium, Kunpeng, Intel; and the operating system must be KirinOS, UOS, OpenEuler, etc.

    **Benefits**: This solution can consolidate heterogeneous cloud-native capabilities for government sectors and state-owned factories, supports domestic chips and servers in the north, and supports heterogeneous operating system and app ecosystem in containers in the south.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mder lifecycle manager](../community/kubean.md), [Middware](../middleware/midware.md), [Network](../network/intro/what-is-net.md), Storage

    ![信创](../images/08xinchuan.png)

=== "Cloud to edge continuum"

    **Applicable scenarios**: An enterprise designs an edge collaboration solution on the basis of cloud, edge, and terminal. The edge is a general computing platform and has strict computing requirements. The edge supports several deployment modes: edge node, edge cluster, data center computing downwards, edge device computing upwards.

    **Benefits**: This solution extends the general cloud-native framework, empowers the edge computing capability, uniformly manages and controls all edge clusters and nodes. Based on the traditional three-tier model of cloud, edge, and terminal. To meet the strict edge computing requirements, this solution provides a four-tier model from cloud to edge continuum by adding the edge clusters and nodes.

    **Modules**: [Global Management](../ghippo/intro/what.md), [Container Management](../kpanda../kpanda/intro/WhatisKPanda.mder lifecycle manager](../community/kubean.md), [Network](../network/intro/what-is-net.md), Storage, Edge nodes, clusters in a weak network

    ![Cloud to edge continuum](../images/09cloud-edge.png)

Just like Lego bricks, it combines dozens of the best open source technologies into a platform. After many dialectical selection, adaptation and running-in, coding debugging, and massive testing, a sword is sharpened in ten years. The new generation of containerized platforms can meet the needs of various scenarios for enterprises migrating to the cloud.

[Download DCE 5.0](../download/dce5.md){ .md-button .md-button--primary }
[Install DCE 5.0](../install/intro.md){ .md-button .md-button--primary }
[Free Trial](license0.md){ .md-button .md-button--primary }