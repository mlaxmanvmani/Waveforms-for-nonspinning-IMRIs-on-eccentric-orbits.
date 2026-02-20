## 5PN eccentric gravitational waveforms for IMRIs on inspiralling orbits. 

### The hybrid phasing and mode amplitude results are computed through 5PN and e<sup>10</sup> order in eccentricty.

This supplemental file contains the complete results which were partially presented in the paper.
It contains expression for

* Phasing inputs: time eccentricity evolution (et), energy flux (F), energy (E) and its derivative (dE/dv).
* Phasing results: TaylorT2 phase and time evolution and TaylorF2 SPA phase. 
* Mode amplitudes: H<sup>lm</sup> mode amplitudes up to l=m=12.
* PN evolution equation: de/dt, dv/dt and de/dt.

Note: The phasing inputs and phasing results are computed in terms of PN parameters v, v0 and e0, while the mode amplitudes and PN evolution equations are computed in terms v and time eccentricity et.     
  
All the expressions are stored in the following format:

`FHybrid[vpow,epow]`, `EnHybrid[vpow,epow]`...etc

where,

- vpow : Power of the post-Newtonian (PN) expansion parameter \( v \)  
- epow : Power of the eccentricity expansion parameter \( e or e<sub>0</sub>\)

### Example

A 1PN accurate expression for energy flux can be obtained as 

`FHybrid = (FHybrid[0,0] + FHybrid[2,0]) + (FHybrid[0,2] + FHybrid[2,2])`

and then replacing "FcircNewt" with appropriate Newtonian factor. All the relevant Newtonian factor for different physical quantities are given in the paper.

Note: We have used two symbols for PN parameters in phasing and mode results which can be replaced as:

`v0byv -> v0/v` and `ebyei -> et/ei`


where, ei is some initial eccentricity defined in the DC modes computation of hereditary integrals (see Ref. [Ebersold et al](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.100.084043])). 


