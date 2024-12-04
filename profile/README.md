# ISOLDE AUTOMOTIVE DEMONSTRATOR

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
## Open-Source: GEMM (General Matrix Multiply) acceleration as a computational backbone in Digital Signal Processing (DSP) pipelines
An example of a DSP pipeline is estimating the relative velocity of objects in a RADAR system. The computation involves Fast Fourier Transforms (FFTs) which in turn, can be expressed in terms of matrix multiplications (via the Cooley-Tukey algorithm).
The demonstrator will feature:   
-	two or more RedMulE(Reduced-Precision Matrix Multiplication Engine) instances.
-	a RISC-V core: ibex(fork)
-	compiler2 support for splitting the original GEMM operation in two or more sub-GEMMs. The sub-GEMMs will be executed in parallel, using the multiple RedMulE instances available in the system.
-	investigation of using OpenMP for allocating the sub-GEMMs to RedMulE instances (in collaboration with NXP-RO).
