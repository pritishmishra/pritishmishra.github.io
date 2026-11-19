---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

<div class="collapsible-controls">
  <button type="button" class="btn btn--small" data-collapsible-action="expand">Expand all</button>
  <button type="button" class="btn btn--small" data-collapsible-action="collapse">Collapse all</button>
</div>

<details class="collapsible collapsible--section" id="university-of-toronto" open markdown="1">
<summary><h1>University of Toronto</h1><span class="collapsible-meta"><strong>Research Assistant, PhD Student</strong> | 09/2020 – Present</span></summary>

<details class="collapsible collapsible--item" id="adaptive-stateful-stream-processing-for-edgecloud-infrastructure" open markdown="1">
<summary><h2>Adaptive Stateful Stream Processing for Edge–Cloud Infrastructure</h2></summary>

- Duration: 2021 – 2026
- Collaboration with researchers from McGill University, Nokia Bell Labs, Huawei Technology, and Konica Minolta.
- About: Stream processing is a real-time processing paradigm in which independent functions, called operators, form a directed acyclic graph (DAG). Stateful operators can run ML functions and retain model state across incoming events.
- Major contributions:
    - Conducted PhD thesis research on deploying and managing these operators across geo-distributed infrastructure, designing mechanisms for adaptive placement, scalable routing, live state migration, and privacy-aware execution.
    - This work resulted in six peer-reviewed publications in top-tier conferences; Falcon received the Best Paper Award at the ACM/IEEE Symposium on Edge Computing 2024, and StreamBucket received the Honourable Mention Award at IEEE CloudNet 2024.
    - Designed and implemented Cassandra-based geo-distributed state storage with gRPC communication, replicating data on demand only at sites that use it and selectively propagating reads and writes to limit cross-site traffic.
    - Implemented distributed checkpointing to reduce snapshot time and recover operator state after failures, excluding network partitions and availability-zone outages.
    - Implemented a geo-distributed router network of message brokers and network bridges using Apache ActiveMQ Artemis, providing exactly-once delivery and in-order tuple processing.
    - Extended the router framework with tuple batching and key bucketing to scale high-throughput applications.
    - Designed and implemented a live state-migration protocol using synchronization markers, dual routing, and controlled output emission. Allowed concurrent reads and writes during migration while preserving exactly-once and in-order processing.
    - Proposed late-binding routing to decouple logical operators from physical deployment locations and select processing destinations at runtime, adapting to changing deployments and data-source locations.
    - Designed locality-aware key buckets using data origins and processing dependencies to guide placement; combined per-bucket statistics with bounded tracking of frequently accessed keys to scale monitoring and placement.
    - Implemented cost-aware joint placement of aggregation and processing operators, tracking dependencies and reconfiguring only when expected savings justified migration.
- Key achievements: Our system keeps reconfiguration-induced application end-to-end tail latency spikes below 40 ms, achieves up to 10.2× lower operational cost and approximately 47× faster placement, and reduces deployment cost by 68.8% and total cost including reconfiguration by 44.5% relative to evaluated baselines.

</details>

<details class="collapsible collapsible--item" id="gpu-accelerated-vector-search-with-numerical-range-filters" open markdown="1">
<summary><h2>GPU-Accelerated Vector Search with Numerical Range Filters</h2></summary>

- Duration: 2025 – Present
- Collaboration with researchers from Indian universities IIIT, MUJ, OUTR, and DTU.
- Major contributions:
    - Designed an attribute-partitioned GPU index with contiguous storage, batched CAGRA search, exact range-filter verification, and cross-partition top-k merging to restrict data access to relevant regions.
    - Developed a modular benchmark with 15 workloads covering concurrent updates, distribution shifts, bursts, filters, and cold starts. Implemented an exact-search oracle that tracks live inserts and deletes to measure retrieval quality against the changing corpus.
    - Measured graph construction separately at 10.2–17.3 s and memory use at approximately 664 MB; persistent graph reuse across batches remains a deployment extension.
    - Benchmarked Milvus, Qdrant, Weaviate, Vespa, and PipeANN, measuring query/write latency, throughput, and recall. Identified 13.8–34.4% relative recall degradation for outlier queries and 1.8–30.5 percentage-point recall loss under concurrent mutations in three-million-vector pilots.
- Key achievements: Achieved Recall@10 of 0.992–0.999 with 2.53–5.58 ms search-stage latency on million-vector datasets with four filtered attributes; search timings exclude on-demand graph construction.

</details>

<details class="collapsible collapsible--item" id="retrieval-augmented-deduplication-of-online-training-datasets" open markdown="1">
<summary><h2>Retrieval Augmented Deduplication of Online Training Datasets</h2></summary>

- Duration: 2024 – 2026
- Collaboration with researchers from McGill University and IBM Research.
- Major contributions:
    - Developed online fuzzy deduplication for evolving ML training datasets. Combined compact MinHash document signatures, FAISS HNSW similarity search, and SIMD-accelerated comparisons to identify likely duplicates without scanning the full corpus; developed a bitmap representation with tie-breaking to improve retrieval.
    - Built an incremental ingestion pipeline that filters duplicates before admission, seals index partitions at one million documents, and merges candidates incrementally to bound result-buffer memory.
