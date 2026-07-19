## Hey, I'm Arda 👋
 
I write Rust and think about where data actually slows down.
 
Most of my time goes to the layer underneath AI/ML systems — the part that moves data around. Not the models. The plumbing. I like it because the plumbing is where the interesting failures live: the pipeline that takes 8 hours when it could take a minute, the worker sitting idle because of skew, the network quietly becoming the bottleneck long after you stopped looking at it.
 
I measure before I touch anything. Then I usually find out I was wrong about where the bottleneck was.
 
---
 
### What I build & break
 
* **Arrow, all the way down:** Building high-throughput data layers natively in Rust. Deep diving into DataFusion (custom `TableProvider` implementations, pushdowns, partitioning) and Ballista (distributed execution, plan serialization via gRPC, custom extension codecs).
* **Streaming & Data Movement:** Writing memory-efficient Kafka consumers with `rdkafka` and `async-stream`, balancing backpressure, and handling chunked parallel workers using Tokio.
* **Distributed Infrastructures:** Deploying distributed query engines on Kubernetes via Helm, orchestration with Airflow across multi-node clusters, and handling the specific ways things break at 3 AM.
* **Vector Data Infra:** Scaled vector pipelines to process 4M+ records with embeddings and Qdrant. 

---
 
### Latest Writing
 
**Custom Data Sources in Ballista** — Serving Apache Arrow streams over HTTP via Axum into distributed query engines ([Qiita](https://qiita.com/ardvci/items/274d400302154e595610) · [Zenn](https://zenn.dev/ardvci/articles/cb9c87f59c4a9a))
**Streaming JSON Parsing** — Why the naive NDJSON parsing approach falls apart at scale and how to keep memory under 2MiB ([Qiita](https://qiita.com/ardvci/items/8f4e587de7343f01ba2f))
**Ballista on Kubernetes** — Distributed query execution with DataFusion ([Medium](https://medium.com/@ardvci/rusty-distributed-computation-ballista-more-than-a-query-engine-45387078704b))

---
 
### Tech Stack
 
* **Systems & Data:** Rust (Tokio · Arrow · DataFusion · Ballista) · Python · Scala/Spark · SQL
* **Infra & Ops:** Kafka · Airflow · Kubernetes · GCP · AWS · Qdrant
