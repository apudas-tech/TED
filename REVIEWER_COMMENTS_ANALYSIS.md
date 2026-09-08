# IEEE TED Reviewer 2 - Detailed Comments & Response Plan

## Manuscript Title
Sign Reversal of the DC-Sweep Capacitance–Voltage Hysteresis Window in Hf₀.₅Zr₀.₅O₂ Ferroelectric Transistors

**Review Status:** Major Revision Required

---

## COMMENT 1: Relationship to Published Work & Novelty
**Severity:** CRITICAL

### Reviewer Points:
- Two recent papers by authors overlap substantially:
  1. "Endurance Paradox in Hafnium-Oxide-Based Silicon-Channel Ferroelectric Transistors" (ACS Appl. Mater. Interfaces, 2026)
  2. "Quantifying Endurance-Driven Loss of Polarization-to-Channel Charge Coupling" (ACS Appl. Electron. Mater., 2026)
  
- These papers report:
  - Ferroelectric polarization remains intact after memory window collapse
  - Polarization-to-channel coupling factor concept
  - Window closure attributed to trap-assisted screening

### Reviewer Request:
1. Clearly cite both papers
2. Distinguish present work by:
   - Device structure differences
   - Wafer batch/cycling conditions
   - Raw data differences
   - Analysis metrics differences
   - Scientific conclusions
3. Identify which results are novel (vs. previously published)

### Key Statement from Reviewer:
> "The novelty of this manuscript should be clearly distinguished from these published studies and, if supported, **limited to the sign reversal of the DC-sweep C-V hysteresis and its frequency- and conductance-dependent characteristics.**"

### Required Actions:
- [ ] Add/update citations for both ACS papers
- [ ] Create comparison table: Present work vs. prior work
- [ ] Clearly highlight novel findings:
  - **Sign reversal** (not just closure) of hysteresis window
  - **Frequency independence** (1 kHz - 1 MHz)
  - **Amplitude independence** (±1.5V to ±3V)
  - **Conductance-dependent characteristics**
  - **Transistor-level confirmation** at multiple extraction criteria
- [ ] Add explicit statement: "Results presented here that differ from prior publications..."

---

## COMMENT 2: Physical Meaning of C-V Window & Memory Claims
**Severity:** HIGH

### Reviewer Points:
- Authors state C-V sweep takes ~1 second
- Pulse-written state does NOT survive the sweep
- Forward/reverse curves overlap after program/erase
- Therefore: **DC-sweep hysteresis ≠ retained memory window**

### Problematic Statements:
- "the device has ceased to store information"
- "endurance failure"
- "the device does not simply lose its memory: it inverts it"

### Physical Reality:
- These statements imply transistor-level memory retention
- But C-V measurement is taken after state has relaxed
- This is DC-sweep hysteresis, not memory-state measurement

### Required Actions:
- [ ] Remove or heavily revise all statements claiming memory loss/inversion
- [ ] Clearly distinguish:
  - **DC-sweep C-V hysteresis** (what is actually measured)
  - **Pulse-written transistor state** (what is claimed to be stored)
- [ ] Note: Transfer characteristics DO show sign reversal at device level (Section III-E)
  - This validates the device-level interpretation
  - But must be clearly separated from C-V interpretation
- [ ] Revise abstract, introduction, and conclusion to reflect this distinction

---

## COMMENT 3: Reliability of Sign Reversal at 10⁴ Cycles
**Severity:** CRITICAL - Measurement Artifact Concern

### Reviewer's Core Concern:
The most important negative window is at 10⁴ cycles, but:
- Lumped Cₚ-Rₚ model is **invalid** at this checkpoint
- Of 57 excluded sweeps (D ≥ 0.9), **38 are from 10⁴ cycles**
- High-loss conditions may cause:
  - Leakage current effects
  - Series resistance distortion
  - Nonequilibrium charging/discharging
  - Measurement model limitations

### Author's Own Acknowledgment (from manuscript):
> "the lumped Cₚ-Rₚ model is no longer valid at this checkpoint, and we restrict the claim accordingly"

### Critical Data Missing:
- Loss tangent (D) distribution at 10⁴ cycles
- Number of valid sweeps per frequency/amplitude
- Unfiltered raw data (uncorrected Cₚ data)

### Author's Defense (Partial):
- Uncorrected Cₚ data shows sign reversal: 25 of 27 sweeps negative (Section III-C)
- Multiple frequencies/amplitudes show reversal
- Transfer characteristics confirm reversal

### Required Actions:
- [ ] **MOST IMPORTANT:** Provide complete Table showing for 10⁴ cycles:
  | Frequency | Amplitude | Valid Sweeps | Failed Sweeps | D (min/max) | Corrected ΔVh | Uncorrected Cₚ ΔVh |
  
- [ ] Expand Section III-C (Artifact Testing):
  - Provide full breakdown of the 25/27 uncorrected sweeps
  - Report D values for all sweeps at 10⁴ cycles
  - Show frequency/amplitude combinations with data
  
