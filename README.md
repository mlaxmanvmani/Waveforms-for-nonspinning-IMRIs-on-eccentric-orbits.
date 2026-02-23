## 5PN eccentric gravitational waveforms for IMRIs on inspiralling orbits. 

### The hybrid phasing and mode amplitude results are computed through 5PN and $e^{10}$ order in eccentricty.

This supplemental file contains the complete results which are partially presented in the paper.
It contains expression for

* Phasing inputs: time eccentricity, energy flux, orbital energy and its derivative.
* Phasing results: TaylorT2 phase, TaylorT2 time and TaylorF2 SPA phase. 
* Mode amplitudes: $H\ell m$ mode amplitudes up to $\ell=m=12$.
* PN evolution equation: $de/dt$, $dv/dt$, $de/dt$, true anomaly, mean motion and periastron precession.

Note: The phasing inputs and phasing results are computed in terms of PN parameters $v$, $v_0$ and $e_0$, where $e_0$ is the initial eccentricity defined at an intial frequency related parameter $v_0$, whereas the mode amplitudes and PN evolution equations are computed in terms $v$, time eccentricity $e_t$ and phase angles $l$ and $\xi$.

Also, note that the expression for time eccentrcity ($e_t$) in the supplemental material is given in the eccentricity expanded format, whereas in the paper we followed the format of [Moore et al, 2016](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.93.124061) for the leading order eccentricity expression.   
### Loading the supplemental file
The .m text file can be loaded into a Mathematica notebook using the built-in `Get` command.
  
All the expressions are stored in the following format:

`EnergyFlux[vpow,epow]`, `Energy[vpow,epow]`...etc

where,

- vpow : Power of the post-Newtonian (PN) expansion parameter $(v)$  
- epow : Power of the eccentricity expansion parameter ($e$ or $e_0$)

### Example

A 1PN accurate expression for energy flux can be obtained as 

`EnergyFlux = (EnergyFlux[0,0] + EnergyFlux[2,0]) + (EnergyFlux[0,2] + EnergyFlux[2,2])`

Note: We have used two symbols for PN parameters in phasing and mode results which can be replaced as:

`v0byv -> v0/v` and `ebyei -> et/ei`


where, $ei$ is some initial eccentricity defined in the DC modes computation of hereditary integrals (see Ref. [Ebersold et al](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.100.084043])). 
