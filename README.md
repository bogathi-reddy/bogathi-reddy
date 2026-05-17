# Hi, I'm Bogathi Reddy 👋

**Physicist specializing in optical modeling, lithography imaging, and physics-inspired AI frameworks.**

I combine an industrial background in advanced euv lithography with modern computational engineering, deep learning, and advanced mathematical optimization. I am currently building a modular portfolio from first principles to showcase scalable solutions for both forward optical transport and complex inverse engineering problems.

---

## 🔬 Core Portfolio Architecture

### 1. Computational Optics & Metrology Engine (`optics-inverse-problems`)
*A comprehensive physics-based simulation and optimization toolkit modeling light propagation from source to sensor.*

*   **A. Forward Lithography Engine**
    *   **Imaging Formulations:** Implementations of **Abbe’s Method** (source-point integration) versus the computationally efficient **Hopkins Formulation** (Transmission Cross Coefficients - TCC) for coherent, partially coherent, and incoherent imaging conditions.
    *   **Optical Column Control:** Full forward modeling of source spatial coherence, custom illumination pupil shaping (annular, quadrupole), projection lens aberrations (Zernike polynomials), and defocus.
    *   **System Parameters:** Parameterized control over Numerical Aperture ($NA$), system magnification ($M$), illumination profiles ($\sigma$), and resist-level thresholds.

*   **B. Wavefront Sensing & Shearing Interferometry**
    *   **Interferometric Principles:** Modeling spatial shearing setups using an object-side grating and an out-of-focus image-side grating to capture phase derivative fringes.
    *   **Near-Field Non-Periodic Propagation:** Leveraging **SVD-accelerated convolution integrals** instead of standard FFTs to forward-propagate fields in the Fresnel regime past the image-plane grating to the near-field sensor.
    *   **Finite Boundary Analytics:** Accurately simulating the diffraction effects of physical, finite-sized markers and non-periodic structures, eliminating the infinite-grating assumptions and edge artifacts inherent to FFT-based setups.
    *   **Systematic Error Modeling:** A forward perturbation simulator that tracks deviations from ideal interferometric theory—including 2D/3D marker edge imperfections, residual source spatial coherence, laser speckle noise, and spatial cross-talk from unwanted high-order pinhole diffraction.


*   **C. Mathematical Inverse Optimization (OPC / ILT)**
    *   **Inverse Lithography Technology (ILT):** Formulating pixel-based and parametric optimization algorithms to solve for the ideal photomask geometry given a target wafer image, inspired by Boyd’s convex optimization frameworks.
    *   **Sub-Resolution Assist Features (SRAFs):** Rules-based and continuous gradient-descent optimization to position assist features that maximize the overlapping process window.
    *   **Source-Mask Optimization (SMO):** Joint optimization loops that dynamically shift illumination pupils alongside mask shapes to satisfy strict Dose-To-Clear ($D_{tc}$) and Critical Dimension ($CD$) constraints.

### 2. Physics-Inspired AI & Deep Generative Models (`physics-inspired-ai`)
*Bridging classical physics engines with deep neural networks to bypass heavy iterative solvers.*
*   **Sensor to Source Inversion:** Training **Physics-Informed Neural Networks (PINNs)** to ingest raw shearing interferometry sensor measurements and instantly predict underlying system error sources.
*   **Surrogate Modeling:** Leveraging deep generative models (GANs, VAEs, Diffusion) to approximate the Hopkins TCC matrix mapping, reducing forward imaging simulation time by orders of magnitude.
---

## 🛠️ Software Engineering & Advanced Skills

*   **Deep Learning & Core ML:** PyTorch, TensorFlow, Physics-Informed Neural Networks (PINNs), Deep Generative Models (GANs/VAEs/Diffusion), Sequence Modeling.
*   **Scientific Computing & Optimization:** Python (NumPy, SciPy), MATLAB, Convex Optimization (CVXPY / Boyd formulations), Non-linear Gradient Descent.
*   **High-Performance Computing (HPC):** Optimizing matrix operations, parallel computing, GPU acceleration (CuPy/PyTorch CUDA), and algorithmic bottlenecks.
*   **MLOps & Deployment (Expanding):** Scalable model tracking, versioning datasets (DVC), containerization, and clean, modular software packaging (`/src` architecture).

---

## 📈 My Strategic Roadmap
- [ ] **Phase 1:** Finalize core Python modules for Hopkins TCC forward imaging matrices.
- [ ] **Phase 2:** Build the forward mathematical simulation for 2D pinhole shearing interferometry.
- [ ] **Phase 3:** Deploy the Convex Optimization scripts for SRAF mask generation.
- [ ] **Phase 4:** Train and evaluate the PINN surrogate model on wavefront error predictions.

## 📫 Connect with me
*   **LinkedIn:** [Your Link Here]
*   **Email:** [Your Email Here]
<!--
**bogathi-reddy/bogathi-reddy** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
