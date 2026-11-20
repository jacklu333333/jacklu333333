# I-Hao (Jack) Lu

**Ph.D. candidate in Computer Science · KAIST**
Generative models for inertial sensing · efficient ML systems

Taipei, Taiwan · [jacklu333333@kaist.ac.kr](mailto:jacklu333333@kaist.ac.kr) · [GitHub](https://github.com/jacklu333333)

I am a Ph.D. candidate at KAIST, advised by Prof. Dong-Soo Han, working on generative models and systems for inertial motion estimation and indoor positioning. My work spans diffusion, flow, and bridge-matching models; distributed training; GPU and edge inference; and the embedded hardware used to collect sensor data.

## Research interests

- **Generative modeling for inertial sensing** — diffusion models, flow matching, bridge matching, and VAEs for dense pedestrian motion estimation and IMU trajectory denoising.
- **Indoor positioning** — pedestrian dead reckoning, particle filters, GNSS/IMU fusion, Wi-Fi fingerprinting, and BLE RSSI analysis.
- **Efficient ML systems** — TensorRT/ONNX deployment, INT8 quantization-aware training, DeepSpeed ZeRO-2, and multi-server LLM serving on k3s.
- **Embedded and FPGA systems** — ESP32/STM32 firmware, Jetson/Coral/Raspberry Pi deployment, and HLS4ML accelerators.

## Selected research

**PedestrianDiffusion — IEEE Internet of Things Journal, 2026**
Diffusion-based dense pedestrian inertial motion estimation. Reduced absolute trajectory error by ~20% versus conventional filtering baselines, and scaled training to ~2B parameters on six GPUs with DeepSpeed ZeRO-2, identifying the sub-1 Gbit/s Ethernet interconnect as the scaling bottleneck.
[Code](https://github.com/jacklu333333/PedestrianDiffusion)

**PRIME — ICRA 2027 (under review)**
Predictive real-time inertial motion estimation. Built a TensorRT FP32 engine from ONNX for Jetson Orin Nano (15 W) running in under 7 ms per inference; benchmarked FP32 against INT8 and characterized TensorRT/CUDA execution-split overhead.

**InertialBridge — ICLR 2027 (under review)**
Structure-aware denoising of IMU trajectories using a variational-autoencoder-conditioned bridge-matching model.

**Edge and FPGA deployment**
Deployed diffusion and flow-matching models on Coral Edge TPU (INT8 QAT) and Raspberry Pi (ONNX), ran TFLite Micro classification on ESP32, and designed an IMU-correction accelerator for a GNSS+IMU chip on Artix-7 100T within the LUT budget using HLS4ML.

**Multi-server LLM serving**
Deployed qwen3.8:27b, qwen3.5:122b, and gemma4 models across eight GPUs on five servers with k3s and Ollama, using one replica per server after measuring that inter-server networking was too slow to pool GPUs.

## Publications

- **I.-H. Lu**, D.-S. Han. "PedestrianDiffusion: Spectral Noise-Conditioned Dense Pedestrian Inertial Motion Estimation." *IEEE Internet of Things Journal*, 2026.
- **I.-H. Lu**, D.-S. Han. "PRIME: Predictive Real-Time Inertial Motion Estimation." *ICRA 2027* (under review).
- **I.-H. Lu**, D.-S. Han. "InertialBridge: Efficient Structure-Aware Denoising of IMU Trajectories via Variational Autoencoder Conditional Bridge Matching." *ICLR 2027* (under review).
- **I.-H. Lu**, D.-S. Han. "Optimizing GNSS Indoor/Outdoor Detection: Balancing Observation Window and Sampling for Accuracy and Responsiveness." *IPIN 2024*.
- J. Kim, J. Park, **I.-H. Lu**. "Hyperbutton: In-Video Question Answering via Interactive Buttons and Hyperlinks." *Asian CHI Symposium 2021*.

## Experience

**Graduate Researcher**, KAIST — Sep 2020–present
Developed particle-filter and PDR positioning for IMU-positioning projects sponsored by Korea's Agency for Defense Development and for a firefighter positioning project. Handed off algorithms to hardware and smartphone teams, including a fixed-weight ONNX model and a C port of a Python particle filter. Mentored a master's student and presented ROS, reinforcement-learning, and positioning demos to sponsors and visitors.

**Research Intern**, ISILAB, KAIST — Nov 2019–Aug 2020
Collected and analyzed BLE RSSI traces for contact tracing, showing that link asymmetry and interference make distance thresholds unreliable.

**Embedded Systems Intern**, Tang Wang Green Energy Technology — Sep 2018–Jan 2019
Developed C firmware for microcontroller-based electric-vehicle and golf-cart controllers.

## Education

- **KAIST** — M.S.–Ph.D. in Computer Science, Sep 2020–Feb 2027 (expected). Advisor: Prof. Dong-Soo Han.
- **National Tsing Hua University** — B.S. in Computer Science, Sep 2016–Jun 2020.

## Technical skills

- **ML:** PyTorch, PyTorch Lightning, Hugging Face Diffusers and Transformers, DeepSpeed (ZeRO-2), ONNX, TensorRT (FP32/INT8), TFLite, HLS4ML
- **Systems:** Linux, Docker, k3s/Kubernetes, Ollama, ROS, Google Cloud
- **Embedded:** ESP32, STM32, Jetson Nano/Orin Nano, Coral Edge TPU, Raspberry Pi 4/5, Artix-7 FPGA; UART, SPI, I2C
- **Languages:** Python, C++, C, SystemVerilog/Verilog, JavaScript, Java
- **Methods:** Diffusion models, flow and bridge matching, VAEs, particle filters, PDR, GNSS/IMU positioning

## Public code

- [PedestrianDiffusion](https://github.com/jacklu333333/PedestrianDiffusion) — diffusion-based pedestrian inertial navigation
- [GATIS](https://github.com/jacklu333333/GATIS) — transformer for inertial indoor/outdoor detection

More public repositories: [github.com/jacklu333333?tab=repositories](https://github.com/jacklu333333?tab=repositories)

## Contact

- Email: [jacklu333333@kaist.ac.kr](mailto:jacklu333333@kaist.ac.kr)
- GitHub: [@jacklu333333](https://github.com/jacklu333333)
- Location: Taipei, Taiwan
- Available for full-time research and engineering roles from March 2027.
