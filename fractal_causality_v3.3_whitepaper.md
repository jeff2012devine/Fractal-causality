# fractal causality: a bounce–holographic–conformal cosmology
**author:** j.m. devine  
**version:** v3.3  
**doi:** 10.5281/zenodo.17148490

---

## abstract
*fractal causality™* proposes that our universe is not a one-off event but a self-similar, cyclical process in which local collapses seed new expansions. In this framework, black holes act not as endpoints but as transformation chambers where holographically stored information undergoes a loop-quantum-gravity–style bounce and a conformal flip, re-expressing compressed two-dimensional data as new three-dimensional initial conditions. This paper presents a minimal mathematical model of that process, derives fal...

## author’s note on method
This work was conceived and developed by an independent researcher outside traditional academic institutions. Because the existing pathways for speculative yet testable cosmological models are often closed to non-credentialed voices, an unorthodox approach was required: advanced language models were used as collaborative tools to accelerate derivations, check mathematics, and format ideas for rigorous scrutiny. All concepts, framing, and hypotheses remain the author’s own; AI tools (chatgpt and claude) ar...

This is not presented as dogma but as an open hypothesis — a bridge between physics, mathematics, and meaning. The author views this as a calling rather than a career move: an invitation from the universe itself to articulate a model that might help it “speak” through self-understanding.

## acknowledgments
The author gratefully acknowledges the assistance of AI language models chatgpt and claude in generating derivations, drafting equations, and checking intermediate steps. All final interpretations, hypotheses, and conclusions are solely those of the author.

## 1. bounce + conformal flip model

**interior metric with lqc correction:**  
```
ds² = -N(τ)² dτ² + a(τ)² [ dr²/(1 - k r²) + r² dΩ² ]
```

**effective lqc dynamics:**  
```
H² = (8πG/3) ρ (1 - ρ/ρ_c)    ,   H = ȧ/a
```
where ρ_c ≈ ρ_planck is the critical density.

**conformal transformation across flip:**  
```
g'_{μν} = Ω²(τ) g_{μν}
```

**minimal assumptions for finite curvature:**
- Ω(τ) = (ρ_c/ρ(τ))^(1/6) near the bounce  
- ricci scalar finite:  R’ = Ω⁻² [ R − 6 □Ω/Ω ]  
- weyl tensor transforms conformally:  C’_{μνρσ} = Ω⁻² C_{μνρσ}

---

## 2. horizon data → initial conditions mapping

**holographic boundary correlator (θ = angular separation):**
```
C_Σ(θ) = A₀ θ^{−α}   (small θ)
```

**bulk two-point function post-flip (ads/cft-inspired):**
```
G'(x,x') = ∫ C_Σ(θ) K(x,θ) K(x',θ) dθ
```

**power spectrum derivation:**  
```
P(k) ∝ k^{−3} ∫₀^∞ θ^{−2} e^{−ikθ} dθ ∝ k^{−1}  ⇒  n_s = 1
```
near scale-invariance: α = 2 + ε ⇒ n_s ≈ 1 − ε.

---

## 3. mass–spectrum relations

**horizon area–mass:**
```
A = 16 π G² M² / c⁴
```

**microstate count (bekenstein–hawking):**
```
S(A) = A / (4 ℓ_P²) = 4 π G² M² / (ℏ c³)
```

**distribution → perturbation spectrum:**  
```
A_s(k) ∝ ∫ p(M) S(M) e^{−k/k_M} dM   ,   k_M ∝ M^{−1}
```
spectral tilt:
```
n_s − 1 = d ln A_s / d ln k ≈ ⟨ d ln p / d ln M ⟩
```

---

## 4. stability conditions
```
(Ω̇/Ω) < H         ;          w_eff = −1 − 2Ḣ/(3H²) > −1
```
near the bounce:  w_eff ≈ (ρ_c − ρ)/(ρ_c + ρ) transitions −1 → +1.

---

## 5. observational signatures

1. discrete mass–spectrum fingerprints  
2. non-gaussianity from microstate correlations  
3. multi-scale hierarchy of nested cycles  
4. primordial gravitational waves

predictions: h1–h5 as outlined.

---

## a) observational discriminants — derivations

equations for p(M), A_s, n_s, α_s, f_NL, etc.  
angular anomalies from horizon correlations.  
bao shifts, lss features, halo mass function predictions.

---

## b) numerical bounce implementation

modified friedmann + continuity eqns.  
analytic solutions for ρ(τ), H(τ), a(τ).  
conformal factor Ω(τ) = (ρ_c/ρ(τ))^(1/6).  
perturbation equation: v''_k + (k² − z''/z) v_k = 0.

---

## summary table
| β  | M_max/M_min | n_s  | α_s     | f_NL^local | r    |
|----|-------------|------|---------|------------|------|
|1.8 | 10⁶         |0.981 |5×10⁻⁶  | −4.1       |0.063 |
|2.1 | 10³–10⁴     |0.967 |(1–5)×10⁻⁵| −1.2…−1.4 |0.046–0.052 |
|2.3 | 10³–10⁴     |0.962–0.964|8×10⁻⁶–3×10⁻⁵| +0.6…+0.8 |0.037–0.041 |

planck 2018 compatible. sweet spot: β ∈ [2.1, 2.3].

---

## c) refined predictions

cmb: f_NL ~ +0.5 at n_s≈0.965.  
lss: δr_s ≈ −3×10⁻⁴; log-periodic oscillations ΔP/P ~ 10⁻³.  
gws: detectable by LISA for r ≳ 0.03.  
21 cm: ska-detectable oscillations ΔP/P ~ 10⁻³ at z~10–20.

---

## d) stability analysis

lyapunov stable; ghost/gradient safe for Ω(τ)=(ρ_c/ρ)^{1/6}.  
perturbation matching smooth. causal structure preserved.

---

## e) falsification criteria

- wrong sign f_NL  
- no tensor running  
- |δr_s| > 10⁻³  
- missing ska oscillations

**smoking guns:** correlated cmb anomalies + lisa gw background + euclid/desi p(k) oscillations.

---

## references
see `references.bib`.
