# Response to Reviewers

**Manuscript:** TED-2026-08-2206-R
**Title (revised):** Sign Reversal of the DC-Sweep Capacitance–Voltage Hysteresis
Window in Hf₀.₅Zr₀.₅O₂ Ferroelectric Transistors

---

We thank both reviewers for a careful and constructive reading. In response we have
measured **four additional devices**, added **transfer characteristics** after program
and erase across the cycling range, repeated the full series at a **ten-fold longer
integration time**, and extended the frequency and amplitude coverage. We have also
restricted several claims the reviewers correctly identified as over-stated, and
corrected the title accordingly.

Changes are marked in blue in the marked copy. Figure numbers below refer to the
revised manuscript.

**Summary of new measurements**

| measurement | scope |
|---|---|
| C–V, devices 6 and 7 | 7 frequencies (1 kHz–1 MHz) × 4 amplitudes, 6–7 checkpoints |
| C–V, devices 2 and 3 | full cycling series at two integration settings |
| Transfer characteristics | program and erase at 6 checkpoints, 5 extraction criteria |
| Total | five devices for C–V, from one for the original submission |

---

## Reviewer 2

### R2-1 — Overlap with the authors' recent publications; statement of novelty

**Accepted. The Introduction has been restructured around this point.**

Both papers are now cited and the relationship stated explicitly (Section I,
paragraphs 3–4).

*Endurance Paradox* (ACS AMI 2026) established that ferroelectric polarization
survives after the FeFET memory window collapses. *Quantifying Endurance-Driven Loss
of Polarization-to-Channel Charge Coupling* (ACS AEM 2026) extracted an apparent
channel-coupled charge density from the threshold-voltage shift, defined a
polarization-to-channel coupling factor, and reported its decrease from 3.5% to 0.9%
at 10⁴ cycles.

The manuscript now states: *"Both establish that the coupling between polarization and
channel degrades while polarization persists; we do not claim that observation as
new."*

Three findings are identified as new, in the paragraph beginning *"Three findings in
the present work are not contained in those studies"*:

1. **The window becomes negative, not merely small.** A coupling factor is
   non-negative by construction, so the regime in which interfacial charge
   *over-compensates* rather than merely screens the polarization field cannot be
   expressed in that framework.
2. **The reversal is established on five independent devices**, across three decades
   of measurement frequency, four sweep amplitudes and a ten-fold change in
   integration time — none of which was reported previously.
3. **It is resolved from the gate-stack C–V alone**, and independently confirmed by
   transfer characteristics.

Following the reviewer's suggestion, the novelty claim is limited to the sign reversal
and its frequency- and conductance-dependent characteristics. All statements about
interface-driven degradation in general are now attributed to the prior work.

**Device structure, wafer and cycling conditions** are identical to the prior studies
(same die and process, ±5 V / 50 µs). All C–V, transfer and polarization data
presented here are new to this manuscript and were acquired on devices not previously
measured. This is stated in the new Section II-B.

---

### R2-2 — Claims about memory failure are not supported by DC-sweep hysteresis

**Accepted in full.** The reviewer is correct that the reported quantity is DC-sweep
hysteresis.

The **title has been changed** to name the measured quantity. The following wording
has been removed throughout:

| removed | replaced with |
|---|---|
| "the device has ceased to store information" | "the hysteresis window has collapsed" |
| "endurance failure" (as a device-level claim) | "loss of DC-sweep hysteresis" |
| "it inverts its memory" | "the sense of the hysteresis loop reverses" |
| "memory window" (unqualified) | "DC-sweep hysteresis window" |

Section II-D now states: *"It is not the retained state of a pulse-written bit, and no
claim about stored information is made from it alone."*

**We have additionally measured the transistor quantity directly** (new Section III-E,
Fig. 8, Table V). ΔV_th falls from +0.581 V pristine to −0.015 V at 10⁴ cycles, i.e.
the transistor threshold window collapses and reverses sign on the same schedule as
the capacitance window (Fig. 7c). The relation assumed in Section II-D is therefore
now supported by measurement rather than asserted.

---

### R2-3 — Evidence that the sign reversal is not a measurement artifact

**Addressed experimentally by three independent checks, now Section III-C and Fig. 5.**

