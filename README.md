This repository presents a hybrid quantum-classical solution for the weighted MaxCut problem on energy grid graphs of 21 and 180 nodes. Direct QAOA simulation for the 180-node
graph requires 2180 amplitudes—computationally prohibitive. To address this, we implement a quantum preconditioning pipeline based on Dupont et al. (2025), where QAOA on small
subgraphs extracts two-point correlations ⟨ZiZj⟩ used to reweight the global graph before classical polish. Two subgraph selection strategies are compared: community detection (covers
63.7% of edges) and light-cone decomposition (covers 100% of edges). Light-cone preconditioning achieves a **+1.23% improvement** over the classical baseline for Problem B
(6861.27 vs. 6778.19), while community-based preconditioning slightly underperforms (-0.06%). This demonstrates that quantum-derived correlations for all edges—especially inter-community
bridges—provide unique structural guidance inaccessible to classical heuristics alone.

All the details is founded in Technical report (Rigetti_challenge_Beerantum.pdf)
