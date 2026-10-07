# undervolts

***this hosts my personal CPU (7700x) & GPU (6950XT) undervolts. 
settings & results may vary depending on several factors,
as well as your BIOS depending on manufacturer***
> [!WARNING]
> i am **NOT** responsible for any crashes, failures, or any harm caused to your components. follow at your own discretion

**sections**
- ***1. CPU limits & curve optimizer***
- ***2. GPU (windows, adrenalin software)***
- ***3. GPU (arch, LACT)***
## 📊 CPU (limits, curves)
|option|value|
|-|-|
|PPT Limit [mW]|125000|
|TDC Limit [mA]|90000|
|EDC Limit [mA]|150000|
|Max CPU Boost Clock Override (+)|25|

### **curve optimizer**
**all cores**
|option|modifier|value|
|-|-|-|
|Cores 0-1|Negative|5|
|Cores 2-7|Negative|11|


## ⚡ GPU (windows, arch linux)  
### 🪟 **AMD adrenalin**
**GPU tuning**
|option|value|
|-|-|
|Min Freq. (MHz)|1500MHz|
|Max Freq. (MHz)|2300MHz|
|Voltage (mV)|1100mV|
<img width="583" height="310" alt="gputuning" src="https://github.com/user-attachments/assets/594038e4-4e7a-4127-ae84-f8cd44fd03d6" />


**VRAM tuning**
|option|value|
|-|-|
|Memory Timing|Fast Timing|
|Max Freq. (MHz)|2300MHz|
<img width="585" height="206" alt="vramtuning" src="https://github.com/user-attachments/assets/10126822-68f9-48b4-87cf-f748e70b654a" />


**Fan Tuning**
|option|value|
|-|-|
|Zero RPM|Disabled <sup>(see: *1, *2)</sup>|
|Max Fan Speed|65-70%|

<sup>***1 customize this to your case, I own an SFF (meshroom S) build. I like to balance between temps and noise**</sup>  
<sup>***2 zero RPM mode is generally not advised in areas where the temperature causes the gpu temps to rise back to the zero RPM threshold, this can cause motor degradation due to constant spin-ups**</sup>

**Power Tuning**
|option|value|
|-|-|
|Power Limit|-5%|
<img width="586" height="152" alt="powertuning" src="https://github.com/user-attachments/assets/9a40b8cc-139f-4344-ad71-51e8af0d31c4" />


---

### 🐧 **LACT (EXPERIMENTAL)**
<sup>**please note, this undervolt is still being EXPERIMENTed on, may not be the final product and may not be stable**</sup>
**Power Usage Limit**
|option|value|
|-|-|
|Power Usage Limit|275W/346W|
<img width="533" height="68" alt="image" src="https://github.com/user-attachments/assets/f59b3004-d1d8-4e80-9315-fd4b7aff5a75" />

**Clockspeed and Voltage**
|option|value|
|-|-|
|Max. GPU Clock (MHz)|2550MHz|
|Min. GPU Clock (MHz)|1450MHz|
|Max. VRAM Clock (MHz)|2350MHz|
|Min. VRAM Clock (MHz)|1348MHz|
|GPU voltage offset (mV)|-80|
<img width="533" height="156" alt="image" src="https://github.com/user-attachments/assets/aee24060-6051-4f62-9eb2-1b74adebac19" />  

---

**build used**
|category|model|
|-|-|
|MB|ASRock B650I Lightning WiFi|
|CPU|AMD Ryzen 7 7700x|
|COOLER|be quiet! Pure Loop 3 (240mm)|
|GPU|AMD Radeon RX 6950 XT Phantom Gaming 16GB OC|
|RAM|Kingston FURY Beast 32GB (2x16GB) DDR5 6000MHz|
|PSU|Corsair RM750x (2018)|
|CASE|SSUPD Meshroom S (v1)|

**tested on**  
*- Wingoys 11 (25H2)*  
*- Arch Linux (CachyOS)*  
