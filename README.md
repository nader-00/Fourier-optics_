# Fourier Optics (SLM Lab)

University lab project exploring Fourier optics with a phase-mostly Spatial Light Modulator (SLM) at λ = 532 nm. The repo contains code and results for (i) characterising the SLM, (ii) imaging and filtering in the Fourier plane with a 4-f system, and (iii) computer-generated holography via the Gerchberg–Saxton algorithm.

## What’s here
- **Notebook:** `Fourier_Optics_Algherbawi.ipynb` – end-to-end workflow:
  - Pixel-pitch measurement of the SLM from grating diffraction.
  - Amplitude/gray-level modulation curve acquisition and fit.
  - Imaging the SLM plane and locating the focal plane via the thin-lens equation.
  - Optical Fourier transforms of test images and **FFT** (fft2/fftshift) comparisons.
  - Fourier-plane filtering (circular low/high-pass, vertical slit) and image reconstruction.
  - Phase-only **Gerchberg–Saxton** hologram synthesis with iteration/error plots.
- **Data/Results:** sample images and saved figures from the lab sessions.

## Key experimental results
- **SLM pixel pitch:** \( p = 33.56 \pm 0.65 \,\mu\text{m} \) (first-order diffraction fit).  
- **Laser:** \( \lambda = 532 \,\text{nm} \).  
- **Imaging check:** measured effective focal length from bench geometry ≈ **71.05 ± 0.31 mm** (vs. nominal 100 mm).  
- **Filtering intuition:** high-pass → edges enhanced; low-pass → blurred global structure; vertical slit → suppresses horizontal detail.  
- **Holography:** Gerchberg–Saxton iterations reduce amplitude error and sharpen reconstructions (e.g., 10 → 50 iters).

## References
- B. E. A. Saleh & M. C. Teich, *Fundamentals of Photonics*.  
- J. Goodman, *Introduction to Fourier Optics*.  
- Lab manual: Fourier Optics & Spatial Light Modulator course (SLM setup, tasks, 4-f filtering, and holography).
