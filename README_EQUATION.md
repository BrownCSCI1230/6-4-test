# README-Test

> This is a testing ground for GitHub Markdown math support.
> 
> The font size is a little too small, as is the kerning between letters.
> 
> _I hope you're not claustrophobic!_
> 
> That said, it appears to work out-of-the-box, which is good.

## Collapsibility

<details>
  <summary>Click to expand!</summary>
  
  ### Reasons Why I Hate GitHub Markdown
  
  - there
  - is
  - no
  - one
  - reason
  - style, definitely style
  
  ### Reasons Why I Tolerate GitHub Markdown
  
  $$
    \text{Math works inside collapsible sections}
  $$
  
  So we can explain certain things in here, away from prying eyes.
  
</details>

## The Intersect Lighting Equation

$$ 
  I_λ = K_a O_{aλ} \\
    + \sum_{m=0}^{\text{numLights}-1} \left[ I_{mλ} \cdot (k_d O_{dλ} \hat{n}) \cdot \hat{L_m} \right]
$$

## The Ray Lighting Equation 

$$
  I_λ = K_a O_{aλ} + \\
    \sum_{i=1}^{m} f_{\text{att}} I_{λi} \\
      \left[ k_d O_{dλ} (\hat{n} \cdot \hat{L_i}) + k_s O_{sλ} (\hat{R_i} \cdot \hat{V})^n \right] \\
    + k_s O_{rλ} I_{rλ}
$$

It's incredibly stupid, but something is wrong with GitHub's math markdown parsing. In the big ray lighting equation above, if you change `\hat{L_i}` to `\hat{L}_i`, it'll break.

It works on its own (see below) so I'm not sure what's going on: 

- `\hat{L_i}`: $\hat{L_i}$
- `\hat{L}_i`: $\hat{L}_i$

## Attenuation

Multiply the contribution of a point light to a surface by $f_{\text{att}}$, where:

$$
  f_{\text{att}} = \min \\
    \left( \\
      \frac{1}{c_\text{constant} + d \cdot c_{\text{linear}} + d^2 \cdot c_{\text{quadratic}}} \\
      , \\
      1 \\
    \right)
$$

## Gradients via Convolution w/ Sobel Filters

$$
  G_x = \begin{bmatrix}
    -1 & 0 & 1 \\
    -2 & 0 & 2 \\
    -1 & 0 & 1 
    \end{bmatrix} \ast A
$$

$$
  G_y = \begin{bmatrix}
    -1 & -2 & -1 \\
    0 & 0 & 0 \\
    1 & 2 & 1 
    \end{bmatrix} \ast A
$$

$$
  G = \sqrt{G_x^2 + G_y^2}
$$

## Convolution and Derivation are Commutative and Associative

$$
  \frac{\partial}{\partial x} \left( I * G \right) \\
    = \frac{\partial}{\partial x} I * G \\
    = I * \frac{\partial}{\partial x} G
$$

## Sobel Filters are Separable

$$
  G_x = \begin{bmatrix}
    1 \\
    2 \\
    1 
    \end{bmatrix} \\
    \ast \\
    \left( \\
    \begin{bmatrix}
    -1 & 0 & 1
    \end{bmatrix} \\
    \ast A \right)
$$

$$
  G_y = \begin{bmatrix}
    1 \\
    0 \\
    -1 
    \end{bmatrix} \\
    \ast \\
    \left( \\
    \begin{bmatrix}
    1 & 2 & 1
    \end{bmatrix} \\
    \ast A \right)
$$

## Why Are We Still Here?

Just to suffer?

$$
  F(u,v) = \sum_{x=0}^{M-1} \sum_{y=0}^{N-1} f(x,y) \\
    e^{-2 \pi i (\frac{ux}{M} + \frac{vy}{N})}
$$

Every night, I can feel my leg... and my arm... even my fingers.

$$
  f(x,y) = \frac{1}{MN} \\
    \sum_{u=0}^{M-1} \sum_{v=0}^{N-1} F(u,v) \\
    e^{2 \pi i (\frac{ux}{M} + \frac{vy}{N})}
$$

The body I’ve lost... the comrades I’ve lost... won’t stop hurting...

$$
  F(u,v) = \sum_{x=0}^{M-1} \\
    \left[ \\
      e^{-2 \pi i u x / M} \\
      \sum_{y=0}^{N-1} f(x,y) \\
        e^{-2 \pi i v y / N} \\
    \right]
$$

It’s like they’re all still there. You feel it, too, don't you?

$$
  f(x,y) = \frac{1}{MN} \\
    \sum_{u=0}^{M-1} \\
      \left[ \\
        e^{2 \pi i u x / M} \\
        \sum_{v=0}^{N-1} F(u,v) \\
          e^{2 \pi i v y / N} \\
      \right]
$$



