---
marp: true
theme: uncover
_class: invert
---
Working with the
# **Caravel Harness**
Cole Blackman, Justin Zhang
*ECE HPLP Lab UVA 2021*

![w:500px](caravel.svg)

---

# **Table of Contents**

### 1. Caravel 
### 2. Openlane (hardening process)
### 3. Caravel I/O
### 4. Future work (SHA256) 

---

# Background: Skywater PDK and Sky130 process node

- Open source toolset
- Google and Skywater
- Design fabrication processes and ICs
- WIP (not supported in production yet/alpha)
- https://skywater-pdk.readthedocs.io/en/latest/

---

# Background: OpenLane Flow

- Complete process for building GDSII database files (IC layouts)
- 
---

![w:900px](openlane.png)

---

# Background: Efabless Open MPW Shuttle Program

- Fabricates your Skywater PDK 130nm process design using Openlane for free

---

# **Caravel**

- Test harness for Skywater 130nm OS PDK
- RISC-V RV32IMC IS running on PicoRV32 processor core
- **Provides a test "harness" of tools like SRAM and GP I/O for open user area circuits** 

---


# Components of Caravel

**What does caravel provide the developer?**

- Wishbone (32-bit)
- 128-bit logic analyzer
- UART
- SPI controller and SPI flash controller
- Large SRAM
- I/O
- And more...

--- 

![w:900px](caravel.svg)

---

# **Our Work**

- Compiled documentation
- Wrote ECE Wiki pages
- Adapted SHA-3 for MPW Shuttle 2.0 and wrote SHA-3 documentation
- Wrote and hardened johnson counter within Openlane/Caravel harness (doesn't use I/O)  
- Wrote Verilog tutorial
- Adapted SHA-3 algorithm for a smaller die size


---

# **Our Future Work**

- Implementation of SHA-2 (256) hashing algorithm in a custom user area ASIC ontop of the Caravel Harness (Bitcoin/Crypto mining applications)
- Entrance into IEEE SSCS design contest

---

# **Key Takeaways**

- Skywater 130 PDK - maturing
- Caravel test harness - good for small applications and education
- 

