# Awesome-Change-Data-Capture-Platform

## Top Change Data Capture (CDC) Platforms Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Log-Based CDC, Real-Time Database Replication, Streaming Change Events & Data Pipeline Integration*

**Last updated: September 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Change Data Capture (CDC)**. These systems capture row-level inserts, updates, and deletes from databases in near real time and stream them to message buses, warehouses, or other systems for analytics, microservices, and replication.



**Examples** include Debezium, Estuary, Fivetran HVR, Qlik Replicate, Striim, Confluent Cloud CDC, Oracle GoldenGate, Airbyte CDC, Upsolver, StreamKap, Debezium Cloud, Fivetran, HVR by Fivetran, Airbyte, PeerDB, Airbyte Cloud, Confluent CDC, and Hevo Data (the category leaders).



**Open-source emphasis**: CDC has a strong open-source core. **Debezium** is the de facto standard for log-based CDC into Kafka and beyond. Additional open projects (PeerDB, Flink CDC, Maxwell, Canal, and others) expand the ecosystem. This section is heavily expanded.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-products)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

- **[Debezium (Cloud / Managed offerings)](https://debezium.io/)**  

  Managed and commercial distributions built on the leading open-source CDC platform for streaming database changes.



- **[Estuary](https://estuary.dev/)**  

  Managed CDC and data movement platform with exactly-once delivery, flexible destinations, and hybrid deployment options.



- **[Fivetran / HVR by Fivetran](https://www.fivetran.com/)**  

  Fully managed ELT and enterprise-grade database replication (HVR) for high-volume CDC into warehouses and lakes.



- **[Qlik Replicate](https://www.qlik.com/)**  

  Enterprise data replication and CDC platform for heterogeneous database and cloud target synchronization.



- **[Striim](https://www.striim.com/)**  

  Low-code streaming and CDC platform for continuous replication, migrations, and real-time pipelines.



- **[Confluent Cloud CDC](https://www.confluent.io/)**  

  Managed CDC connectors and change-event streaming on Confluent Cloud, tightly integrated with Kafka.



- **[Oracle GoldenGate](https://www.oracle.com/integration/goldengate/)**  

  Enterprise real-time data replication and CDC solution for Oracle and heterogeneous databases.



- **[Airbyte (Cloud / CDC connectors)](https://airbyte.com/)**  

  Open-core data integration platform with CDC support across many sources and a managed cloud offering.



- **[Upsolver](https://www.upsolver.com/)**  

  Streaming data platform with CDC ingestion and transformation for lakehouse and analytics use cases.



- **[StreamKap](https://streamkap.com/)**  

  Managed real-time CDC platform focused on sub-second latency and operational streaming pipelines.



- **[Hevo Data](https://hevodata.com/)**  

  No-code data pipeline platform with CDC capabilities for warehouse and analytics destinations.



- **[PeerDB (Cloud options)](https://www.peerdb.io/)**  

  Postgres-oriented CDC and replication platform with open-source roots and managed offerings.



## Open-Source GitHub Projects

- **[Debezium](https://github.com/debezium/debezium)**  

  Leading open-source CDC platform—captures row-level changes from many databases and streams them via Kafka Connect (or Debezium Server).



- **[Debezium Server](https://github.com/debezium/debezium-server)**  

  Standalone runtime for Debezium connectors without a full Kafka Connect cluster—streams to Kafka, Pulsar, Kinesis, and more.



- **[PeerDB](https://github.com/PeerDB-io/peerdb)**  

  Open-source Postgres-first CDC and replication tool optimized for high-performance streaming to warehouses and queues.



- **[Apache Flink CDC](https://github.com/apache/flink-cdc)**  

  Flink-based CDC connectors and framework for capturing and processing database changes in streaming jobs.



- **[Maxwell’s Daemon](https://github.com/zendesk/maxwell)**  

  Open-source MySQL binlog CDC tool that outputs change events as JSON to Kafka, Kinesis, or other targets.



- **[Canal](https://github.com/alibaba/canal)**  

  Alibaba’s open-source MySQL binlog incremental subscription and consumption component widely used in China and beyond.



- **[Airbyte open-source CDC connectors](https://github.com/airbytehq/airbyte)**  

  Open-source data integration platform with CDC modes for supported databases alongside batch sync.



- **[pgoutput / logical decoding open tools](https://github.com/)**  

  Community utilities around Postgres logical replication and decoding for custom CDC pipelines.



- **[Documentation and Debezium playbooks](https://debezium.io/documentation/)**  

  Official guides for connectors, schema evolution, signaling, and production deployment patterns.



- **[CDC example stacks and tutorials](https://github.com/)**  

  Docker Compose and lab repositories demonstrating Debezium + Kafka + warehouse end-to-end flows.



### Additional Strong Open-Source Options

- Standardizing on **Debezium** + Kafka (or Debezium Server) for most relational CDC needs.

- Using **PeerDB** when Postgres-to-warehouse latency and simplicity are priorities.

- Combining **Flink CDC** when change streams must be processed with complex streaming logic.

- Accepting that fully managed operations, ultra-broad connector catalogs, enterprise support, and zero-ops scale still drive adoption of commercial platforms (Fivetran/HVR, Striim, Qlik Replicate, Oracle GoldenGate, Estuary, StreamKap, Confluent Cloud, etc.).

- Focusing open-source efforts on ownership of the change stream, cost control, and deep customization.



**Frameworks for building custom systems**: Capture with Debezium or PeerDB → stream via Kafka/Pulsar → land in a warehouse or serve microservices → monitor lag and schema changes. Suitable for data and platform engineering teams. Many organizations run open CDC cores with managed Kafka or commercial overlays for operations.



## How to Contribute

1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.

- CDC systems read production database logs and can impact source load. Test thoroughly, monitor lag, and plan for schema changes. This list is not operational advice.



---

**Made for data engineers, platform teams, and open-source streaming advocates.**

Let's keep change streams reliable, portable, and as open as practical.
