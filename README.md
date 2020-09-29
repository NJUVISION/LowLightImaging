# Low-light Color Imaging via Dual Camera Acquisition
[Peiyao Guo ](https://github.com/peiyaoooo) and Zhan Ma  
Vision Lab, Nanjing University  
## Introduction  
As existing low-light color imaging suffers from the unrealistic color representation or blurry texture 
  with a single camera setup, we are motivated to devise a dual camera system using a high spatial resolution (HSR) monochrome camera and 
  another low spatial resolution (LSR)  color camera  for synthesizing the high-quality color image under low-light illumination conditions. 
  The key problem is how to efficiently learn and fuse cross-camera information for improved presentation in such heterogeneous setup with domain gaps (e.g., color vs. monochrome, HSR vs. LSR).
  We have divided the end-to-end pipeline into three consecutive modularized sub-tasks, including the reference-based exposure compensation (refEC), reference-based colorization (refColor)
  and reference-based super-resolution (refSR), to alleviate domain gaps and capture inter-camera dynamics between hybrid inputs. In each step, we leverage the powerful deep neural network (DNN) to respectively transfer and enhance 
  the illuminative, spectral and spatial granularity in a data-driven way. Each module is first trained separately, and then jointly fine-tuned for robust and reliable performance. Experimental results have shown that our work provides the leading performance in synthetic content from popular test datasets when compared to existing algorithms, and offers appealing color reconstruction using real captured 
  scenes from an industrial monochrome and a smartphone RGB cameras, in low-light color imaging application.