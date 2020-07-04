---
layout: archive
title: ""
permalink: /projects/
author_profile: true
---

# Projects at SAP
- ## Mobile Development Kit (MDK)
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

- ## Service-Fabrik Broker
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

- ## Service-Fabrik Backup & Restore Library
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

- ## CloudFoundry CLI Plugin
    - Team: SAP Cloud Platform
    - Project Duration: 8 months
    - Modules Used: CloudFoundry, Docker, Kubernetes.
    - Languages Used: Go.
    - Github: [https://github.com/cloudfoundry-incubator/service-fabrik-cli-plugin](https://github.com/cloudfoundry-incubator/service-fabrik-cli-plugin)
    - Designed and developed CloudFoundry-based CLI plugin to create/manage backup and restore for backing services like Postgresql, Redis and MongoDb. The project is now Cloudfoundry-incubated.

# Entrepreneurship
- ## Hubris by SAP
    - Role: Co-founder and Tech Lead
    - Duration: 1 year
    - About: Hubris was a recommendation engine that could automatically tune databases and applications as per the unique needs of the user. It removed any need of manual intervention by a Database Admin and aimed to provide accurate and tailor-made recommendations for each unique scenario. This was a generic product that could be paired with any kind of database and a standard database could be made autonomous with this offering. During the run of 1 year, Hubris catered to nearly 8 companies (small/mid-scale customers).
    - Entrepreneurial Contributions:
        - Designed the business model, revenue projections, marketing models, FTE resource allocations, etc. 
        - Acquired a customer group of 1 Large Enterprise and 5 Small Enterprises. 
        - Presented the idea in the Innvent Startup Challenge 2019, adjudged as the best startup idea in the event
        - Presented the incubation of idea in SAP Accelerator, Potsdam/Berlin, 2019
        - Presented the idea to SAP Executive Board in Los Angeles for seeking seed funding
        - Winner of SAP Stellar Award for Nascent Entrepreneurship 2019 for contributions to Hubris
    - Technical Contributions:
        - Developed the ML model based on Bayesian Optimisation leveraging real-time experiences
        - Designed a prototype for tuning of multiple-databases like PostgreSQL, MySQL, SAP HANA and AWS RDS
        - Identified the bottlenecks in performance of the Autonomous Services architecture. Designed and implemented a framework to run the Autonomous Services as part of SAP Cloud Platform micro-services offering
        - Developed a throttling-detection architecture to make the Autonomous Services scalable and robust for a Multi-Cloud PaaS Architecture
        - Designed framework for tuning of applications running on Java platform

# Research Projects
- ## WASM Based Serverless Framework
    - Languages Used: Rust, Bash.
    - Modules Used: WASM/WASI framework of Rust, Docker, Kubernetes.
    - Web-assembly as a potential for developing cloud-based platforms has been gaining a lot of popularity over the last few years. Inspired by the Mozilla-backed open-source projects
    of Web-Assembly (WASM) and Web-Assembly System Interface (WASI), this project is a WASM-based runtime that not only provides functionalities of a serverless architecture, but also provides features like CPU, memory and file-system isolation resulting in multi-tenancy within function execution. This also overcomes limitations, like cold-start and complex architecture for stateful services, existing in other serverless implementations. As an extension to this work, we have designed a model for placement and execution of serverless functions as per data-locality, which helps in achieving better execution latency and reduced network usage as compared to existing random function placement strategies.
    - This project was presented at leading industrial conferences:
        - "A Poor-man Serverless framework for cloud-based applications using web-assembly", presented at CloudFoundry Summit Europe 2019 and OpenSource Summit Japan 2019
    - A sneak-peek of this work was presented in the poster session of the Web Conf 2020. You can find the publication [here](https://dl.acm.org/doi/abs/10.1145/3366424.3382670).

- ## Hybrid Distributed Collaborative Filtering Recommender Engine
    - Keywords: Recommendation System, Big Data Tools, Apache Spark, Collaborative Filtering, Machine Learning, K-means Clustering. 
    - Brief Details: The aim of the paper is to design a movie-recommendation engine using an algorithm which overcomes many disadvantages put forward by the prevalent techniques. The paper tries to leverage the benefits of big data tools and clustering techniques in-order to improve the throughput and maintain scalability of the engine.

# Internship Projects
- ## Stewarded Reference Table 2.0
    - Team: Enterprise Business Intelligence at Dell International
    - Duration: 3 months
    - Brief Details: A self-service ETL portal which extracts and modifies (if required) data of a flat delimited file and pushes the data extracted into the Teradata database. This tool caters to over 1500 users of the enterprise

- ## Electronic Door Surveillance
    - Brief Details: A product which records and displays the details of the persons who visited the client in his absence.