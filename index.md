 # Decision Graph                                                                                                                                                                                       
                                                                                                                                                                                                           
  >  **decision structures for smarter AI**: Representing the choices, actions, and communications actors (agent, humans, and hybrid systems) make to provide deep decision making context to AI systems.                  
                                                                                                                                                                                                           
Map any decision-making context, including OpenTelemetry agent traces, into 

1. Contntext graph (Neo4j or any property-graph database)
2. Analytics-ready tabular data (Arrow / Parquet) for ML training pipelines, RL, and agentic research.
                                                                                                                                                                                                           
  ## Projects                                               

  | Repo | Status | Purpose |
  |---|---|---|
  | **[decision-graph](https://github.com/decision-graph/decision-graph)** [![PyPI](https://img.shields.io/pypi/v/decision-graph?include_prereleases&label=PyPI)](https://pypi.org/project/decision-graph/) | alpha — `dg/v1` | The schema — `spec.json`, design rationale, reference Python package with bundled spec and instance validator. |                                                                    
  | **[otela](https://github.com/decision-graph/otela)** [![PyPI](https://img.shields.io/pypi/v/otela?label=PyPI)](https://pypi.org/project/otela/) | shipped — `at/v2` | OpenTelemetry agent-trace ingestion. Normalizes OTLP/JSON to Arrow / Parquet today; the `dg/v1` generator is the next addition. |
  | **otel-to-neo4j (https://github.com/decision-graph/otel-to-neo4j)** | Working Batch Agent Trace Ingestion | Neo4j-specific loader for OTel agent traces. Built on otela; loads at/v2 tables into a Neo4j graph. |
                                                            
