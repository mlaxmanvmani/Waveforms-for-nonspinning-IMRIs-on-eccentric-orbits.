## 5PN eccentric gravitational waveforms for IMRIs on inspiralling orbits. 

### The hybrid phasing and mode amplitude results are computed through 5PN and e<sup>10</sup> order in eccentricty.

This supplemental file contains the complete results which were partially presented in the paper.
It contains expression for

* Phasing inputs: time eccentricity, energy flux, orbital energy and its derivative.
* Phasing results: TaylorT2 phase, TaylorT2 time and TaylorF2 SPA phase. 
* Mode amplitudes: Hlm mode amplitudes up to l=m=12.
* PN evolution equation: de/dt, dv/dt and de/dt.

Note: The phasing inputs and phasing results are computed in terms of PN parameters v, v0 and e0, while the mode amplitudes and PN evolution equations are computed in terms v and time eccentricity et.

### Loading the supplemental file
The .m text file can be loaded into a Mathematica notebook simply using the in built "Get" command.
  
All the expressions are stored in the following format:

`EnergyFlux[vpow,epow]`, `Energy[vpow,epow]`...etc

where,

- vpow : Power of the post-Newtonian (PN) expansion parameter \( v \)  
- epow : Power of the eccentricity expansion parameter \( e or e<sub>0</sub>\)

### Example

A 1PN accurate expression for energy flux can be obtained as 

`EnergyFlux = (EnergyFlux[0,0] + EnergyFlux[2,0]) + (EnergyFlux[0,2] + EnergyFlux[2,2])`

Note: We have used two symbols for PN parameters in phasing and mode results which can be replaced as:

`v0byv -> v0/v` and `ebyei -> et/ei`


where, ei is some initial eccentricity defined in the DC modes computation of hereditary integrals (see Ref. [Ebersold et al](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.100.084043])). 


