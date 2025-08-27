# ICS-43434 Manual Soldering Profile (with MG Chemicals 4902P Low-Temp Paste)

**Date created:** 2025-08-27  
**Author:** [Wang Gucheng]

---

## Paste Information
- **Type:** MG Chemicals 4902P  
- **Alloy:** Sn42Bi57Ag1  
- **Solidus/Liquidus:** ~138 °C  
- **Recommended peak:** 160–170 °C  
- **TAL (time above liquidus):** 45–60 s  
- **Ramp rates:** ≤2 °C/s heating, ≤3 °C/s cooling

---

## Component Information
- **Device:** TDK InvenSense ICS-43434 MEMS microphone  
- **Reflow qualification:** JEDEC J-STD-020  
- **Absolute max peak:** 260 °C (classification only, not target)

---

## Manual Soldering Profile (tested working)

| Stage      | Set Temp (°C) | Time (s) | Notes |
|------------|---------------|----------|-------|
| Preheat    | 120           | 60–75    | Gentle ramp, activate flux |
| Soak       | 140           | 60–75    | Uniform heating, flux fully active |
| Reflow     | 165 (≤170)    | 45–60    | Above 138 °C, ensures full wetting |
| Cooling    | ≤100          | Until RT | Fan cooling, ≤3 °C/s |

---

## Observations
- Joints appear shiny and smooth when peak = **165 °C for ~50 s**.  
- No bridging or voiding observed on 2-layer test PCB.  
- ICS-43434 sensitivity unchanged after reflow.  
- Cooling quickly after reflow prevents Bi joint brittleness.

---

## Practical Tips
- Keep **airflow away from microphone port**.  
- Use **Kapton + thin foil shielding** if nearby hot air is unavoidable.  
- Always allow solder paste to **warm to room temperature** and mix before use.  
- Validate with thermocouple on a scrap PCB for new batches.

---

## Revision History
- **v1.0 (2025-08-27):** Initial profile documented after successful test.
