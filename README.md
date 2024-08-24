# GPU-benchmark-for-deep-learning-applications

This repo will include the GPU performance benchmark targeting deeplearning applications. This bench mark has been used in the EQ-ViT and SSR work.

## to-do list
- Scripts
  - The current code structure is not a good one when serving as a benchmarking tool, since (1)the model files is mannualy installed, (2)the tensorRT tool environment chain is a bit complicated.
  - Providing a docker container(with dockerfile) together with the source scripts
  - Add a script to download the source files of different models
  - For the pytorch-onnx-TensorRT compilation flow, (1) re-write the torch-->onnx scripts (2)the onnx-->trt python script seems could be replaced by the simple command line tools of trtexec, should compare the difference (3)the INT8 calibration part should be checked 
  - For the performance measurement, use the flags to control the output of nsys and ncu profiles.
- documentations
  - quick start: docker install + shell example
  - install: (1) use docker (2) build docker locally (3) install locally 
  - compilation flow: (1)pytorch-onnx-trt flow, (2)onnx-->trt flow
  - performance measurement
  - version control: the version of pytorch, onnx and trt
  - test results: the results on different hw platforms
