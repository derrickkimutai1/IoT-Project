# Embedded Systems & IoT
## Prototypes of Embedded Devices
**Group 10**

---

## 1. Group Members


| Name | Student ID | Role in this Deliverable |
|---|---|---|
| Jesse Richard and Ryan Arkadie | 159287, 168052| Physical prototype (a), wiring & testing |
| Derrick Kibet and Emmanuel Ochieng | 169651, 169765 | Physical prototype (b), documentation |
| Joe Karogo and Matthew Wachira | 167141, 151733 | Wokwi simulations (a) and (c) |
| Jarvis Getenga | 169888 | Sensor calibration, IDE output capture |

**Evidence of groupwork:**

![Group photo](media/group_photo.jpeg)


---

## 2. Overview of Architectures

Per the Deliverable 2 brief, our group produced the required minimum of 4 prototypes:

| Architecture | Description | Prototype Type |
|---|---|---|
| (a) | ESP32 + MQ-5 + DHT22 + LCD | **Physical** and **Simulated** (both required) |
| (b) | ESP32 (MQ-5) ↔ ESP32 (DHT22), interfaced directly | **Physical** |
| (c) | ESP32 (DHT22) → Relay → ESP32 (MQ-5) | **Simulated** |

(b) and (c) are interchangeable per the brief; our group built (b) physically and (c) as a simulation.

---

## 3. Architecture (a): ESP32 + MQ-5 + DHT22 + LCD

### 3.1 Physical Prototype

![Physical prototype (a)](media/4aphysical%201.jpeg)
![Physical prototype (a) - alternate angle](media/4aphysical%202.jpeg)

**IDE Output:**

![IDE output (a)](media/4aIDE%20simulated.jpeg)


### 3.2 Simulated Prototype

**Wokwi Project Link:** [https://wokwi.com/projects/467286122843350017](https://wokwi.com/projects/467286122843350017)


![Simulated prototype (a)](media/4a%20Wokwi%20simulated.png)

---

## 4. Architecture (b): ESP32 (MQ-5) ↔ ESP32 (DHT22)

### 4.1 Physical Prototype


![Physical prototype (b)](media/4bphysical%201.jpeg)
![Physical prototype (b) - alternate angle](media/4bphysical%202.jpeg)

**IDE Output:**

![IDE output (b)](media/4bIDE%20simulated.jpeg)

---

## 5. Architecture (c): ESP32 (DHT22) → Relay → ESP32 (MQ-5)

### 5.1 Simulated Prototype

**Wokwi Project Link:** [https://wokwi.com/projects/467156925257896961](https://wokwi.com/projects/467156925257896961)


![Simulated prototype (c)](media/4c%20Wokwi%20simulated.png)



---

## 6. Issues Encountered and Resolutions

- **Problem:** The LCD module for architecture (a) did not display any output during physical testing.
- **Solutions explored:** Wiring connections were checked and re-checked. Two likely causes were identified:
Insufficient voltage being delivered to the LCD, or
Complete failure of the LCD module itself
Given the time available before submission, we were unable to conclusively isolate and fix the root cause.
- **Recommendation / resolution:** Despite the LCD issue, the IDE serial monitor produced correct, meaningful output — confirming that the underlying program logic (sensor reads, data formatting, thresholds) was working as intended. This strongly suggests the fault is isolated to the hardware/display layer rather than the code.

---

## 7. Repository Structure

```
/Iot-markdown
│
├── DELIVERABLE2.md           # this document
├── media/                    # all images referenced above
│   ├── 4a Wokwi simulated.png
│   ├── 4aIDE simulated.jpeg
│   ├── 4aphysical 1.jpeg
│   ├── 4aphysical 2.jpeg
│   ├── 4bIDE simulated.jpeg
│   ├── 4bphysical 1.jpeg
│   ├── 4bphysical 2.jpeg
│   └── 4c Wokwi simulated.png

```