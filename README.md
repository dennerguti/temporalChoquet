# Choquet Comparative Models

This repository presents the fundamental equations and mathematical foundations used for the comparative study of Choquet-based models. These equations are essential for understanding how different aggregation and weighting mechanisms perform in time-dependent scenarios.

---

## Overview

The equations below describe the mathematical structure behind the **Choquet comparative models**, emphasizing the role of each variable and parameter.

- **X** represents the time measure, applied over **sliding windows** ranging from sizes 5 to 130.  
- **Y** represents the **weights** assigned to the mathematical models: **SMA**, **WMA**, **PMA**, **EMA**, and **HMA**.

The weight distribution is designed so that the sum always equals **1**, ensuring that each analysis remains normalized, concise, and accurate. These formulations enable the systematic evaluation of performance, adaptability, and robustness across models.

Furthermore, they provide a reproducible and transparent framework for all stages, from data collection to model application, allowing researchers to interpret and compare the results in a consistent way. Ultimately, these equations serve as the theoretical and analytical foundation for assessing the Choquet models’ performance across different temporal conditions.

## I. T-Norms

### Minimum
$$
T_M(x, y) = \min(x, y)
$$

### Algebraic Product
$$
T_P(x, y) = xy
$$

### Łukasiewicz
$$
T_L(x, y) = \max(0, x + y - 1)
$$

### Hamacher Product
$$
T_{HP}(x, y) =
\begin{cases}
0, & \text{if } x = y = 0 \\
\dfrac{xy}{x + y - xy}, & \text{otherwise}
\end{cases}
$$

---

## II. Overlap Functions

### OB(x, y)
$$
OB(x, y) = \min(x\sqrt{y},\, y\sqrt{x})
$$

### Cuadras-Augé Copula
$$
O_{mM}(x, y) = \min(x, y) \cdot \max(x^2, y^2)
$$

### \( O_{\alpha}(x, y) \)
$$
O_{\alpha}(x, y) = xy \big(1 + \alpha(1 - x)(1 - y)\big), \quad \alpha \in [-1, 1]
$$

### ODiv(x, y)
$$
O_{Div}(x, y) = \frac{xy + \min(x, y)}{2}
$$

### Geometric Mean
$$
GM(x, y) = \sqrt{xy}
$$

### Harmonic Mean
$$
H_S(x, y) =
\begin{cases}
0, & \text{if } x = y = 0 \\
\dfrac{2}{\dfrac{1}{x} + \dfrac{1}{y}}, & \text{otherwise}
\end{cases}
$$

### Sine
$$
Sine(x, y) = \frac{\pi}{2} \, (xy)^{\frac{1}{4}}
$$

### ORS
$$
ORS(x, y) = \min\left( \frac{(x + 1)\sqrt{y}}{2},\, y\sqrt{x} \right)
$$

---

## III. Copulas That Are Neither T-Norms Nor Overlap Functions

### CF(x, y)
$$
CF(x, y) = xy + x^2 y (1 - x)(1 - y)
$$

### CL(x, y)
$$
CL(x, y) = \max\left( \min\left(x, \frac{y}{2}\right),\, x + y + 1 \right)
$$

---

## IV. Aggregation Functions Other Than (I)–(III)

### FGL(x, y)
$$
FGL(x, y) = \sqrt{ \frac{x(y + 1)}{2} }
$$

### FBPC(x, y)
$$
FBPC(x, y) = xy^2
$$

---

## V. Left 0-Absorbent (0,1)-Pre-Aggregation Functions

### FNA(x, y)
$$
FNA(x, y) =
\begin{cases}
x, & \text{if } x \le y \\
\min(x, y), & \text{otherwise}
\end{cases}
$$

### FNA₂(x, y)
$$
FNA_2(x, y) =
\begin{cases}
x, & \text{if } x \le y \\
\dfrac{x(y + 1)}{2}, & \text{if } 0 < x \le y \\
\min(x, y), & \text{otherwise}
\end{cases}
$$
