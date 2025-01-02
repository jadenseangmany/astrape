# Astrape
A convolution neural network (CNN) accelerator deployed on a field programmable gate array (FPGA), designed for accelerating data compression specifically from spacecraft.
## Motivation
During modern spacecraft expeditions, data compression accuracy and performance is incredibly vital in making accurate analysis in the discoveries we make in space. Spacecraft collects massive amounts of data that include high resolution images of planet surfaces, spectral data, sensor readings, and more. Due to incredibly large distances for data transmission in space, communication links between spacecraft and ground stations are computationally and temporally expensive, and data in deep space may be once in a lifetime observations that must not be lost during compression. Hence, we need to create a lightweight, cost effective, energy efficient, and high performance compression solution that allows us to receive data from deep space within a reasonable time and accurate to ensure life changing discoveries don't go unseen. And that solution is possible through FPGAs.
## High Level Development Workflow
### Altering CNNs
Find an existing CNN that is task specific for general data compression and image preprocessing (neural image codecs), then train it for spacecraft specific data (planet imaging, simulated hyperspectral images, sensor outputs).
### Optimizing for FPGA
Take that CNN and optimize it for FPGA implementation, then we accelerate CNN components (convolution and activation).
### Testing
Find datasets online to test our accelerator, and compare it with CPU and GPU based software acceleration.
