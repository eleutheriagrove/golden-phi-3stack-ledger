# Minimal 3-Stack Information-Dynamics Ledger: Explicit Spectrum and Prototype

## 1. Locked 3-Stack Definitions and Spectrum Change under $\sigma_i$

Levels $k = 1,2,3$ with rotation numbers successive Fibonacci approximants $\omega_k = F_n / F_{n+1} \to \phi^{-1} \approx 0.618$.

Residual charges $Q^{(k)} \in \mathbb{Z}$ (or residual group elements) locked by KAM persistence.

### Pre-surgery (Brunnian / Borromean triple)
| Quantity          | Value          |
|-------------------|----------------|
| $\operatorname{lk}_{12}$ | 0              |
| $\operatorname{lk}_{13}$ | 0              |
| $\operatorname{lk}_{23}$ | 0              |
| $\overline{\mu}_{123}$   | $\pm 1$      |
| $Q^{(1)}, Q^{(2)}, Q^{(3)}$ | fixed     |

### Action of directed surgery $\sigma_i$ (operates on level $i$)
Surgery rewrites higher-order invariants into ordinary linking at coarser levels and updates residual charges hierarchically.

**Example: $\sigma_2$ (middle level)**
- $\overline{\mu}_{123} \to 0$
- $\operatorname{lk}_{12} \to \pm 1$, $\operatorname{lk}_{23} \to \pm 1$, $\operatorname{lk}_{13}$ remains 0 (or intermediate)
- $Q^{(2)}$ updated; $Q^{(1)}$ (coarser) updated; $Q^{(3)}$ (finer) unchanged

**General pattern (piecewise):**
- Operated level and all coarser enclosing levels: charges and linking numbers rewritten.
- Finer levels: invariant.
- Continuous flow between surgeries: entire $\Sigma$ fixed.

This matches local reconnection converting Brunnian to Hopf/Whitehead intermediates (Lambropoulou–Antoniou) and the information-theoretic lift of MI minima.

## 2. Schematics
(See generated images in conversation: stacked tori with surgery arrows; Borromean-to-Hopf/Whitehead transition with spectrum labels.)

## 3. Discrete Computational Prototype
Three weakly coupled circle maps:
$$
\theta_k(t+1) = \theta_k(t) + 2\pi \omega_k + \epsilon \sum_{j \neq k} \sin(\theta_j - \theta_k) \pmod{2\pi}
$$
with $\omega_k$ Fibonacci approximants, $\epsilon \ll 1$.

Linking proxy: integrated phase-difference winding $\frac{1}{2\pi}\int d(\theta_i - \theta_j)$.

- Under continuous iteration: windings (and residual labels) stable (KAM-like protection).
- Discrete surgery (e.g., $\theta_i \leftarrow \theta_i + \pi$ at chosen step when proxy conditions hold): jumps the spectrum, after which continuous flow again freezes the new labels.

## 4. Information-Theoretic Side (Baudot–Bennequin)
Exact binary distributions realizing absolute minimum $J_3 = I(X;Y;Z) = -1$:

**Case 1:** $p_{000}=1/4, p_{011}=1/4, p_{101}=1/4, p_{110}=1/4$, others 0.

**Computed:**
- Individual $H(X)=H(Y)=H(Z)=1$
- Pairwise $I(X;Y)=I(X;Z)=I(Y;Z)=0$
- Triple interaction $I_3 = -1$

**Case 2:** mirror image, identical statistics.

**Surgery example** (mass redistribution lifting pairwise while destroying the pure triple minimum):
- Pre: pairwise 0, $I_3=-1$
- Post: selected pairwise rise, $I_3$ moves away from -1

Pre-surgery spectrum sits at the multivariate MI minimum (invisible to pairwise probes); surgery makes selected components visible—exactly the ledger behavior.

## 5. Concrete Platforms for Stress-Testing
- **DNA nanotech ligation**: physical reconnection of strands realizing Brunnian-to-Hopf transition; measure topological invariants before/after.
- **Multicomponent BEC vortex reconnection**: dynamical surgery on quantized vortices; track linking numbers and residual circulation (charges) under continuous flow vs. reconnection events.
- **Anyonic braiding circuits** (Fibonacci anyons): residual topological charges protected until deliberate braiding/surgery; implement 3-level hierarchy.
- **Pure numerical KAM + link-invariant codes**: extend the circle-map prototype to higher stacks, compute Milnor $\overline{\mu}$ proxies or finite-type invariants under controlled perturbations and discrete surgeries.

All can be started without wet-lab resources; the definitions and spectrum rules above are sufficient entry points.

## Piecewise spectrum table
| $\sigma$ | Pre $\operatorname{lk}$ | Post $\operatorname{lk}$ | $\overline{\mu}_{123}$ | Charges updated | Charges fixed |
|------------|---------------------------|----------------------------|---------------------------|-----------------|---------------|
| $\sigma_1$ | all 0 | $\operatorname{lk}_{12},\operatorname{lk}_{13}\to\pm1$ | $\to0$ | $Q^{(1)}$ | $Q^{(2)},Q^{(3)}$ |
| $\sigma_2$ | all 0 | $\operatorname{lk}_{12},\operatorname{lk}_{23}\to\pm1$ | $\to0$ | $Q^{(1)},Q^{(2)}$ | $Q^{(3)}$ |
| $\sigma_3$ | all 0 | $\operatorname{lk}_{13},\operatorname{lk}_{23}\to\pm1$ | $\to0$ | $Q^{(1)},Q^{(2)},Q^{(3)}$ | none |

## Total-recall dynamic memory extension
Content encoded in residual-charge patterns + Brunnian higher-order locks. Continuous KAM flow = associative search/exploration (no rewrite). Query match on lower levels triggers selective $\sigma_i$ that writes coarser charges and releases protected higher-order pattern for recall. Finer = local features, coarser = global context. Protected under noise until intentional class-changing update.