- [ ] Address mechanism: If Cₚ-Rₚ model fails, what is physical interpretation?
  - Is uncorrected Cₚ reliable under high-loss conditions?
  - What is the physical meaning of ΔVh when correction is ill-conditioned?

- [ ] Consider alternative explanations:
  - Frequency-dependent trap response
  - Nonequilibrium effects at high losses

---

## COMMENT 4: Device-to-Device Reproducibility
**Severity:** HIGH - Statistical/Claims Issue

### Reviewer Points:
- **All results from single device** (device-1 for C-V details)
- Different frequencies/amplitudes ≠ device-to-device reproducibility
- Uncertainty bars misleading:
  - Derived from different measurement conditions
  - NOT from independent devices or repeated measurements
  - Gives false impression of statistical significance

### Problematic Claim:
> "window is negative by 4.6 sigma"
- This implies statistical significance across multiple devices
- But all from one device at different conditions
- Misrepresents reliability

### Partial Redemption:
Figure 4 DOES show five devices with reproducible sign reversal:
- Device-1: crosses zero at 503 cycles
- Device-2: 871 cycles
- Device-3: 1117 cycles
- Device-6: 2136 cycles
- Device-7: 2422 cycles
- All show negative window at 10⁴ cycles

### Required Actions:
- [ ] **CRITICAL REVISION of statistical claims**
  - Remove "4.6 sigma" statement or clarify its meaning
  - Replace with: "All five independent devices show sign reversal by 10⁴ cycles"
  
- [ ] Clarify error bars in Figure 4:
  - Add caption explaining: "Error bars represent spread across different frequencies/amplitudes, not device-to-device variation"
  - Or convert to device-to-device representation
  
- [ ] Provide for Figure 4 devices (at 10⁴ cycles):
  - Mean and std. dev. of ΔVh across measurement conditions
  - Verification that sign reversal is consistent (not frequency/amplitude dependent)
  
- [ ] Table 1 revision:
  - Show data for all five devices at multiple conditions
  - Or clearly state that only device-1 was measured at multiple frequencies/amplitudes
  
- [ ] Revise manuscript language:
  - "Five independent devices reproducibly show sign reversal" ✓
  - "Reversal is frequency- and amplitude-independent" (for each device) ✓
  - "Window is statistically significant at 4.6σ" ✗ (remove or clarify)

---

## COMMENT 5: Capacitance Validity Range vs. Sign Reversal Claim
**Severity:** HIGH - Internal Contradiction

### The Problem:
Authors present three simultaneous observations at 10⁴ cycles:
1. Preserved polarization (PUND measurement)
2. Unchanged gate-stack capacitance
3. Hysteresis sign reversal

**BUT:** Capacitance constancy is only validated through 10³ cycles!

### Author's Own Statement:
> "a physically meaningful corrected capacitance is obtained through 10³ cycles on device-1 and through 10² on device-2, **while at 10⁴ cycles ωRₛC ≈ 0.50 and the correction is ill-conditioned. No corrected value is quoted there**"

### Logical Consequence:
Cannot simultaneously claim:
1. Capacitance unchanged (only proven to 10³)
2. Hysteresis reversal (occurs at 10⁴)
3. Both support charge-screening model (requires both to be true)

### Required Actions:
- [ ] Revise all claims about "unchanged capacitance":
  - Current: "series-resistance-corrected accumulation capacitance is unchanged" at 10⁴ cycles ✗
  - Revised: "series-resistance-corrected accumulation capacitance is unchanged through 10³ cycles; at 10⁴ cycles the correction is ill-conditioned and no corrected value is reported"
  
- [ ] In Interpretation section (III-F):
  - Remove assumption that capacitance is constant at 10⁴ cycles
  - Explain how charge-screening model still accounts for observations **without this assumption**
  - OR use alternative evidence (e.g., uncorrected Cₚ, conductance trends)

- [ ] In Figure 7 caption and text:
  - Clarify that capacitance validation extends only to 10³ cycles
  - Explain why polarization + reversal still support screening model without capacitance data

- [ ] Add new analysis:
  - Can sign reversal + preserved polarization alone (without capacitance) support screening?
  - What additional information would pin down the mechanism at 10⁴ cycles?

---

## COMMENT 6: Ambiguous Charge Location & Over-Interpretation
**Severity:** MEDIUM - Interpretation Overreach

### Reviewer Points:
Results do NOT uniquely identify charge location. Possibilities:
- Bulk HZO
- HZO/SiO₂ interface
- Within SiO₂
- SiO₂/Si interface

### Observations Cannot Resolve:
- Conductance increase
- Imprint shift
- C-V flank asymmetry

### Problematic Statements in Manuscript:
- "Only one class of explanation survives"
- "all point to the same interfacial region"
- "interface engineering rather than ferroelectric engineering"

### Physical Reality:
- Observations are **consistent with** interfacial charge
- They do NOT **prove** interfacial origin

