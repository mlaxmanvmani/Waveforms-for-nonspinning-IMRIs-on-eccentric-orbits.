## 5PN eccentric waveforms for intermediate-mass-ratio-inspirals (IMRIs) from post-Newtonian and black hole perturbation theory 

The supplemental file ([name of the file]) lists Gravitational Wave Phasing (Taylor approxinants) and Amplitude (spherical harmonic modes) computed through 5PN order and to $10^{\rm th}$ in the eccentricity parameter. Inputs required to arrive at the final results are also included. More specifically,   

* Evolution of time-eccentricity: $e_t(v, v_0, e_0)$, where $v$ is a frequency dependent PN parameter and $e_0$ refers to a reference eccentricity evaluated at a reference frequency ($v_0$).
* EnergyFlux, Energy and its derivative ($dE/dv$) in terms of $v, v_0, e_0$.
* Phasing: TaylorT2, TaylorF2 as explicit functions of $v, v_0, e_0$.
* Amplitude: $H^{\ell m}$ with $2\leq\ell\leq12$ and $0\leq|m|\leq12$ in terms of the time-eccentricity ($e_t$), the PN parameter ($v$) and an angle $\xi$ related to mean-anomaly.
* Orbit averaged evolution equations for the time-eccentricity ($e_t$) and the PN parameter ($v$): $de/dt$, $dv/dt$, $de/dt$ in terms of the time-eccentricity ($e_t$), the PN parameter ($v$).
* Other orbital elements: true anomaly($\nu$), mean motion ($n$) and the constant $k$ characterising orbital precession as a function of the time-eccentricity ($e_t$), the PN parameter ($v$). 

NOTE: The time-eccentrcity ($e_t$) is written in a form that is fully expanded in eccentricity, whereas the preprint ([arXiv reference]) follows the format of [Moore et al, 2016](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.93.124061).   
### Loading the supplemental file
The .m text file can be loaded into a Mathematica notebook using the built-in `Get` command.
  
All the expressions are stored in the following format:

`EnergyFlux[vpow,epow]`, `Energy[vpow,epow]`...etc

where,

- vpow : Power of the post-Newtonian (PN) expansion parameter $(v)$  
- epow : Power of the eccentricity expansion parameter ($e_t$ or $e_0$)

### Example

A 1PN accurate expression for energy flux can be obtained as 

`EnergyFlux = (EnergyFlux[0,0] + EnergyFlux[2,0]) + (EnergyFlux[0,2] + EnergyFlux[2,2])`

Note: We have used two symbols for PN parameters in phasing and mode results which can be replaced as:

`v0byv -> v_0/v` and `ebyei -> et/e_i`


where, $e_i$ is another reference eccentricity that appears in the computation of memory integrals leading to zero frequency ($m=0$ modes) contributions; see for instance, Ref. [Ebersold et al](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.100.084043]). 
