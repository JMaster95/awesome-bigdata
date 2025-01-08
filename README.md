# awesome-bigdata

## Data Storage 
### 1. **PostgreSQL**
- **简介**: 高性能开源关系型数据库，支持复杂查询、事务处理以及扩展性。
- **特点**:
  - 支持 ACID 和事务处理。
  - 丰富的数据类型支持（JSON, XML, ARRAY 等）。
  - 可扩展性强，通过插件（如 PostGIS、TimescaleDB）实现更多功能。
- **适用场景**:
  - 数据分析、业务系统、时间序列存储。
- **官网**: [https://www.postgresql.org](https://www.postgresql.org)

### 2. **MySQL**
- **简介**: 一款流行的开源关系型数据库，社区版和企业版均可用。
- **特点**:
  - 易于使用，支持多种存储引擎（InnoDB、MyISAM）。
  - 支持主从复制和高可用性方案。
  - 社区活跃，支持广泛的开发语言和框架。
- **适用场景**:
  - Web 应用、内容管理系统。
- **官网**: [https://www.mysql.com](https://www.mysql.com)

### 3. **MongoDB**
- **简介**: 一款 NoSQL 文档型数据库，使用 JSON 类似的 BSON 格式存储数据。
- **特点**:
  - 灵活的数据模式（Schema-less）。
  - 高可扩展性，支持分片和副本集。
  - 强大的查询和索引功能，支持地理空间数据。
- **适用场景**:
  - 大数据应用、实时分析、非结构化数据存储。
- **官网**: [https://www.mongodb.com](https://www.mongodb.com)

### 4. **Apache Cassandra**
- **简介**: 分布式 NoSQL 数据库，专为处理大规模、高可用性数据设计。
- **特点**:
  - 高可扩展性，线性扩展节点。
  - 去中心化架构，无单点故障。
  - 支持时间序列数据和宽表存储。
- **适用场景**:
  - 日志数据存储、IoT 数据存储。
- **官网**: [https://cassandra.apache.org](https://cassandra.apache.org)

### 5. **Redis**
- **简介**: 一款开源的内存数据库，支持多种数据结构（String、Hash、List 等）。
- **特点**:
  - 高速性能，数据存储在内存中。
  - 支持持久化选项（AOF 和 RDB）。
  - 内置分布式功能，适合高并发场景。
- **适用场景**:
  - 缓存、会话存储、消息队列。
- **官网**: [https://redis.io](https://redis.io)

### 6. **Elasticsearch**
- **简介**: 开源分布式搜索引擎，基于 Lucene 构建。
- **特点**:
  - 全文搜索、高速查询。
  - 可视化工具 Kibana 集成。
  - 支持复杂的聚合和分析功能。
- **适用场景**:
  - 日志分析、全文检索。
- **官网**: [https://www.elastic.co](https://www.elastic.co)

### 7. **Hadoop HDFS**
- **简介**: 分布式文件系统，Hadoop 的核心组件之一。
- **特点**:
  - 高吞吐量数据访问，适合大数据存储。
  - 支持容错和高可用性。
  - 与 MapReduce、Spark 等生态系统集成。
- **适用场景**:
  - 大数据存储与处理。
- **官网**: [https://hadoop.apache.org](https://hadoop.apache.org)

### 8. **Apache HBase**
- **简介**: 开源分布式 NoSQL 数据库，运行在 HDFS 之上。
- **特点**:
  - 高度可扩展，适合海量结构化和半结构化数据。
  - 强一致性，低延迟读写。
  - 与 Hadoop、Spark、Hive 深度集成。
- **适用场景**:
  - 大数据实时查询、时序数据存储。
- **官网**: [https://hbase.apache.org](https://hbase.apache.org)

### 9. **ClickHouse**
- **简介**: 高性能的列式存储数据库，专注于实时分析。
- **特点**:
  - 高效的列式存储，查询速度快。
  - 支持 SQL 查询语法。
  - 适合海量数据的聚合分析。
- **适用场景**:
  - 实时分析、BI 工具集成。
- **官网**: [https://clickhouse.com](https://clickhouse.com)

### 10. **Apache Hive**
- **简介**: 大数据批处理 SQL 查询工具，运行在 Hadoop 之上。
- **特点**:
  - SQL 风格查询语言 HiveQL。
  - 与 HDFS 和 MapReduce 深度集成。
  - 支持 UDF 扩展。
- **适用场景**:
  - 大数据批量查询。
- **官网**: [https://hive.apache.org](https://hive.apache.org)
  
## Data Warehouse

### Apache Iceberg

**简介**  
Iceberg 是一个高性能的表格式，用于大规模数据湖管理，支持高效的数据读写和版本控制。

**特点**  
- 支持表级事务和数据快照。  
- 高效处理大规模分区和元数据管理。  
- 与 Spark、Flink、Presto 等大数据工具兼容。  

**使用场景**  
- 数据湖中大规模表管理和查询优化。  
- 分析和处理结构化和半结构化数据。  

**官网**  
[https://iceberg.apache.org](https://iceberg.apache.org)

## Data Lake

### Delta Lake

**简介**  
Delta Lake 是一个基于 Apache Spark 的开源存储层，提供 ACID 事务支持，确保数据湖中的数据质量和一致性。

**特点**  
- 支持 ACID 事务，保障数据完整性。  
- 高性能增量数据处理。  
- 支持数据版本管理和时间旅行（Time Travel）。  

**使用场景**  
- 数据湖中的数据治理与质量保障。  
- 增量数据加载与分析。  

**官网**  
[https://delta.io](https://delta.io)

### Apache Hudi

**简介**  
Hudi 是一个流式数据湖平台，用于管理存储在 HDFS 或云上的大规模数据，支持实时数据插入和查询。

**特点**  
- 支持实时更新和查询。  
- 提供增量数据处理能力。  
- 集成流处理框架，如 Kafka 和 Flink。  

**使用场景**  
- 实时数据湖分析与更新。  
- 构建数据流管道，实现数据变化捕获（CDC）。  

**官网**  
[https://hudi.apache.org](https://hudi.apache.org)

### Alluxio

**简介**  
Alluxio 是一个分布式存储系统，作为跨平台的虚拟数据湖层，用于统一访问多种存储后端。

**特点**  
- 提供跨云和本地存储的统一访问。  
- 支持多种存储后端（HDFS、S3、GCS）。  
- 提高存储访问性能，通过数据缓存加速计算。  

**使用场景**  
- 构建多云或混合云数据湖。  
- 数据湖存储访问优化和加速。  

**官网**  
[https://www.alluxio.io](https://www.alluxio.io)

### Data Cloud
## Data Integration 
## Data Clean
## Data Compute
## Data Model
## Data Safe
## Data Report
## Data Lifecycle
## Data 

