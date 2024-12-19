# TensorRT-Triton-ONNX Testing Roadmap

## TensorRT Testing (https://github.com/triton-inference-server/tutorials)
- Basic LLM and VLM deployment testing
- Adding dynamic batching and scheduling mechanisms
- Understanding ensemble with LLM (tokenizer, post-process)
- Semantic-Cache, Iterative Scheduling, Constraint decoding (for formatted output)
- Basic Tool Calling and Tool Calling with Triton
- Migration guide
> **Goal**: Successfully test with Llama3 VTS

## TensorRT-LLM Testing (https://github.com/triton-inference-server/tensorrtllm_backend)
- Model Parallelism
- Key-Value Cache
- Decoding
- Chunk Context, Lora
- Benchmarking
> **Goal**: Advanced testing with Llama3 VTS, experiment with T5 translation and VTS summarization

## ONNX Testing (https://github.com/yester31/TensorRT_Examples)
- Creating TensorRT Model from ONNX (CPP, Python, Polygraphy)
- Dynamic shape (dynamic batch, dynamic input size)
- Custom Plugin (CUDA preprocessing)
- Modifying ONNX graph with ONNX GraphSurgeon
- Optimization: PTQ, QAT, Sparsity, Pruning, Distillation
> **Goal**: Optimize and deploy ONNX on TensorRT with practical applications (testing with license plate and car style recognition)

## Additional Objectives
- Understand and measure performance & accuracy
- Learn and implement several blueprints (self-built PDF extraction)
- Deploy LLM on CPU:
  * GGUF
  * GGML
  * .cpp

> **Final Goal**: Ability to self-build and host optimized models on Dify
