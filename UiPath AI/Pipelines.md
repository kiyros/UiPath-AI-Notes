## Pipelines
### About Pipelines
- A pipeline is a description of an ML workflow, including all of the functions in the workflow and the order of execution of these functions. The Pipeline includes the definition of the inputs required to run the pipeline and outputs to get from this pipeline.
- A Pipeline Run is an execution of a pipeline based on code provided by the user. Once completed a Pipeline Run will have associated outputs and logs.

There are **3** types of pipelines:
- A **Training Pipeline** takes as input an ML Package and a dataset, together producing a new ML package version.
- An **Evaluation Pipeline** takes as input a ML Package Version and a dataset, together producing a set of metrics and logs.
- A **Full Pipeline** essentially runs a data processing function, and a Training Pipeline and an Evaluation Pipeline in succession.

**What happens if there is an already existing model trained?**
- If there is already a model trained, you need to retrain the model. To retrain the model, you should add additional data samples to the initial dataset and create a pipeline on top of ML Package version 12.0 with the bigger dataset. The ML Package version 12.2 stores the knowledge of the model.

**How to run an evaluation pipeline?**  
- To run an evaluation pipeline, it needs to be set up on the ML Package version containing the knowledge of the model from training (Eg: 12.1) on the evaluation dataset.  
- An **evaluation dataset** is a dataset that the model wasn’t trained on, to properly evaluate the performance of the model.