**(a) The reversal is present in uncorrected data.** Using the measured C_p with no
series correction, 25 of 27 surviving sweeps at 10⁴ cycles on device-1 are negative,
spanning five frequencies, four sweep amplitudes and both pulse states. The reversal
is therefore not produced by the correction of Eq. (8).

**(b) It survives a ten-fold change in integration time.** The full cycling series was
repeated on devices 2 and 3 with the ADC integration increased from 1 to 10 power-line
cycles (16.7 → 167 ms per point):

| N | dev-2, PLC 1 | dev-2, PLC 10 | dev-3, PLC 1 | dev-3, PLC 10 |
|---|---|---|---|---|
| 10³ | −0.021 | −0.022 | +0.129 | +0.141 |
| **10⁴** | **−0.265** | **−0.211** | **−0.262** | **−0.205** |
| 10⁵ | −0.115 | −0.098 | −0.105 | −0.087 |

The sign is unchanged at every checkpoint through 10⁵ on both devices. Magnitudes
differ by 15–22%, and in the reversed regime they move **toward** zero at longer
integration. Charge leaking during the integration window would produce the opposite
dependence, since a longer integration would deepen an artifact-driven negative
window. The observed trend is therefore inconsistent with that mechanism.

**(c) It is present at every frequency and amplitude measured.** Devices 6 and 7 were
characterised at seven frequencies from 1 kHz to 1 MHz and four sweep amplitudes from
±1.5 V to ±3 V at each checkpoint. The window is negative at 10⁴ cycles in every one
of these conditions (Fig. 4d, Fig. 5a). At 10⁴ on device-7, ΔV_hyst = −0.261, −0.281,
−0.275 and −0.281 V at 100, 300, 500 kHz and 1 MHz respectively.

The loss tangent, valid-sweep count and unfiltered results at each frequency and
amplitude are provided in the supplementary data file accompanying this submission.

---

### R2-4 — Single device; the "4.6σ" statement

**Accepted. The statistical claim has been removed and four additional devices
measured.**

The "negative by 4.6σ" statement is deleted. As the reviewer notes, that figure
derived from spread across measurement conditions rather than independent devices.

**Five devices are now reported** (Fig. 4a, Table I):

| N | dev-1 | dev-2 | dev-3 | dev-6 | dev-7 |
|---|---|---|---|---|---|
| pristine | +0.363 | +0.822 | +0.804 | +0.791 | +0.803 |
| 10³ | −0.052 | −0.021 | +0.129 | +0.010 | +0.172 |
| **10⁴** | **−0.151** | **−0.265** | **−0.262** | **−0.205** | **−0.275** |
| 10⁵ | — | −0.115 | −0.105 | — | −0.116 |

All five show a counter-clockwise window when fresh and a clockwise window by 10⁴
cycles. Interpolated zero crossings are **503, 871, 1117, 2136 and 2422 cycles** — a
spread of a factor of five (Fig. 4b).

The window efficiency shows still closer agreement: devices 2, 3, 6 and 7 give
**15.9–16.5% pristine** and converge to **−3.2 to −4.2% at 10⁴** (Table II).

**Error bars** are now defined explicitly in each caption as the standard deviation
over the stated sweep amplitudes and frequencies, with the number of sweeps given.
Device-to-device spread is presented separately as the range across devices.

We note that device-1 has a smaller pristine window (0.363 V) than the other four
(0.79–0.82 V). This is stated in Section III-B as die-to-die variation; the sign
reversal is common to all five.

---

### R2-5 — The capacitance claim cannot be extended to 10⁴ cycles

**Accepted. The reviewer is correct, and the new data confirms this more strongly than
the original manuscript indicated.**

Testing the validity of Eq. (8) at each checkpoint on all devices, a physically
meaningful corrected capacitance is obtained through 10³ cycles on device-1 and
through 10² on device-2. At 10⁴ cycles ωR_sC ≈ 0.50 on every device and the correction
is ill-conditioned.

**The claim of three simultaneous observations at 10⁴ has been removed.** Section III-D
now states: *"No corrected value is quoted there, and the claim of an unchanged
capacitance is not extended to the checkpoint at which the sign reversal occurs."*

In its place we make a narrower and better-supported statement. On device-2, over
N = 1 to 10² cycles:

