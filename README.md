# Experiment-1
**Question:** Given that POWER, P=100µW, perform DC Analysis, Transient Analysis, and AC Analysis for the given circuit designs, and observe the effects of width adjustments for each MOSFET.

## Design-1:
   ![Screenshot 2025-02-16 111936](https://github.com/user-attachments/assets/0b661ae7-5761-4b9b-bd75-93c0fc60eabb)

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
![Screenshot 2025-02-16 120802](https://github.com/user-attachments/assets/109d353f-a954-4e08-b8d1-603ea40ea67c)

### 1) DC Analysis:
**Procedure:** Select the DC output print (DC op pnt) in the simulation command editor and run the simulation.
![Screenshot 2025-02-16 121422](https://github.com/user-attachments/assets/8dbd733e-f0a2-4165-8a8e-ebee3b28ace2)

The figure shows the values obtained from DC analysis.
   ![Screenshot 2025-02-16 121045](https://github.com/user-attachments/assets/22bca609-a67e-4459-aa60-e584eb189442)


### 2) Transient Analysis:
**Procedure:** Select transient analysis in the simulation command editor, set the stop time to 1ms, and run the simulation.

The graph illustrates the transient response.

### 3) AC Analysis:
**Procedure:** Choose AC analysis in the simulation command editor, provide the specified values, and run the simulation.
![Screenshot 2025-02-16 122038](https://github.com/user-attachments/assets/e43f0303-c135-4a82-bc71-12e6ae6000b9)

The graph depicts the AC response.
![Screenshot 2025-02-16 122339](https://github.com/user-attachments/assets/87da114b-e8f6-4981-823f-d8a504316454)


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
![Screenshot 2025-02-16 124234](https://github.com/user-attachments/assets/59e297de-ed5d-426c-8e40-92aee8d3e793)

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
![image](https://github.com/user-attachments/assets/b26e13fb-57be-4522-8e21-9b4730448512)


The VTC curve shows Vin at 0.8V in the saturation region.
![Screenshot 2025-02-16 125157](https://github.com/user-attachments/assets/abddb50e-8287-42ad-9dcc-fc4e29b37ff7)

Then the input voltage parameters are given as.

![Screenshot 2025-02-16 125547](https://github.com/user-attachments/assets/f60a3923-74f3-4b7b-8bd2-f000b36797cf)

Length and Width of the Channel of the two MOSFETS used to obtain the given Current is shown in the figure below.

![Screenshot 2025-02-16 125820](https://github.com/user-attachments/assets/2197048a-07ff-4819-ae53-b6f496449d35)
![Screenshot 2025-02-16 125811](https://github.com/user-attachments/assets/a2eae298-1edc-49bc-a925-278ec1eee622)


### 1) DC Analysis:
**Procedure:** Select DC output print (DC op pnt) in the simulation command editor and run the simulation.
![Screenshot 2025-02-16 121422](https://github.com/user-attachments/assets/fe699e4e-be59-4a89-a524-8d88a54555c4)

The diagram below presents the results derived from the DC analysis.
![Screenshot 2025-02-16 125843](https://github.com/user-attachments/assets/dded314a-ede4-45dd-aa51-d8a5251a6ec2)


### 2) Transient Analysis:
**Procedure:** Select transient analysis, set stop time to 1ms, and run the simulation.
 ![Screenshot 2025-02-16 130048](https://github.com/user-attachments/assets/c3faea32-8fd7-4cdb-9d7b-0b454f8d626b)

The below Graph presents the Transient Response for the Given Design.

![Screenshot 2025-02-16 130108](https://github.com/user-attachments/assets/7d25b588-1dd1-406c-98cd-8fa4fc5c6163)

### 3) AC Analysis:
**Procedure:** Choose AC analysis, input the specified values, and run the simulation.
 ![image](https://github.com/user-attachments/assets/80e2d1d3-f2f6-4ce8-b26e-0a803006303a)

 The Graph below shows the AC Analysis of the Given Design;
 ![Screenshot 2025-02-16 130145](https://github.com/user-attachments/assets/e24ddc06-ca3f-41da-b214-6e012222aa04)

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

