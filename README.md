# mlrun-huggingface-demo

This demo contain 2 notebooks: pipeline.ipynb and serving.ipynb.

* The pipeline notebook shows how to create a real-time pipeline with MLRun which fine-tune a model by a dataset that are loaded from the [HuggingFace Hub](https://huggingface.co/docs/hub/index).
The pipeline consist from 4 steps:
  1. **Dataset preparation** - Includes Loading data from the HuggingFace hub and applying tokenization (both train and test datasets).
  2. **Train** - Loading a model from the hub, train and evaluation.
  3. **Optimize** - Optimize the model with ONNX
  4. **Serve** - Deploy a serving function with preprocess and postprocess functions.

* The serving notebook shows how to deploy a serving function for huggingface models.

Both notebooks are ended with a gradio interface for infering the huggingface models. Gradio is a friendly web interface which is a good way to demo ML models. 

