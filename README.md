# Boardoza TPP60308 60V Buck Breakout Board

The **Boardoza TPP60308 Buck Breakout Board** is a **step-down DC-DC converter** board based on the TPP60308 regulator IC. Designed for efficient power conversion, the board supports pulse-skipping operation for improved efficiency at light loads and provides flexible switching-frequency control. It also includes useful power-management features such as soft-start and protection against overcurrent and excessive temperature.

The board operates from a wide 5V - 60V input range and provides a regulated 5V output with 3A continuous output current, supporting loads up to 3.5A. Its **RT/CLK (Resistor-Timing / Clock) pin allows the switching frequency to be adjusted** from 100kHz to 2.5MHz using an external resistor. The same pin can also receive an external clock signal, allowing the converter to synchronize its switching frequency using its **integrated PLL (Phase-Locked Loop)**. These capabilities make the board suitable for **embedded systems, industrial power conversion, control electronics, and applications requiring a stable 5V supply from 60V DC sources**.


|Front Side|Back Side|
|:---:|:---:|
|![Front](./assets/TPP60308%20Front.png)|![Back](./assets/TPP60308%20Back.png)|

---

## Key Features

- **Wide-Input Buck Conversion:** Converts 60V DC supplies to a regulated 5V output for embedded and industrial electronics.
- **Light-Load Efficiency:** Pulse-skipping operation reduces switching losses when the connected load requires little power.
- **Flexible Frequency Control:** Adjustable switching frequency enables designs to balance efficiency, component size, and electromagnetic interference.
- **External Clock Synchronization:** Integrated PLL allows the converter switching frequency to synchronize with an external clock source.
- **Integrated Protection:** Thermal shutdown, overcurrent protection, and undervoltage lockout (UVLO) help protect the converter during abnormal operating conditions.
- **Controlled Power-Up:** Adjustable soft-start helps reduce inrush current during converter startup.

---

## Technical Specifications

**Model:** TPP60308   
**Manufacturer:** Boardoza  
**Manufacturer IC:** 3PEAK  
**Input Voltage:** 5V - 60V  
**Functions:** Step-Down DC-DC Voltage Conversion  
**Output Voltage:** 5V  
**Continuous Output Current:** 3A  
**Maximum IC Output Current:** 3.5A  
**Switching Frequency:** 100kHz - 2.5MHz  
**External Clock Frequency:** 160kHz - 2.3MHz  
**Internal Voltage Reference:** 0.8V, 1.5%  
**Operating Quiescent Current:** 160µA  
**Shutdown Current:** 2.25µA  
**Operating Temperature:** -40°C to +125°C  
**Board Dimensions:** 60mm x 20mm

---

## Board Pinout

### ( J1 ) Power and Converter Control Pins

| Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | VCC | Power Supply Input (5V - 60V) |
| 2 | EN | Active-High Device Enable Pin with Internal Pull-Up Current Source |
| 3 | CLK | RT/CLK Frequency-Setting and External Clock Synchronization Input |
| 4 | GND | Ground |

### ( J2 ) Regulated Power Output

| Pin Number | Pin Name | Description |
| :---: | :---: | --- |
| 1 | VOUT | Regulated 5V DC Output |
| 2 | GND | Ground |

>Note: The RT/CLK pin can be used in two ways. An external resistor can set the switching frequency from 100kHz to 2.5MHz, or an external clock signal can synchronize the converter through its integrated PLL (Phase-Locked Loop). For external clock synchronization, the supported input frequency is 160kHz - 2.3MHz, with HIGH > 2V, LOW < 0.5V, and a minimum pulse width of 15ns.

---

## Board Dimensions

<img src="./assets/TPP60308 Dimensions.png" alt="TPP60308 Dimension" width="450"/>

---

## Step Files

[Boardoza TPP60308.step](./assets/TPP60308%20Step.step)

---

## Sensor Datasheet

[TPP60308 Datasheet.pdf](./assets/TPP60308%20Datasheet.pdf)

---

## Version History

- V1.0.0 - Initial Release

---

## Support

- If you have any questions or need support, please contact <support@boardoza.com>

---

## **License**
### **Hardware Design**

[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

All hardware design files are licensed under [Creative Commons Attribution-ShareAlike 4.0 International License][cc-by-sa].

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg
