# Simple Vulkan Computing Pipeline Example

This repository contains a simple example showing how to use the Vulkan computing capabilities.

This example is built with cmake which makes it simpler to build across multiple platforms.

To set up you just need to make sure you have the Vulkan SDK installed, and then you can run `cmake .`.

Example output from program:

```
INFO: Device GeForce GTX 1650
INFO: Finding compute queue
DEBUG: Creating buffer: { TransferSrc | TransferDst }{ HostVisible }128
DEBUG: Creating buffer: { TransferSrc | TransferDst | StorageBuffer }{ DeviceLocal }128
INFO: Copying data from host memory to staging buffer
INFO: Shader file path: shaders/glsl/computeheadless.comp.spv
DEBUG: Reading file
INFO: Converting the read file into module
INFO: Converting to shader stage
Compute input: { 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27, 28, 29, 30, 31,
}
Compute output: { 38, 8, 10, 12, 30, 32, 34, 36, 54, 56, 58, 60, 78, 80, 82, 84, 102, 104, 106, 108, 126, 128, 130, 132, 150, 152, 154,
 156, 174, 176, 178, 148, }
Finished.
```

