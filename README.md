# Gaussian-Pulse-Propagation
# Broadening of Gaussian Pulses

## Objective
Compare the results predicted by the linear system model of an optical fiber with the results of simulation.

---

## Theory
An optical fiber can be represented approximately by a linear system with an impulse response \(h(t)\) or a transfer function \(H(j\omega)\).  

If the optical source has a spectral width much greater than the signal bandwidth (e.g., the source is a directly modulated laser diode) and the operating wavelength is far from the zero-dispersion wavelength, then \(H(j\omega)\) is approximately Gaussian:

<img width="1482" height="1120" alt="image" src="https://github.com/user-attachments/assets/83f63473-b1b3-4afc-ad17-9e9850041cae" />


---

### Output Pulse Broadening
If a Gaussian pulse is input to a linear system with a Gaussian impulse response, the output is also Gaussian with RMS width:

<img width="340" height="102" alt="image" src="https://github.com/user-attachments/assets/c60d35c1-8a0f-4c50-873d-1314ec59a29f" />



---

## Calculations
<img width="1076" height="1280" alt="WhatsApp Image 2026-09-03 at 6 55 56 AM" src="https://github.com/user-attachments/assets/8b8a3de9-ba1d-4d8d-8578-4d64e227db6c" />


**Required Calculations:**
<img width="1548" height="298" alt="image" src="https://github.com/user-attachments/assets/b2fb676a-afb0-48ef-914b-309b2ea38a17" />


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
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/7558c0e2-ea83-4eae-a292-829c4b233bab" />


---

## Analysis
Compare the simulation results with the theoretical calculations and discuss any observed differences.


---
 Results to Record
<img width="1448" height="1015" alt="Screenshot 2026-02-05 113211" src="https://github.com/user-attachments/assets/5a7b450e-e6d6-4efc-8c33-791775fdfa8c" />
## Result
The theoretical broadening ratio (
σ
out
/
σ
in
) for a chirped Gaussian pulse over 
50
 km
 of SMF-28 fiber was calculated using the linear system model formulas. The OptiSystem simulation confirmed these analytical results, showing precise agreement between the measured input/output pulse widths and the expected broadening profile influenced by the negative laser chirp factor.



