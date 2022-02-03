# Teaching assistant ge-pde-ws2122

## Class of **Partial Differential Equations (PDE)** - WS 2021-2022
### Global exercises (GEs)
- **Hyperbolic systems** of **conservation laws**
- **Riemann**'s problems
- **Cauchy**'s problems
- **Shock** solution vs **Rarefaction** solution
- **Finite Volume Methods**
- Conservation form $u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(\widetilde{F}^{n}_{j-1/2} - \widetilde{F}^{n}_{j+1/2} \Big)$
- Consistent numerical flux function $\widetilde{F}^{n}_{j-1/2}\left(u^{n}_{j-1},u^{n}_{j}\right)$ and $\widetilde{F}^{n}_{j+1/2}\left(u^{n}_{j},u^{n}_{j+1}\right)$
- Numerical Analysis: **Lax** Equivalence Theorem: **Consistency** $+$ **Stability** $\Leftrightarrow$ **Convergence**
- Exact **Riemann** solver: **Godunov**'s scheme
- Approximate **Riemann**'s solvers: 
  - **Roe**'s solver 
  - Local **Lax-Friedrichs** (LLF) solver
  - **Harten-Lax-van Leer** (HLL) solver
- Structure of Finite Volume Method
  - **Monotone** $\rightarrow$ **$L_{1}$-Contraction** $\rightarrow$ **Total-Variation-Diminishing** (TVD) $\rightarrow$ **Monotonicity-Preserving**
- Nonlinear + higher order numerical scheme: 
  - TVD scheme 
  - **Harten** theorem

## Teaching assistant's extra materials and supplements

### Unnoted materials
- [x] [GE09](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-09.pdf) 
- [x] [GE10](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-10.pdf)
- [x] [GE11](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-11.pdf)
- [x] [GE12](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-12.pdf) 
- [x] [GE13](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-13.pdf) 
- [x] [GE14](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-14.pdf) 
- [x] [GE15](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-15.pdf) 
---
### Noted materials
- [x] [CW49/2021 $\rightarrow$ GE09-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-09.pdf) 
- [x] [CW50/2021 $\rightarrow$ GE10-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-10.pdf)
- [x] [CW51/2021 $\rightarrow$ GE11-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-11.pdf)
- [x] [CW02/2022 $\rightarrow$ GE12-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-12-noted.pdf) 
- [x] [CW03/2022 $\rightarrow$ GE13-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE13/ge-13-noted.pdf)
- [x] [CW04/2022 $\rightarrow$ GE14-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE13/ge-14-noted.pdf)
- [x] [CW05/2022 $\rightarrow$ GE15-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE13/ge-15-noted.pdf)