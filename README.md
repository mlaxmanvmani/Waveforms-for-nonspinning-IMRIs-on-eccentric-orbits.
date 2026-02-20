## 5PN eccentric gravitational waveforms for IMRIs on inspiralling orbits. 

### The phasing and mode amplitude results are computed through 5PN and e<sup>10</sup> order in eccentricty.

The supplemental file contains first the expressions for the phasing inputs which are eccentricity evolution (e<sub>t</sub>), energy flux (F), energy (E) and its derivative (dE/dv) in terms of parameters v, v0, and e0.

Then it has 

All the relevant quantities are stored in the following format:


`FHybrid[vpow,epow]`, `EnHybrid[vpow,epow]`...etc

where,

- vpow : Power of the post-Newtonian (PN) expansion parameter \( v \)  
- epow : Power of the eccentricity expansion parameter \( e or e<sub>0</sub>\)

### Example

FHybrid\[2,6\] represents the \(v<sup>2</sup> e<sup>6</sup>\) term multiplied with the appropriate newtonian factor.

Note: We have used two symbols for phasing and mode results which can be replaced as:

`v0byv -> v0/v` and `ebyei -> et/ei`


where, et is the time eccentricity and ei is some initial eccentricity defined in the computation of hereditary integrals of Ref. [Ebersold et al](https://journals.aps.org/prd/pdf/10.1103/PhysRevD.100.084043]). 


