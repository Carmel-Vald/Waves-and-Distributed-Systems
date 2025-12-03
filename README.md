# Waves-and-Distributed-Systems
mplementing numerical simulations of pulse propagation in dispersive media, multi-layer optical coatings, quarter-wave anti-reflection layers, and distributed Bragg reflectors (DBR).


##  Contents

### 1. Pulse Propagation in Dispersive Media
Simulation of a Gaussian-modulated pulse propagating through different refractive-index profiles:

- **Constant refractive index (no dispersion)**  
  The pulse shifts in time without distortion.

- **Linear dispersion**  
  Shows amplitude reduction and envelope broadening due to frequency-dependent phase velocity.

- **Quadratic dispersion**  
  Produces severe pulse distortion, asymmetry, spreading, and non-constant group velocity.

Includes:
- Time-domain pulse plots at multiple propagation distances  
- Fourier spectrum using `fft` and `fftshift`  
- Superposition plots showing deformation growth  
- Interpretation of the physical behavior in each case

---

### 2. Quarter-Wave Anti-Reflection Coating (λ/4 Layer)
A full transfer-matrix analysis of a single-layer coating intended to minimize reflections:

- Derivation of reflection & transmission coefficients using boundary conditions  
- Finding refractive index \( n_2 \) and thickness \( h \) for zero reflection  
- Numerical solution for:
  - Air → Glass interface  
  - \( n_1 = 1 \), \( n_3 = 1.45 \)  
  - Center wavelength \( \lambda_0 = 1.55 \mu m \)

Includes graphs of:
- Reflection vs wavelength  
- Reflection vs incident angle  
- Odd-multiple thickness behavior and spectral shifts  

All handwritten derivations are included as scanned pages.

---

### 3. Distributed Bragg Reflector (DBR)
Design and simulation of multilayer Bragg mirrors consisting of alternating λ/4 layers:

- Transfer matrix for one DBR period  
- Amplitude reflection and transmission coefficients  
- DBR design for two refractive index contrast cases:
  - \( n_H / n_L = 1.01 \)
  - \( n_H / n_L = 1.1 \)

Simulations include:
- Reflectivity vs wavelength  
- Optical phase response (unwrapped phase)  
- Effect of oblique incidence (e.g., 5° tilt) on the reflective spectrum  
- Determination of number of required periods for >99% reflection

---

### 4. Handwritten Derivations
The repository includes scanned handwritten pages containing:

- Full optical transfer-matrix expansions  
- Boundary-condition derivations  
- Thickness and refractive-index solutions  
- DBR resonance and phase behavior derivations  

These support and validate the numerical MATLAB results.

---

##  Tools & Technologies
- MATLAB  
- Transfer Matrix Method (TMM)  
- Fourier-domain signal analysis  
- Numerical optical simulation  

### Quick Access
[ Open main.m](main.m)
