# Agentic Fraud Triage Eval
Designing Fraud Triage framework for fraud detection on IEEE CIS data set.
Architecture :
IEEE CIS csv data -> (Kafka/ Redpanda) Stream -> XGBoost Baseline(Yet to evaluate right model here)
-> Triage Logic (If fraud / non fraud certainity < 90% pass it to agentic framework else directly to decision log ) -> Agentic Evaluation of Unsure Cases (LangGraph AI Agent, Vector Embeddings stored @  QDrant Db / Redis cache) -> Decision Log (Graphana) -> Evaluation(Model alone with Model + Agent, Pass^k consistency , Pass@k(for my sake lol) -> Evaluation: Cost/Speed/Failure -> Reporting -> OSS eval Tool Repo integration   
