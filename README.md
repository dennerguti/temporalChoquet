# Choquet Comparative Models

This repository presents the fundamental equations and mathematical foundations used for the comparative study of Choquet-based models. These equations are essential for understanding how different aggregation and weighting mechanisms perform in time-dependent scenarios.

---

## Overview

The equations below describe the mathematical structure behind the **Choquet comparative models**, emphasizing the role of each variable and parameter.

- **X** represents the time measure, applied over **sliding windows** ranging from sizes 5 to 130.  
- **Y** represents the **weights** assigned to the mathematical models: **SMA**, **WMA**, **PMA**, **EMA**, and **HMA**.

The weight distribution is designed so that the sum always equals **1**, ensuring that each analysis remains normalized, concise, and accurate. These formulations enable the systematic evaluation of performance, adaptability, and robustness across models.

Furthermore, they provide a reproducible and transparent framework for all stages — from data collection to model application — allowing researchers to interpret and compare the results in a consistent way. Ultimately, these equations serve as the theoretical and analytical foundation for assessing the Choquet models’ performance across different temporal conditions.

---

## I. T-Norms

### Minimum  
<p align="center"><code>T<sub>M</sub>(x, y) = min{x, y}</code></p>

### Algebraic Product  
<p align="center"><code>T<sub>P</sub>(x, y) = xy</code></p>

### Łukasiewicz  
<p align="center"><code>T<sub>L</sub>(x, y) = max{0, x + y − 1}</code></p>

### Hamacher Product  
<p align="center">

$$
T_{HP}(x, y) =
\begin{cases}
0, & \text{if } x = y = 0 \\
\frac{xy}{x + y - xy}, & \text{otherwise}
\end{cases}
$$
</p>

---

## II. Overlap Functions

### OB(x, y)
<p align="center"><code>OB(x, y) = min{x√y, y√x}</code></p>

### Cuadras-Augé Copula  
<p align="center"><code>O<sub>mM</sub>(x, y) = min{x, y}·max{x², y²}</code></p>

### Oα(x, y)
<p align="center"><code>O<sub>α</sub>(x, y) = xy(1 + α(1 − x)(1 − y)),  α ∈ [−1, 1]</code></p>

### ODiv(x, y)
<p align="center"><code>O<sub>Div</sub>(x, y) = (xy + min{x, y}) / 2</code></p>

### Geometric Mean  
<p align="center"><code>GM(x, y) = √(xy)</code></p>

### Harmonic Mean  
<p align="center">

$$
H_S(x, y) =
\begin{cases}
0, & \text{if } x = y = 0 \\
\frac{2}{\frac{1}{x} + \frac{1}{y}}, & \text{otherwise}
\end{cases}
$$
</p>

### Sine  
<p align="center"><code>Sine(x, y) = (π / 2)·(xy)^(1/4)</code></p>

### ORS  
<p align="center"><code>ORS(x, y) = min{ ((x + 1)√y) / 2, y√x }</code></p>

---

## III. Copulas That Are Neither T-Norms Nor Overlap Functions

### CF(x, y)
<p align="center"><code>CF(x, y) = xy + x²y(1 − x)(1 − y)</code></p>

### CL(x, y)
<p align="center"><code>CL(x, y) = max{ min{x, y/2}, x + y + 1 }</code></p>

---

## IV. Aggregation Functions Other Than (I)–(III)

### FGL(x, y)
<p align="center"><code>FGL(x, y) = √( x(y + 1) / 2 )</code></p>

### FBPC(x, y)
<p align="center"><code>FBPC(x, y) = xy²</code></p>

---

## V. Left 0-Absorbent (0,1)-Pre-Aggregation Functions

### FNA(x, y)
<p align="center">

$$
FNA(x, y) =
\begin{cases}
x, & \text{if } x ≤ y \\
min(x, y), & \text{otherwise}
\end{cases}
$$
</p>

### FNA₂(x, y)
<p align="center">

$$
FNA₂(x, y) =
\begin{cases}
x, & \text{if } x ≤ y \\
\frac{x(y + 1)}{2}, & \text{if } 0 < x ≤ y \\
min(x, y), & \text{otherwise}
\end{cases}
$$
</p>

---

## Citation

If you use or reference these formulations, please cite this repository and acknowledge the Choquet comparative framework in your work.
