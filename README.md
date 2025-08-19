# The Open Health Natural Language Processing Toolkit (OHNLPTK)
This is the Documentation and Status Tracking Repository for the Open Health Natural Language Processing Toolkit. Please refer to individual component repositories for relevant source code (linked below)

## OHNLPTK Components (for End Users)
- [Backbone](https://www.github.com/OHNLP/Backbone): OHNLPTK's pipeline execution engine based on [Apache Beam](https://beam.apache.org/) allowing for JSON-configurable, modular, plug-and-play execution of data transformation pipelines at scale (including support for popular frameworks such as Apache Spark, Apache Flink, GCP Dataflow, and Azure Databricks). Includes built in adapters for a variety of data sources
- [BackboneConfigurator](https://www.github.com/OHNLP/BackboneConfigurator): User Interface for Editing and Configuring Backbone Pipelines
- [MedTagger](https://www.github.com/OHNLP/MedTagger): NLP for General Clinical Information Extraction Tasks as part of Backbone Pipelines
- [MedXN](https://www.github.com/OHNLP/MedXN): An extension of MedTagger specifically tuned for drug extraction
- [PresidioDeidentificationforOHNLPTK](https://www.github.com/OHNLP/presidiodeidentificationforohnlptk): Wraps Microsoft's [Presidio SDK](https://microsoft.github.io/presidio/) to allow for De-identification and Synthetic Replacement of Clinical Text as part of Backbone Pipelines using any trained Huggingface-hub-format-compatible PII recognizer BERT-based model

## OHNLPTK Components (for Developers)
- [backbone API](https://github.com/OHNLP/Backbone/tree/master/API): Java API for Backbone. Use this as a basis for implementing your own java-based Backbone pipeline components. Also contains code for java-python bridge implementation to allow for mixing languages amongst different components
- [backbone-xlang-python](https://www.github.com/OHNLP/backbone-xlang-python): Python API for Backbone. Use this as a basis for implementing your own python-based Backbone pipeline components
- [ohnlptk-ml](https://www.github.com/OHNLP/ohnlptk-ml): Various machine learning API extensions for Backbone. Extend this to implement federated learning on BYO pytorch models using FedAVG as part of Backbone pipelines

## Legacy
- [Demonstration Website](https://github.com/OHNLP/ohnlptk): Contains a (now partially defunct) demonstration website for the OHNLP toolkit. This repository is not kept up to date and is not compatible with the latest OHNLP Toolkit features. A replacement demonstration website/code rewrite is in progress that supports more generalized features beyond N3C-related phenotypes.
