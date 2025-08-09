Thanks, Nima! I’ve reviewed your friend’s README and now I’ll help you write a similar one for your ICU bed allocation project. It will be clean, math-rich, and explanatory—just like theirs.

---

# ICU Bed Allocation via Game Theory

This project simulates ICU bed allocation among hospitals using two game-theoretic mechanisms: optimal auctions and stable matching. Patients arrive randomly and are assigned values based on exponential distributions:

$$
f_i(t) = 0.5i \cdot e^{-0.5i t}, \quad i \in \{1, 2\}
$$

Each hospital has a fixed number of beds. Patients are prioritized based on their value \( v_i \), and allocation is determined by:

- **Optimal Mechanism**: Beds go to patients with highest \( C_i(v_i) \); payments are auction-based.
- **Stable Matching**: Patients are matched to hospitals based on preferences and availability.

Mortality is modeled as:

$$
P_{\text{death}}(t) = 1 - 2 \cdot e^{-0.5i t}
$$

### Metrics

- Average hospital income
- Average patient payment
- Number of deceased patients

### Observations

- Stable matching yields higher hospital income.
- Optimal mechanism results in higher mortality due to stricter selection.
- Insurance discounts reduce patient payments under stable matching.

The full methodology and results are documented in the LaTeX report.

---

Let me know if you'd like to include code snippets or visualizations next!
