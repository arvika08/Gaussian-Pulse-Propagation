# Gaussian-Pulse-Propagation
# Broadening of Gaussian Pulses

## Objective
Compare the results predicted by the linear system model of an optical fiber with the results of simulation.

---

## Theory
An optical fiber can be represented approximately by a linear system with an impulse response \(h(t)\) or a transfer function \(H(j\omega)\).  

If the optical source has a spectral width much greater than the signal bandwidth (e.g., the source is a directly modulated laser diode) and the operating wavelength is far from the zero-dispersion wavelength, then \(H(j\omega)\) is approximately Gaussian:

<p align="center">
  <img src="https://github.com/user-attachments/assets/83f63473-b1b3-4afc-ad17-9e9850041cae" width="650">
</p>


---

### Output Pulse Broadening
If a Gaussian pulse is input to a linear system with a Gaussian impulse response, the output is also Gaussian with RMS width:

<p align="center">
  <img src="https://github.com/user-attachments/assets/c60d35c1-8a0f-4c50-873d-1314ec59a29f" width="220">
</p>


---

## Calculations
**System Parameters:**

| Component | Parameter | Value |
|-----------|-----------|-------|
| Transmitter – Gaussian Pulse Generator | Operating wavelength | 1550 nm |
| | Bit rate | 2.5 Gb/s |
| | FWHM pulse width | 0.5 bit period |
| | Chirp factor | -6 |
| Fiber | Type | Corning SMF-28 |
| | Length | 50 km |

**Required Calculations:**
<p align="center">
  <img src="https://github.com/user-attachments/assets/b2fb676a-afb0-48ef-914b-309b2ea38a17" width="750">
</p>


## Layout
Place and connect the following components:
1. **User-defined bit sequence generator** – set to generate a single pulse of the specified width  
2. **Optical Gaussian pulse generator** – enter the chirp factor as a negative number  
3. **Optical fiber** – set according to specifications  
4. **Optical spectrum analyzers** and **optical time domain visualizers** at input and output of fiber  

---

## Simulation
- Set the parameters and run the simulation.  
- Use the visualizer displays to measure:  
  - FWHM width of input and output pulses  
  - FWHM width of optical spectra  

---

## Analysis
Compare the simulation results with the theoretical calculations and discuss any observed differences.
<p align="center">
  <img src="https://github.com/user-attachments/assets/34be1011-de30-4a23-96e5-2de158a9dc23" width="320">
  <img src="https://github.com/user-attachments/assets/86d979e1-0409-48ef-8f53-8b3bfa47dd21" width="420">
</p>




---
 ## Results to Record
<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/5a7b450e-e6d6-4efc-8c33-791775fdfa8c"
    width="700"
  >
</p>



