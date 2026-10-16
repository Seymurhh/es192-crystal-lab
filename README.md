# ES 192 Crystal Lab

Interactive models for **ES 192: Materials Selection in Mechanical Design** (Harvard SEAS), Weeks 9–10, Materials Fundamentals.

**Live page:** https://seymurhh.github.io/es192-crystal-lab/

| Tab | Link | Lecture | What it shows |
|---|---|---|---|
| Bonds | [#bonds](https://seymurhh.github.io/es192-crystal-lab/#bonds) | 9A | Ionic, covalent, metallic, van der Waals and hydrogen bonds; energy–distance and force–distance curves; bond energy vs melting point for 20 substances |
| Unit cells | [#cells](https://seymurhh.github.io/es192-crystal-lab/#cells) | 9A | SC, BCC, FCC, HCP, rock salt and diamond cubic in 3D; atoms per cell, coordination shells, densest planes, real metals with computed lattice constant and density, iron's BCC ↔ FCC change |
| Stack the layers | [#stack](https://seymurhh.github.io/es192-crystal-lab/#stack) | 9A | Build close-packed layers: ABAB → HCP, ABCABC → FCC, stacking faults |
| Atom raft | [#raft](https://seymurhh.github.io/es192-crystal-lab/#raft) | 9A · 10A | Live 2D Lennard-Jones simulation (~1,800 atoms): melting, slow cooling vs quenching, grain orientation map, vacancies, solutes, glass formation |
| Dislocations | [#disl](https://seymurhh.github.io/es192-crystal-lab/#disl) | 10A | Edge dislocation glide vs rigid slip, Burgers circuit, solute and grain-boundary pinning |
| Phase diagrams | [#phase](https://seymurhh.github.io/es192-crystal-lab/#phase) | Lab 9 · 10B | Cu–Ni, Pb–Sn (solder) and Fe–C (steel): hover or pin a point to see the phases, tie line and lever-rule fractions, a live microstructure and the atomic arrangement; "cool slowly" logs every phase change |

**Present mode** (top right) enlarges the models for projection.

## Embed in Canvas

In a Canvas page, switch the editor to HTML and paste:

```html
<iframe src="https://seymurhh.github.io/es192-crystal-lab/#cells" width="100%" height="900" style="border:0" allowfullscreen title="ES 192 Crystal Lab"></iframe>
```

Change `#cells` to any tab name above.

## Data sources

- Bond energies and melting points: Callister & Rethwisch, *Materials Science and Engineering: An Introduction*, 10th ed., Table 2.3.
- Atomic radii and crystal structures: same, Table 3.1. Atomic weights: Fig. 2.8. Computed density uses ρ = nA / (V<sub>C</sub> N<sub>A</sub>), Eq. 3.8.
- Measured densities and lattice constants for C, Si and NaCl: standard reference values.
- Phase diagrams: Pb–Sn and Fe–Fe₃C traced from the vector figures in Callister & Rethwisch 10e (Figs. 9.8, 9.24), snapped to the labelled invariant points; Cu–Ni fitted through the melting points of Cu and Ni and the 1250 °C tie line of §9.8 (Fig. 9.3b). Checks: Pb–Sn liquidus 214 °C at 50 wt% Sn (Table 9.1); Example Problem 9.2 and the §9.8 lever-rule example reproduced.

Bond-curve shapes (Morse form), raft temperatures (reduced Lennard-Jones units) and dislocation stresses (0–100 schematic scale) are teaching schematics that show trends, not measured values.

## Files

- `index.html`: the published page (self-contained; loads three.js r128 from cdnjs and fonts from Google Fonts).
- `crystal-lab.html`: the same page without the HTML document wrapper (source used for the claude.ai artifact).
