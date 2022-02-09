# Teaching assistant ge-pde-ws2122

## Class of **Numerical methods for Partial Differential Equations (NumPDE)** - WS 2021-2022
### Global exercises (GEs): GE09-GE10-GE11-GE12-GE13-GE14-GE15-GE15e
- Linear ![](./eqns/plus_w.svg#gh-dark-mode-only) ![](./eqns/plus_b.svg#gh-light-mode-only)  Nonlinear **Hyperbolic systems** of **conservation laws**
- **Cauchy**'s problems
- **Riemann**'s problems
- Linear scalar advection equation
- Nonlinear viscous **Burgers**' ![](./eqns/plus_w.svg#gh-dark-mode-only) ![](./eqns/plus_b.svg#gh-light-mode-only) inviscid **Burgers**' equations
- Hyperbolic systems of first order PDE: 
  - (strictly) hyperbolicity: disctinct eigenvalues
  - diagonalizable matrix ![](./eqns/ARLR_w.svg#gh-dark-mode-only) ![](./eqns/ARLR_b.svg#gh-light-mode-only) 
  - Decomposition of system of first order PDEs into separated first order PDEs
- **Shock** solution vs **Rarefaction** solution
- **Finite Volume Methods**
- Conservation form 
  <p align="center">
    <!-- <img src="https://latex.codecogs.com/svg.image?\bg_black&space;\inline&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(\widetilde{F}^{n}_{j-1/2}&space;-&space;\widetilde{F}^{n}_{j&plus;1/2}&space;\Big)" title="\bg_black \inline u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(\widetilde{F}^{n}_{j-1/2} - \widetilde{F}^{n}_{j+1/2} \Big)" />
    <img src="https://latex.codecogs.com/svg.image?\bg_white&space;\inline&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(\widetilde{F}^{n}_{j-1/2}&space;-&space;\widetilde{F}^{n}_{j&plus;1/2}&space;\Big)" title="\bg_white \inline u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(\widetilde{F}^{n}_{j-1/2} - \widetilde{F}^{n}_{j+1/2} \Big)#gh-dark-mode-only" /> -->
    <!-- <img src="https://latex.codecogs.com/svg.image?\inline&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(\widetilde{F}^{n}_{j-1/2}&space;-&space;\widetilde{F}^{n}_{j&plus;1/2}&space;\Big)" title="\inline u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(\widetilde{F}^{n}_{j-1/2} - \widetilde{F}^{n}_{j+1/2} \Big" />
    <img src="https://latex.codecogs.com/svg.image?\dpi{100}&space;\inline&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(\widetilde{F}^{n}_{j-1/2}&space;-&space;\widetilde{F}^{n}_{j&plus;1/2}&space;\Big)" title="\inline u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(\widetilde{F}^{n}_{j-1/2} - \widetilde{F}^{n}_{j+1/2} \Big)" /> -->
  </p>
  
   <!-- ![](./eqns/cunda.svg#gh-dark-mode-only)

   ![](./eqns/cunli.svg#gh-light-mode-only)

   ![](./eqns/cunno1.svg#gh-dark-mode-only) -->

   <!-- <img src="https://latex.codecogs.com/svg.image?\color[rgb]{1,1,1}{1&plus;cundark}#gh-dark-mode-only" title="\color[rgb]{1,1,1}{1+cundark}" />

   <img src="https://latex.codecogs.com/svg.image?\color[rgb]{0,0,0}{1&plus;cunwhite}#gh-light-mode-only" title="\color[rgb]{0,0,0}{1+cunwhite}" /> -->

<!-- <p align="center">
  <img src="https://raw.githubusercontent.com/GiorgosXou/Random-stuff/main/StackOverflow/Answers/70200610_11465149/b.png#gh-light-mode-only" height="120" width="120"/>
  <img src="https://raw.githubusercontent.com/GiorgosXou/Random-stuff/main/StackOverflow/Answers/70200610_11465149/w.png#gh-light-mode-only" height="120" width="120"/>
</p> -->

- Consistent numerical flux function 
  <!-- <p align="center">
    <img src="https://latex.codecogs.com/gif.image?\dpi{80}&space;\bg_white&space;\inline&space;\widetilde{F}^{n}_{j-1/2}\left(u^{n}_{j-1},u^{n}_{j}\right)" title="\bg_white \inline \widetilde{F}^{n}_{j-1/2}\left(u^{n}_{j-1},u^{n}_{j}\right)" /> and <img src="https://latex.codecogs.com/gif.image?\dpi{80}&space;\bg_white&space;\inline&space;\widetilde{F}^{n}_{j&plus;1/2}\left(u^{n}_{j},u^{n}_{j&plus;1}\right)" title="\bg_white \inline \widetilde{F}^{n}_{j+1/2}\left(u^{n}_{j},u^{n}_{j\+1}\right)" />
  </p> -->
- Upwind-to-the-left (UWL): 
  <!-- <img src="https://latex.codecogs.com/gif.image?\dpi{80}&space;\bg_white&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&plus;\frac{\Delta&space;t}{\Delta&space;x}\Big(f(u^{n}_{j-1})&space;-&space;f(u^{n}_{j})\Big)" title="\bg_white u^{n+1}_{j} = u^{n}_{j}+\frac{\Delta t}{\Delta x}\Big(f(u^{n}_{j-1}) - f(u^{n}_{j})\Big)" /> -->
- Upwind-to-the-right (UWR): 
  <!-- <img src="https://latex.codecogs.com/gif.image?\dpi{80}&space;\bg_white&space;u^{n&plus;1}_{j}&space;=&space;u^{n}_{j}&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(f(u^{n}_{j})&space;-&space;f(u^{n}_{j&plus;1})\Big)" title="\bg_white u^{n+1}_{j} = u^{n}_{j} + \frac{\Delta t}{\Delta x}\Big(f(u^{n}_{j}) - f(u^{n}_{j+1})\Big)" /> -->
- **Lax-Friedrichs** (LF): 
  <!-- <img src="https://latex.codecogs.com/gif.image?\dpi{80}&space;\bg_white&space;u^{n&plus;1}_{j}&space;=&space;\frac{1}{2}\Big(&space;u^{n}_{j-1}&space;&plus;&space;u^{n}_{j&plus;1}&space;\Big)&space;&plus;&space;\frac{\Delta&space;t}{\Delta&space;x}\Big(f(u^{n}_{j-1})-f(u^{n}_{j&plus;1})\Big)" title="\bg_white u^{n+1}_{j} = \frac{1}{2}\Big( u^{n}_{j-1} + u^{n}_{j+1} \Big) + \frac{\Delta t}{\Delta x}\Big(f(u^{n}_{j-1})-f(u^{n}_{j+1})\Big)" /> -->
- **Lax-Wendroff** (LW)
- Numerical Analysis: **Lax** Equivalence Theorem: 
  **Consistency** ![](./eqns/plus_w.svg#gh-dark-mode-only) ![](./eqns/plus_b.svg#gh-light-mode-only) **Stability** ![](./eqns/LRarrow_w.svg#gh-dark-mode-only) ![](./eqns/LRarrow_b.svg#gh-light-mode-only)  **Convergence**
  - Nonlinear numerical methods
  - Non-oscillatory behaviours of higher order numerical methods
- Exact **Riemann** solver: **Godunov**'s scheme
- Approximate **Riemann**'s solvers: 
  - **Roe**'s solver 
  - Local **Lax-Friedrichs** (LLF) solver
  - **Harten-Lax-van Leer** (HLL) solver
- Structure of Finite Volume Method
  - **Monotone** ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) ![](./eqns/L1_w.svg#gh-dark-mode-only) ![](./eqns/L1_b.svg#gh-light-mode-only)-**Contraction** ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) **Total-Variation-Diminishing** (TVD) ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) **Monotonicity-Preserving**
- Nonlinear + higher order numerical scheme: 
  - **Harten** theorem
  - Incremental form
  - TVD scheme
- A bit insight into **Godunov**'s solver with graphical explanations

<!-- <img src="https://render.githubusercontent.com/render/math?math=%5Cbbox%5Bwhite%5D%7B%5Clarge%5Cf(x)=sin(x)%7D"> 

<img src="https://render.githubusercontent.com/render/math?math=\bbox[white]\displaystyle\sum_{n=0}^\infty\frac{1}{2^n}">

- <img src="https://latex.codecogs.com/gif.latex?O_t=\text { Onset event at time bin } t " > 
- <img src="https://latex.codecogs.com/gif.latex?s=\text { sensor reading }" > 
- <img src="https://latex.codecogs.com/gif.latex?P(s | O_t )=\text { Probability of a sensor reading value when sleep onset is observed at a time bin } t" >
-->
 
## Teaching assistant's extra materials and supplements

### Unnoted materials

#TODO

- [x] [GE09](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-09.pdf) 
- [x] [GE10](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE10/ge-10.pdf)
- [x] [GE11](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE11/ge-11.pdf)
- [x] [GE12](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-12.pdf) 
- [x] [GE13](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE13/ge-13.pdf) 
- [x] [GE14](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE14/ge-14.pdf) 
- [x] [GE15](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE15/ge-15.pdf) 
- [x] [GE15e](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE15e/ge-15e.pdf) 
---
### Noted materials

#TODO

- [x] CW49/2021 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE09-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE09/ge-09.pdf)
- [x] CW50/2021 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE10-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE10/ge-10.pdf)
- [x] CW51/2021 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE11-offline](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE11/ge-11.pdf)
- [x] CW02/2022 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE12-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE12/ge-12-noted.pdf) 
- [x] CW03/2022 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE13-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE13/ge-13-noted.pdf)
- [x] CW04/2022 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE14-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE14/ge-14-noted.pdf)
- [x] CW05/2022 ![](./eqns/rightarrow_w.svg#gh-dark-mode-only) ![](./eqns/rightarrow_b.svg#gh-light-mode-only) [GE15-noted-online](https://github.com/tuanvo-git/ge-pde-ws2122/blob/main/GE15/ge-15-noted.pdf)