- Key achievements: Evaluation on 30+ million-document datasets showed 1.34–3.70× higher throughput than Milvus, a state-of-the-art vector database, with up to 97% recall.

</details>

<details class="collapsible collapsible--item" id="token-and-kv-cache-reuse-for-rag-pipeline-optimization" open markdown="1">
<summary><h2>Token and KV-Cache Reuse for RAG Pipeline Optimization</h2></summary>

- Duration: 2026 – Present
- Collaboration with researchers from McGill University and Nutanix.
- Major contributions:
    - Built a prototype caching tokenized document chunks by stable chunk ID. Designed retrieval to pass IDs from the vector index, fetch text from object storage on cache misses, and reuse token IDs across requests.
    - Designed cache-aware chunk ordering and separate directories for shared evidence prefixes and private conversation histories, enabling reuse of evidence-only prompt prefixes without sharing user-specific dialogue.
    - Investigating integration with vLLM and LMCache for exact-prefix KV-cache reuse. Lower CPU cost per request and faster time to first token remain evaluation targets; measured serving gains are not yet established.

</details>

</details>

<details class="collapsible collapsible--section" id="sap-labs" open markdown="1">
<summary><h1>SAP Labs</h1><span class="collapsible-meta"><strong>Senior Developer</strong> | 08/2016 – 08/2020</span></summary>

<details class="collapsible collapsible--item" id="mobile-development-kit-mdk" open markdown="1">
<summary><h2>Mobile Development Kit (MDK)</h2></summary>

- Team: SAP Mobile Services
- Project Duration: ~ 1 year
- Role: Senior Developer
- Modules Used: iOS SDK, Android SDK, NativeScript.
- Languages Used: TypeScript, Java, Swift/Objective C.
- About: MDK is an SDK library that can be used to easily design cross-platform mobile applications.
- Major contributions:
    - Developed features like: Charts and other Analytics, Just-in-time loading feature for List-pickers, Avatar image support, Offline Data, etc. for the library in iOS and Android.
    - Acted as Security Lead for all applications deployed for Mobile (iOS/Android)
    - Performed penetration testing, threat modelling, i/o operations for application security

</details>

<details class="collapsible collapsible--item" id="service-fabrik-broker" open markdown="1">
<summary><h2>Service-Fabrik Broker</h2></summary>