### Required Actions:
- [ ] Revise Interpretation (Section III-F) language:
  
  **Current language (too definitive):**
  - "Only one class of explanation survives"
  - "Interface engineering"
  
  **Revised language (appropriate uncertainty):**
  - "Interfacial charge provides a consistent account" 
  - "An interfacial charge model could account for both observations, though charge location (bulk vs. interface) remains to be determined"
  - "These results motivate interface engineering approaches, though bulk effects cannot be excluded"

- [ ] Add to Limitations section:
  - Charge location (bulk HZO vs. interfacial) cannot be resolved
  - Transmission electron microscopy or charge pumping would be needed
  - Alternative interpretations (e.g., bulk trap response) not ruled out

- [ ] Distinguish proven vs. inferred:
  - **Proven:** Sign reversal + preserved polarization + unchanged Cₚ (to 10³)
  - **Inferred:** Mechanism is interfacial charge screening

---

## COMMENT 7: Data Consistency Issues - Vₓ at 10³ Cycles
**Severity:** MEDIUM - Data Integrity

### The Discrepancy:
- Table II: Vₓ = 2.37 V at 10³ cycles
- Pristine: Vₓ = 2.08 V
- Stated variation: ±4%
- **Actual: 14% change — OUTSIDE stated range**

### Author's Note:
- Figure 2 labels this as "single unverified trace"
- But included in Table II anyway
- Inconsistent with text claiming "Vₓ constant to 4%"

### Required Actions:
- [ ] **CRITICAL:** Explain in caption and text:
  - Why is trace considered "unverified"?
  - Was it excluded from 4% variation calculation?
  - Why retain in Table II if unverified?
  - Redo analysis excluding this point?

- [ ] Revise Conclusion:
  - Current: "Vₓ is constant to within 4% at every verified checkpoint through 10⁴"
  - This should clarify: through 10² or through 10⁴ (excluding 10³)?

- [ ] Verify all other Table II values against Figure 2

---

## COMMENT 8: Manuscript Quality Issues
**Severity:** LOW - Production/Polish

### Issues Noted:
- Unresolved cross-references: "Table ??" and "[?]"
- Spacing errors
- Typographical errors
- Inconsistencies between main text, figures, tables, conclusions

### Required Actions:
- [ ] **Full proofread:**
  - Search for: "??", "Table ?", "Fig ?"
  - Fix all unresolved references
  
- [ ] **Consistency check:**
  - Does each statement appear consistently in:
    - Abstract
    - Main text
    - Figure captions
    - Table captions
    - Conclusion
  
  - Flag contradictions (e.g., 4% variation vs. 14% value)

- [ ] **Terminology standardization:**
  - Hysteresis window: always ΔVₕ
  - Remanent polarization: always 2Pᵣₑₘ
  - Coercive voltage: always Vₓ

---

## SUMMARY OF MAJOR REQUIRED REVISIONS

| Priority | Issue | Page | Fix Complexity |
|----------|-------|------|-----------------|
| 🔴 CRITICAL | Novelty vs. prior work | Intro, Abstract | HIGH |
| 🔴 CRITICAL | Sign reversal artifact concern | Sec III-C, Results | HIGH |
| 🔴 CRITICAL | Capacitance claim vs. 10⁴ validity | Sec III-D, III-F | HIGH |
| 🟠 HIGH | Memory/endurance claims vs. DC-sweep | Throughout | MEDIUM |
| 🟠 HIGH | Statistical significance misrepresentation | Sec III-A, Fig 4 | MEDIUM |
| 🟡 MEDIUM | Charge location overstatement | Sec III-F | LOW |
| 🟡 MEDIUM | Vₓ 10³ data inconsistency | Table II, Sec II | MEDIUM |
| 🟢 LOW | Manuscript polish | Throughout | LOW |

---

## RECOMMENDED RESPONSE STRATEGY

### Phase 1: Address Criticality Issues
1. Clarify novelty relative to published work
2. Provide complete data table for 10⁴ cycles
3. Fix capacitance claim contradiction
4. Tone down interpretation language

### Phase 2: Strengthen Experimental Support
1. Add multi-device data at 10⁴ cycles if available
2. Provide uncorrected Cₚ analysis
3. Clarify error bar meanings

### Phase 3: Polish & Consistency
1. Full proofread
2. Verify all cross-references
3. Ensure consistency across sections

---

## QUESTIONS FOR AUTHORS TO CONSIDER

1. **Novelty:** What specific findings have NOT been reported in the ACS papers?
2. **Artifacts:** Can you provide data distribution showing robust sign reversal across frequencies/amplitudes at 10⁴?
3. **Capacitance:** What physical meaning does ΔVₕ have when Cₚ-Rₚ model fails?
4. **Statistics:** Can multi-device measurements at 10⁴ cycles be obtained to strengthen reproducibility?
5. **Mechanism:** What would definitively prove interfacial vs. bulk charge origin?

