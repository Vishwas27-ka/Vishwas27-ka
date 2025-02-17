# Experiment-1
**Question:** Given that POWER, P=100µW, perform DC Analysis, Transient Analysis, and AC Analysis for the given circuit designs, and observe the effects of width adjustments for each MOSFET.

## Design-1:
   **Aim:** Determine the DC operating point, calculate gain through transient analysis, and conduct AC analysis.

   **Components:** MOSFET, resistors, DC power supply.

   **Procedure:**
   - Connect the circuit as shown.
   - Attach RD to the drain and the DC power supply to both the gate and resistor.
   - Ground the source terminal.
   - Set input voltage to 0.9V and VDD to 1.8V.

Using the power formula:  
P = V * I

The drain current (Id) is calculated as:

Id = 5.56 × 10^-5 A

Adjust L and W (MOSFET channel dimensions) to achieve the desired current. The chosen dimensions are displayed in the figure.

### 1) DC Analysis:
**Procedure:** Select the DC output print (DC op pnt) in the simulation command editor and run the simulation.

The figure shows the values obtained from DC analysis.

### 2) Transient Analysis:
**Procedure:** Select transient analysis in the simulation command editor, set the stop time to 1ms, and run the simulation.

The graph illustrates the transient response.

### 3) AC Analysis:
**Procedure:** Choose AC analysis in the simulation command editor, provide the specified values, and run the simulation.

The graph depicts the AC response.

### Result (Design-1):
1. **DC Analysis:**
   - The calculated Id (5.56×10^-5 A) matches the expected value.
   - Adjusting L and W (L=175nm, W=178nm) achieved the required current.
   - Circuit behavior under DC conditions was as anticipated.
2. **Transient Analysis:**
   - The transient response graph shows smooth behavior with no unexpected distortions.
   - The circuit responded well to variations, confirming stability.
3. **AC Analysis:**
   - The AC response graph indicates circuit stability across different frequencies.
   - The observed gain (-9.94 dB) and phase shift (~180°) aligned with theoretical predictions.

### Inference (Design-1):
1. Proper MOSFET dimension selection controls the drain current effectively.
2. **Width Adjustment Impact:**
   - M1 significantly influences Id; wider width increases Id and vice versa.
3. The design performed well in all analyses, demonstrating reliability and feasibility.

---

## Design-2:
**Aim:** Find the DC operating point, calculate gain using transient analysis, and perform AC analysis.

**Components:** MOSFETs (M1 and M2), DC power supply.

**Procedure:**
   - Assemble the circuit as shown.
   - Connect the gate to the DC power supply.
   - Ground the source terminal.
   - Determine VTC and set input voltage to 0.8V with VDD at 1.8V.

Using the formula:  
P = V * I / n

The drain current (Id) is calculated as:

Id = 5.56 × 10^-5 A

Adjust L and W for both MOSFETs to achieve the desired current. The dimensions are displayed in the figure.

**DC Sweep Analysis:** Conduct this analysis to find Vin in the saturation range by selecting DC Sweep in the simulation command editor and running the simulation.

The VTC curve shows Vin at 0.8V in the saturation region.

### 1) DC Analysis:
**Procedure:** Select DC output print (DC op pnt) in the simulation command editor and run the simulation.

### 2) Transient Analysis:
**Procedure:** Select transient analysis, set stop time to 1ms, and run the simulation.

### 3) AC Analysis:
**Procedure:** Choose AC analysis, input the specified values, and run the simulation.

### Result (Design-2):
1. **DC Analysis:**
   - Calculated Id (5.56×10^-5 A) matched the expected value.
   - Adjusted dimensions achieved the desired current:
     - M1: L=500nm, W=950nm.
     - M2: L=300nm, W=1020nm.
2. **Transient Analysis:**
   - The transient graph confirmed smooth transitions.
   - The circuit responded well to input variations, indicating stability.
3. **AC Analysis:**
   - The AC graph confirmed stability over various frequencies.
   - Gain (3.8 dB) and phase shift (~180°) aligned with expectations.

### Inference (Design-2):
1. Correct MOSFET dimension selection controls drain current effectively.
2. The VTC curve helped select the appropriate saturation voltage (0.8V).
3. **Width Adjustment Impact:**
   - M2 had a significant influence on Id; wider width increased Id notably.
   - M1 had a smaller effect; changes in width caused minor Id variations.
4. The design met performance expectations, demonstrating practical feasibility.