- Team: SAP Cloud Platform
- Project duration: ~ 3 years
- Role: Developer
- Github: [https://github.com/cloudfoundryincubator/service-fabrik-broker](https://github.com/cloudfoundryincubator/service-fabrik-broker)
- Modules Used: CloudFoundry, Docker, Kubernetes, Grafana, Riemann, InfluxDb, Bosh.
- Languages Used: Go, NodeJs, Python, Closure, Bash.
- Supported IaaS: AWS, OpenStack, Microsoft Azure, Google Cloud Platform, Alibaba Cloud. 
- About: Service-Fabrik Broker is an open-source Cloudfoundry-incubated project. It is a web-server used to create and manage database service instances on a PaaS platform.
- Major contributions:
    - Designed and Developed Multi-AZ HA and ZDM functionality for the cluster-based service-fabrik broker deployment for mulitple IaaSes like AWS, GCP, Azure and Openstack.
    - Designed and developed a turbulence framework to ensure the resilience of all Service-Fabrik components against potential disasters like Network Failure, Disk Failure, AZ Failure, etc.
    - Implemented Monitoring & Alerting for Bosh/Docker based instances for all services provisioned via SAP Cloud Platform.

</details>

<details class="collapsible collapsible--item" id="service-fabrik-backup--restore-library" open markdown="1">
<summary><h2>Service-Fabrik Backup &amp; Restore Library</h2></summary>

- Team: SAP Cloud Platform
- Project duration: ~ 3 years
- Role: Developer
- Github: [https://github.com/cloudfoundry-incubator/service-fabrik-backup-restore](https://github.com/cloudfoundry-incubator/service-fabrik-backup-restore)
- Modules Used: CloudFoundry, Docker, Kubernetes.
- Languages Used: Python.
- Supported DBs: PostgreSQL, MongoDb, Redis.
- Supported IaaS: AWS, OpenStack, Microsoft Azure, Google Cloud Platform, Alibaba Cloud.
- About: This library creates an on-demand or scheduled backup of the service instances. These backups can further be used to recover the state of an instance, especially during any failures.
-  Major contributions:
    - Implemented Point-in-time Recovery Feature for Service-Fabrik Backup Restore Library and facilitated the support for other backing services like PostgreSQL, MongoDb and Redis. 
    - Designed a framework to reduce the Restore Turnaround Duration for backing services in-order to comply to better RTO SLAs.

</details>

<details class="collapsible collapsible--item" id="cloudfoundry-cli-plugin" open markdown="1">
<summary><h2>CloudFoundry CLI Plugin</h2></summary>

- Team: SAP Cloud Platform
- Project Duration: 8 months
- Modules Used: CloudFoundry, Docker, Kubernetes.
- Languages Used: Go.
- Github: [https://github.com/cloudfoundry-incubator/service-fabrik-cli-plugin](https://github.com/cloudfoundry-incubator/service-fabrik-cli-plugin)
- Designed and developed CloudFoundry-based CLI plugin to create/manage backup and restore for backing services like Postgresql, Redis and MongoDb. The project is now Cloudfoundry-incubated.

</details>

</details>

<details class="collapsible collapsible--section" id="independent-research" open markdown="1">
<summary><h1>Independent Research</h1><span class="collapsible-meta"><strong>Freelance research conducted alongside my role at SAP Labs</strong> | 2018 – 2020</span></summary>

<details class="collapsible collapsible--item" id="software-defined-networking-and-edge-resource-management" open markdown="1">
<summary><h2>Software-Defined Networking and Edge Resource Management</h2></summary>

- Duration: 2018 – 2020
- This work resulted in six publications in top-tier conferences and journals.
- Major contributions:
    - Designed a hierarchical SD-WAN control plane separating LAN and WAN controllers. Used event-driven mirroring of CPU load and flow-table changes to predict controller saturation and trigger proactive load redistribution.
    - Developed adaptive flow-entry timeouts to balance prediction accuracy, first-packet latency, and TCAM use; evaluated synchronous and asynchronous controller notifications to trade off latency and prediction lead time.
    - Designed Bayesian-game router-to-controller assignment using request history, controller capacity, and WAN bandwidth; ran decision logic in controller-side threads to avoid computation on forwarding devices.
    - Designed traffic-aware router selection to relieve controller load while bounding the traffic affected by migration; incorporated flow priorities and link utilization to protect high-priority services.
    - Designed SLA-constrained edge resource allocation using a multi-leader, multi-follower Stackelberg game, matching vCPU and memory demands to available capacity and response-time budgets.
    - Evaluated SD-WAN designs with Floodlight, a 20-node distributed Mininet setup emulating 120 routers under loads up to 24,000 control requests/s, and a separate 12-switch OpenFlow 1.3 testbed; evaluated edge allocation in ns-3.

</details>

<details class="collapsible collapsible--item" id="wasm-based-serverless-framework" open markdown="1">
<summary><h2>WASM Based Serverless Framework</h2></summary>

- Languages Used: Rust, Bash.
- Modules Used: WASM/WASI framework of Rust, Docker, Kubernetes.
- Web-assembly as a potential for developing cloud-based platforms has been gaining a lot of popularity over the last few years. Inspired by the Mozilla-backed open-source projects
of Web-Assembly (WASM) and Web-Assembly System Interface (WASI), this project is a WASM-based runtime that not only provides functionalities of a serverless architecture, but also provides features like CPU, memory and file-system isolation resulting in multi-tenancy within function execution. This also overcomes limitations, like cold-start and complex architecture for stateful services, existing in other serverless implementations. As an extension to this work, we have designed a model for placement and execution of serverless functions as per data-locality, which helps in achieving better execution latency and reduced network usage as compared to existing random function placement strategies.
- This project was presented at leading industrial conferences:
    - "A Poor-man Serverless framework for cloud-based applications using web-assembly", presented at CloudFoundry Summit Europe 2019 and OpenSource Summit Japan 2019
- A sneak-peek of this work was presented in the poster session of the Web Conf 2020. You can find the publication [here](https://dl.acm.org/doi/abs/10.1145/3366424.3382670).

</details>

</details>

<details class="collapsible collapsible--section" id="internship-projects" open markdown="1">
<summary><h1>Internship Projects</h1></summary>

<details class="collapsible collapsible--item" id="stewarded-reference-table-20" open markdown="1">
<summary><h2>Stewarded Reference Table 2.0</h2></summary>

- Team: Enterprise Business Intelligence at Dell International
- Duration: 3 months
- Brief Details: A self-service ETL portal which extracts and modifies (if required) data of a flat delimited file and pushes the data extracted into the Teradata database. This tool caters to over 1500 users of the enterprise

</details>

<details class="collapsible collapsible--item" id="electronic-door-surveillance" open markdown="1">
<summary><h2>Electronic Door Surveillance</h2></summary>

- Brief Details: A product which records and displays the details of the persons who visited the client in his absence.

</details>

</details>

<script>
(function () {
  var sections = document.querySelectorAll('details.collapsible');
  var buttons = document.querySelectorAll('[data-collapsible-action]');
  Array.prototype.forEach.call(buttons, function (button) {
    button.addEventListener('click', function () {
      var open = button.getAttribute('data-collapsible-action') === 'expand';
      Array.prototype.forEach.call(sections, function (d) { d.open = open; });
    });
  });
  function revealTarget() {
    var id = decodeURIComponent(window.location.hash.slice(1));
    var target = id && document.getElementById(id);
    if (!target) { return; }
    for (var node = target; node; node = node.parentElement) {
      if (node.tagName === 'DETAILS') { node.open = true; }
    }
    target.scrollIntoView();
  }
  window.addEventListener('hashchange', revealTarget);
})();
</script>
