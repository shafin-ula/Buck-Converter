## Testing 1

### Test Setup and Constraints

#### DC Power Supply
- **Vin:** 5 V  
  - Current limit: 5 mA
- **Vout:** 6 V  
  - Current limit: 5 mA

#### Waveform Generator
- **Signal Type:** PWM (Square Wave)
- **Frequency:** 50 kHz
- **Duty Cycle:** 50%
- **Amplitude:** 5 V peak-to-peak
- **DC Offset:** 2.5 V
- **Voltage Range:** 0 V to 5 V

> **Note:** The PWM signal must strictly swing between 0 V and 5 V.



## Test: Load Test

- Connected **Vout** to a 10 Ω power resistor (10 W, heat-sinked).
- Measured voltage across the **0.5 Ω current sense resistor** and computed current:
  \[
  I = \frac{V_{\text{sense}}}{0.5\ \Omega}
  \]
- Increased **Vin** up to **16 V** and observed changes in output voltage and current.
- **OPAMP_OUT** tracked **Vout**, confirming proper feedback operation.

### Output at Different Switching Frequencies

- **50 kHz**  
  ![50 kHz Test](50kHz%20Test.png)

- **75 kHz**  
  ![75 kHz Test](75kHz%20Test.png)

- **100 kHz**  
  ![100 kHz Test](100kHz%20Test.png)
