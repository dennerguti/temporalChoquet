Here are all the equations related to Choquet comparative models, emphasizing the importance of each variable and parameter for the work. The letter X represents the time measure conducted in sliding windows variations ranging from size 5 to 130, while the letter Y represents the weight values assigned to the mathematical models SMA, WMA, PMA, EMA, and HMA. These weights are distributed according to the window size to ensure that the sum always results in 1. This ensures that the analyses are concise and accurate. These fundamental equations are essential for understanding and analyzing the results; they provide a solid foundation for the comparative evaluation of the studied models.

Furthermore, the equations provide a quantitative framework for evaluating the effectiveness and performance of each model in various time scenarios. They provide a systematic way of understanding how variations in time windows impact the weighting of various mathematical models, providing valuable insights into their adaptability and robustness. These equations help ensure the transparency and replicability of the analyses performed by detailing each step of the analytical process, from data collection to model application. By using them, it's possible to thoroughly compare the Choquet models and determine their advantages and disadvantages in different usage contexts. Finally, the equations are essential for the theoretical grounding and practical application of this work, as they serve as the basis for researching and interpreting the results.


# I - T-norms

## Minimum  
<p align="center">$TM (x, y) = \min\{x, y\}$ </p>

## Algebraic Product  
<p align="center">$TP (x, y) = xy$ </p>

## Łukasiewicz 
<p align="center">$TL(x, y) = \max\{0, x + y - 1\}$ </p>

## Hamacher Product
$$
\ THP (x, y) =
  \begin{cases}
    0       & \quad \text{if x = y = 0} \\
    \frac{{xy}}{{x + y - xy}}  & \quad \text{otherwise} 
  \end{cases}
\$$

# II - Overlap functions
## OB (x,y)
<p align="center">$OB (x, y) = \min\{ x\sqrt{y}, y\sqrt{x}\}$ </p>

## Cuadras-Augé copula
<p align="center">$OmM (x, y) =  \min\{x,y\}\max\{x^2,y^2	\}$ </p>

## Oα (x, y)
<p align="center">$Oα (x, y) = xy(1 + α(1 − x)(1 − y)),  α ∈ [-1,1]$ </p>

## ODiv (x, y)
<p align="center">$ODiv (x, y) = \frac{{xy + \min\{x,y\}}}{{2}}$ </p>

## Geometric Mean
<p align="center">$GM (x, y) = \sqrt{xy}$ </p>

## Harmonic Mean
$$
\ HS (x, y) =
  \begin{cases}
    0       & \quad \text{if x = y = 0} \\
    \frac{{2}}{{ \frac{{1}}{{x}} +  \frac{{1}}{{y}}}}  & \quad \text{otherwise} 
  \end{cases}
\$$

## Sine
<p align="center">$Sine (x, y) = \frac{{\pi}}{{2}}(xy)^\frac{{1}}{{4}}$ </p>

## ORS
<p align="center">$ORS (x, y) = \min\{ \frac{{(x+1) \sqrt{y}}}{{2}}, y\sqrt{x}\}$ </p>

#  III - Copulas that are neither t-norms nor overlap functions
## CF (x, y)
<p align="center">$CF (x, y) = xy + x^2y(1-x)(1-y)$ </p>

## CL (x, y)
<p align="center">$CL (x, y) = \max\{\min\{x,\frac{{y}}{{2}}\},x+y+1\}$ </p>


# IV - Aggregation functions other than (I)-(III)

## FGL (x, y)
<p align="center">$FGL (x, y) = \sqrt{ \frac{{x(y+1)}}{{2}}}$ </p>

## FBPC (x, y)
<p align="center">$FBPC (x, y) = xy^2$ </p>

# V - Left 0-absorbent (0, 1)-pre-aggregation functions
## FNA (x, y)
$$
\ FNA (x, y) =
  \begin{cases}
    x       & \quad \text{if x ≤ y} \\
    \min\{(x, y)}  & \quad \text{otherwise} 
  \end{cases}
\$$

## FNA2 (x, y)


$$
\ FNA (x, y) =
  \begin{cases}
    x       & \quad \text{if x ≤ y} \\
    \frac{{x(y+1)}}{{2}} & \quad \text{0 < x ≤ y} \\
    \min\{(x, y)}  & \quad \text{otherwise} 
  \end{cases}
\$$
