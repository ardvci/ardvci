## Hey, I'm Arda 👋
 
I write Rust and think about where data actually slows down.
 
Most of my time goes to the layer underneath AI/ML systems — the part that moves data around. Not the models. The plumbing. I like it because the plumbing is where the interesting failures live: the pipeline that takes 8 hours when it could take a minute, the worker sitting idle because of skew, the network quietly becoming the bottleneck long after you stopped looking at it.
 
I measure before I touch anything. Then I usually find out I was wrong about where the bottleneck was.
 
---
 
### Focus areas
 
**Arrow, all the way down.** Columnar memory is the thing that makes everything else possible — once data is in Arrow, it stops paying serialization tax every time it crosses a boundary. I work on top of that: DataFusion (custom sources, how pushdown propagates into the scan, where partitioning gets decided), Ballista (plan serialization, distributed execution), Arrow IPC and zero-copy reads.
 
**Streaming & data movement.** Kafka ingestion, backpressure, bounded memory under load. Rust with Tokio — chunked parallel workers, channels bridging blocking I/O with async tasks.
 
**Distributed systems on Kubernetes.** Airflow across 10+ nodes, Ballista via Helm, Spark for the heavy batch stuff. Skew, shuffle, resource sizing, and the specific way things break at 3am.
 
**Vector search & embeddings.** Mapped 4M+ records across providers with embeddings and Qdrant. This is where the data infra work starts touching ML directly, and it's the direction I keep gravitating toward.
 
---
 
### Writing
 
- [Streaming JSON parsing](https://qiita.com/ardvci/items/8f4e587de7343f01ba2f) — why the naive approach falls apart at scale
- [Ballista on Kubernetes](https://medium.com/@ardvci/rusty-distributed-computation-ballista-more-than-a-query-engine-45387078704b) — distributed query execution with DataFusion
- I write in English and Japanese. Mostly on [Qiita](https://qiita.com/ardvci) & [Medium](https://medium.com/@ardvci).
---
 
### 🧰 Tools
 
`Rust` (Tokio · Arrow · DataFusion · Ballista) · `Python` · `Scala/Spark` · `SQL`
`Kafka` · `Airflow` · `Kubernetes` · `GCP` · `AWS` · `BigQuery` · `Qdrant`
