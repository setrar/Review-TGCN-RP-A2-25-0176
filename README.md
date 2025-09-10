# Review-TGCN-RP-A2-25-0176
Review of Reducing the Energy Footprint of 5G: A gNB on MPSoC with Low-Power FFT Acceleration

### Abstract TGCN-RP-A2-25-0176
Open, virtualized architectures are reshaping cellular networks but purely software-based 5G deployments often struggle to meet strict real-time requirements.

Thus, accelerators are often utilised even at the expense of a high energy consumption. 

In this paper, we propose and demonstrate an energy-efficient solution that accelerates Fast Fourier Transform (FFT) computations by placing Low-PHY functions in an MPSoC FPGA. Moreover, by placing High-PHY layer functions in the CPU of the same MPSoC, we eliminate host-to-accelerator bottlenecks (e.g., accelerator to processor transfer time) that typically limit hardware speedups and contribute to unnecessary energy expenditure.

Though implemented into a single MPSoC, the solution is compatible with Open RAN solutions, such as the one proposed by the Small Cell Forum (SCF) in the 5G function application platform interface (5G-FAPI). 

We validate our MPSoC-based gNB architecture using OpenAirInterface. Experimental results demonstrate that the MPSoC-based approach achieves up to 13× speedup compared to CPU-based implementations, particularly for larger FFT sizes, which directly contributes to reduced energy consumption per processed task.

Furthermore, a detailed power consumption analysis shows that, while the processing system remains a significant energy consumer, hardware acceleration enhances overall energy efficiency by shifting computationally intensive tasks to dedicated, optimized hardware, thereby substantially reducing the energy consumption for these demanding functions and paving the way for greener 5G deployments.