- C_acc = **184.2 ± 1.6 pF (±0.9%)**, with the correction **below 1.9%** at every
  point and D = 0.12–0.15;
- ΔV_hyst falls from 0.920 V to 0.331 V, i.e. **64% of the collapse**.

The stack capacitance is therefore constant to better than 1%, on essentially
uncorrected data, over the range in which the window loses most of its magnitude.

---

### R2-6 — The charge location is not uniquely determined

**Accepted. The language has been moderated throughout.**

Removed: *"Only one class of explanation survives"*, *"all point to the same
interfacial region"*, and the unqualified recommendation of *"interface engineering
rather than ferroelectric engineering"*.

The mechanism is now described as **effective charge within the channel-side gate
stack**, following the reviewer's phrasing, and Section III-G states that the
measurements *"do not distinguish charge in bulk HZO, at the HZO/SiO₂ interface,
within SiO₂, or at the SiO₂/Si interface."*

We have also removed the claim that the flank asymmetry, imprint drift and conduction
increase share a single origin, and now state that the mechanism is presented *"as
consistent with charge trapping rather than as an identification of the responsible
traps."* TEM-EELS and charge pumping are identified as the measurements that would
localize and quantify it directly.

---

### R2-7 — V_c at 10³, and unresolved cross-references

**Both corrected.**

**The 10³ P–V trace.** The program- and erase-state columns for this checkpoint are
byte-identical in the source workbook, so only one measurement exists there; this is
why it is labelled unverified. It was excluded from the V_c variation statistic for
that reason. In the revision it is (i) retained in Table III with an explicit footnote,
(ii) drawn as an open symbol in Fig. 2, and (iii) excluded from all fitted quantities,
with the exclusion stated. Recomputing over the verified checkpoints ≤10⁴ gives
**3.7%**; the manuscript now states 4% consistently in the abstract, text and captions.

**Cross-references.** All unresolved references (`Table ??`, `[?]`) have been fixed and
the manuscript recompiled with no undefined references or citations. The missing
left-hand side of Eq. (5) (the symbol V_imp) has been restored. The manuscript has
been proofread throughout, and the figure captions and axis labels corrected.

---

## Reviewer 1

### R1-1 — Verify the memory-window failure by transistor readout

**Accepted, and addressed with new measurements (Section III-E, Fig. 8, Table IV).**

Transfer characteristics were measured after ±5 V, 50 µs program and erase at each
cycling checkpoint. The extraction method and read delay are stated explicitly:
V_th at a constant current of 1 µA, V_D = 0.1 V, read delay 60 s determined from
measurement timestamps, all terminals at 0 V during the delay, and each read preceded
by a fresh write.

| N | V_th(program) | V_th(erase) | ΔV_th |
|---|---|---|---|
| pristine | 0.294 | 0.875 | **+0.581** |
| 10² | 0.533 | 0.776 | +0.243 |
| 10³ | 0.327 | 0.434 | +0.108 |
| **10⁴** | 0.083 | 0.067 | **−0.015** |

The transistor threshold window collapses and reverses sign at 10⁴ cycles, on the same
schedule as the capacitance window (Fig. 7c). The reversal is **independent of the
extraction criterion**, being present at 1, 3, 10, 30 and 100 µA (Fig. 8c).

We note the two quantities are measured on very different timescales — 60 s for the
transistor read against ~17 ms per point for C–V — so their agreement indicates that
the responsible charge is stable over at least that range. This is stated in the text.

In line with the reviewer's alternative instruction, all claims about memory failure
and stored information have nonetheless been removed from the abstract, title and
conclusion, and the manuscript is framed around the hysteresis window.

---

### R1-2 — Interpretation of the charge density from Eq. (9)

**Accepted.**

The quantity is an equivalent areal charge density inferred from the window shift and
the interfacial capacitance, not a directly extracted interface-trap density. It has
been renamed **ΔN_eq** throughout, and the assumptions are now stated: *"Equation (11)
assumes a sheet charge at the interfacial layer and an unchanged C_IL; it is an
equivalent density inferred from a voltage shift, not a directly extracted
interface-trap density, and is denoted N_eq for that reason."*

Following the reviewer's instruction where independent trap-sensitive data is not
available, the mechanism is now **presented as consistent with charge trapping rather
than as an identification of the responsible traps** (Section III-G). Charge pumping
and TEM-EELS are identified as the measurements required to quantify and localize it.

