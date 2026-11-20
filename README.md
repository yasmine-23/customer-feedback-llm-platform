# Customer Feedback Intelligence & LLM Evaluation Platform

**Status:** Planned

This project builds a repeatable pipeline that turns customer reviews into
structured feedback. A local language model will classify themes and sentiment,
and the pipeline will validate outputs and record the model and prompt version
used for each prediction.

A labeled sample will be used to compare the model with a baseline. The
evaluation will measure classification quality, latency, and invalid outputs.
Incremental processing will reprocess only new reviews or reviews affected
by a change in the model or prompt.

**Stack:** Python, Prefect, Ollama, Parquet, pytest  
**Data:** [Amazon Reviews 2023](https://huggingface.co/datasets/McAuley-Lab/Amazon-Reviews-2023)  
**Deliverables:** Inference pipeline, versioned prompts, evaluation report,
and automated tests.
