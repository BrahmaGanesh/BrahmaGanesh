# Brahma Ganesh Katrapalli
**Entry-Level ASIC Design Verification Engineer**  
[LinkedIn](https://www.linkedin.com/in/katrapallibrahmaganesh) | [GitHub](https://github.com/BrahmaGanesh) | [Email](mailto:brahmaganeshkatrapalli@gmail.com)

---

## Professional Summary

Entry-Level ASIC Design Verification Engineer with hands-on experience building UVM-based testbenches, writing SystemVerilog Assertions, and closing functional coverage for industry-standard protocols. Experienced in debugging simulation failures, analyzing waveforms, and tracing issues to root RTL or testbench causes. Focused on building reliable, self-checking verification environments rather than just passing tests.

---

## 🛠️ Verification Mindset

I approach verification with a structured, reliability-first methodology:
*   **Verification Planning:** Start with the specification to derive features, corner cases, and assertions before writing code.
*   **Stimulus Strategy:** Build constrained-random sequences to hit edge cases that directed tests miss.
*   **Measuring Progress:** Use functional coverage and code coverage to objectively measure verification completeness.
*   **Debugging:** Systematic root-cause analysis using waveforms, logs, and transaction-level traces.

---

## 💻 Technical Skills

| Category | Skills |
| :--- | :--- |
| **Verification** | UVM, SystemVerilog, SVA (Assertions), Functional Coverage, Constrained Random Verification (CRV) |
| **Hands-on Protocols** | **APB**, **SPI** (End-to-end verification with UVM) |
| **Working Knowledge** | UART, I2C, Digital Logic, FSM Design |
| **Tools & OS** | QuestaSim, Vivado, Python (Automation), Linux, Git |

---
## 🧪 Verification Deliverables I Can Own

I take ownership of the following verification responsibilities:

* **Verification Planning:** Deriving a complete verification plan directly from protocol specifications.
* **UVM Testbench Development:** Building reusable UVM agents (driver, monitor, sequencer) and environment components.
* **Checking & Modeling:** Implementing self-checking scoreboards and reference models.
* **Assertions:** Writing concurrent SystemVerilog Assertions to enforce protocol timing and data integrity.
* **Functional Coverage:** Defining covergroups and driving coverage closure based on verification goals.
* **Debugging:** Isolating and resolving failures across RTL, testbench, and stimulus layers using waveforms and logs.

## 📂 Key Verification Projects

### 1️⃣ [APB Protocol Verification (UVM)](https://github.com/BrahmaGanesh/APB-Protocol-Design-UVM-Verification.git)
**Role:** Designed the complete verification environment for an AMBA APB Slave DUT.

*   **Verification Plan:**
    *   Targeted Setup/Access phase timing adherence.
    *   Verified randomized wait-states (PREADY low) and error responses (PSLVERR).
    *   Validated back-to-back transfers without idle cycles.
*   **Testbench Architecture:**
    *   **Scoreboard:** Implemented an associative array-based reference model to predict expected read data and compare against DUT output.
    *   **Coverage:** Defined covergroups for Address ranges, Read/Write distribution, and PREADY delays.
*   **Real Bugs Caught & Resolved:**
    *   **Timing Violation:** Detected a protocol violation where `PENABLE` was asserted before `PSEL` setup time requirements were met using concurrent SVA bound to the interface.
    *   **Data Integrity:** Fixed a scoreboard mismatch caused by incorrect data sampling during extended wait-states (PREADY=0).

### 2️⃣ [SPI Master/Slave Verification (SystemVerilog/UVM)](https://github.com/BrahmaGanesh/spi-protocol-verification-uvm.git)
**Role:** Verified a configurable SPI controller supporting all 4 CPOL/CPHA modes.

*   **Focus Areas:**
    *   Verified correct data sampling edges for all CPOL/CPHA mode combinations.
    *   Validated `CS_N` (Chip Select) assertion timing and setup/hold requirements.
    *   Tested asynchronous reset behavior during active transfers.
*   **Challenges Solved:**
    *   **Mode Mismatch:** Debugged and resolved a data shift issue in Mode 3 (CPOL=1, CPHA=1) where the MSB was being driven one cycle late.
    *   **Corner Case:** Verified system behavior when back-to-back transfers occurred with minimal inter-frame delay.

---

## 🎓 Education & Training

**ASIC Design Verification Training** | ChipEdge Technologies  
*Completed intensive hands-on ASIC Verification training with multiple UVM projects.*  
*   Focus: SystemVerilog, UVM, Protocol Verification, and Linux environment.

**B.Tech in Electronics & Communication Engineering**  
*Graduated 2025*

---