We attempted transient recovery measurements (fixed-V_G drain-current sampling after
program and erase at pristine, 10³ and 10⁴ cycles). The terminal currents in the
erase-state measurements did not satisfy Kirchhoff's law — the source and body currents
cancelled while the drain current lay outside that loop — indicating a parasitic
conduction path in the measurement configuration. We have therefore excluded these
data rather than present a transient we cannot attribute to the channel. The
measurement is being repeated.

---

### R1-3 — Roles of wake-up, charge trapping and fatigue

**Accepted, and the framing has been rewritten.**

The statement that endurance failure is "not" caused by ferroelectric fatigue was too
general. The revised text states that **loss of switchable polarization alone cannot
account for the early collapse of the DC-sweep hysteresis window in these devices**,
and Section III-A now says explicitly: *"We therefore do not claim that ferroelectric
fatigue is absent. The ferroelectric does degrade, approximately two decades after the
hysteresis window has collapsed."*

At 10⁵ cycles the reduction in 2P_r to 18.6 µC/cm², the broadening of the switching
peaks and the rise in non-switching current are now presented as evidence that
ferroelectric and electrical degradation do contribute at later stages.

We now also state that **wake-up and charge trapping proceed simultaneously** during
early cycling rather than sequentially, supported by new data: devices 2 and 3 show
wake-up in the hysteresis window itself, rising from 0.822 to 0.920 V and from 0.804
to 0.968 V between pristine and one cycle before collapsing.

The Introduction and abstract have been revised to acknowledge prior identification of
charge trapping, trap generation and ferroelectric/dielectric interfacial-layer effects
as established FeFET endurance mechanisms, with citations to Yurchuk, Gong & Ma,
Toprasertpong, Tasneem and Passlack.

---

### R1-4 — Limitations: charge location, response time, reproducibility

**All three accepted and stated explicitly in Section III-G.**

**Charge location.** Addressed under R2-6. The description is now "effective charge
within the channel-side gate stack", following the reviewer's suggested phrasing.

**Response time.** We agree that the microsecond time constant from the AC dispersion
and the ~17 ms dwell of the DC sweep cannot be assigned to the same charge population.
The manuscript now states that **no common origin is claimed**, and additionally notes
that δV in Eq. (12) decreases with cycling rather than growing, so the AC-active
population is not the one responsible for the reversal.

**Reproducibility.** Four additional devices have been measured; the C–V sign reversal
is now established on five devices (R2-4). The remaining limitations are stated
plainly:

- the five devices are from a single die, and the zero-crossing cycle count varies by
  a factor of five among them;
- polarization (PUND) and transfer characteristics were each measured on a **single
  device**, so the decoupling argument combines a five-device window measurement with
  single-device polarization and transistor references;
- η depends on the convention chosen for the ideal window, and alternative denominators
  shift the absolute values but not the sign change or the trend.

**Provenance of the polarization data.** In the interest of transparency we draw the
reviewers' attention to a point not made explicit in the original submission. The PUND
measurement was performed on one device of the die, not on each device individually.
Because polarization behaviour is uniform across devices of this process, the resulting
2P_r(N) is used as a **common reference** against which the window of every device is
compared, rather than as a per-device quantity. This is now stated in the new
Section II-B and in the caption of Table II.

---

## Summary of changes

| section | change |
|---|---|
| Title | narrowed to the measured quantity |
| Abstract | rewritten; five devices, integration control, transistor confirmation |
| I | prior work cited and differentiated; three novel findings identified |
| II-B | **new** — devices and data provenance |
| II-D | transfer-characteristic method, read delay, extraction criterion |
| II-E | **new** — integration-time control |
| II-G | ΔN_it → ΔN_eq with assumptions stated |
| III-B | five-device window; die-to-die variation stated |
| III-C | **new** — three artifact checks |
| III-D | capacitance claim restricted to the valid range |
| III-E | **new** — transistor-level confirmation |
| III-F | efficiency against the common reference, five devices |
| III-G | mechanism language moderated; limitations stated |
| Figures | 8 figures, of which 4 are new or substantially rebuilt |
| Tables | 4 tables, of which 3 are new or rebuilt |
