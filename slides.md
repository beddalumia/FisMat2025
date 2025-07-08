---
colorSchema: light
color: rose
layout: cover
routerMode: hash
title: FisMat2025
theme: neversink
neversink_slug: "FisMat2025"
---

# Symmetry resolved `entanglement` in the _2d_ Hubbard model

Contributed talk by **Gabriele Bellomia**    
Postdoc at SISSA - _Strongly Correlated Electrons_   

<br />
    
<img src=/images/sissalight.svg width=110 class="float-right mr-10 mb-5">

:: note ::
Workshop **"Taming the interplay of spin and charge in unconventional superconductors"**  
**FisMat2025** --- July 7<sup>th</sup>, Venice --- _Moderated by Claudio Giannetti and Massimo Capone_

<!-- 
### Abstract
Recent experimental and theoretical advances have opened new perspectives on the characterization of strongly correlated electrons, adding a new layer of understanding in terms of concepts and tools borrowed from quantum information theory. We join the effort by investigating, within cluster dynamical mean-field theory (CDMFT), the local and quasilocal (short-range) quantum information content of salient landmarks in the phase diagram of the two-dimensional Hubbard model on the square lattice, relevant to the physics of unconventional superconductivity in copper oxides. In particular, I will discuss the behavior of symmetry-resolved measures of entanglement and correlation shared by pairs of electronic orbitals, spatially separated within clusters embedded in the two-dimensional Hubbard lattice. The symmetry resolution of our entanglement measures, complemented with the restrictions imposed by fermionic superselection rules, allow for a clear identification of Mottness, both in the half-filled insulator and in the strongly correlated metal found at small hole-doping fractions: a significant holon-doublon entanglement is manifested only in the vicinity of the Mott transition lines, while spatial spin singlets dominate the entanglement content of both the strongly-localized Mott insulator and the optimally doped metal. Remarkably, all contributions to the symmetry-resolved two-site entanglement are suppressed by several orders of magnitude in the Fermi liquid regime found at either weak interaction strengths or large doping fractions. Our results provide a formal basis for early proposals of an RVB mechanism underlying the physics of unconventional superconductivity, through a clean scrutiny of the contributions associated to charge-fluctuating and spin-singlet Bell pairs. -->


---
layout: image-right
image: /images/armitage_quanta.jpg
neversink_slug: Kristina Armitage for Quanta Magazine
---


# Why entanglement?

Many-body entanglement has proven to

<v-clicks at="+1">

- be a central tool in statistical physics
- mark states of high quantum complexity

  
</v-clicks>

<v-clicks>

It is also expected to be a **resource for quantum technologies**, provided that

</v-clicks>

<v-clicks at="+1">

- it is operationally accessible
- it goes beyond classical simulation

  
</v-clicks>

---
layout: default
---

# Why symmetry resolved?

<br />

<div class="neversink-pink-light-scheme ns-c-bind-scheme"> 
&nbsp; Operationally accessible entanglement: parity superselection rule (P-SSR)
</div>  
  <v-clicks>

  - Fundamental rule of quantum mechanics :   
    -> No superpositions of states with different parity of the electron number<sup>1</sup>   
  - It surely applies to the full state   
    -> operationally applies also to local operations<sup>2</sup>
  - Even stronger arguments for the local P-SSR:   
    -> It is needed by the no-signaling theorem<sup>3</sup>    
    -> It is required for mathematical consistency<sup>4</sup>    
    -> It ensures robustness against time evolution<sup>5</sup>  

  </v-clicks>


<hr>    


<kbd v-click="1"> <sup>1</sup> Wick _et al._, *The Intrinsic Parity of Elementary Particles*, Physical Review **88**, 101 (1952) </kbd>  
<kbd v-click="2"> <sup>2</sup> Ding _et al._, _Physical entanglement between localized orbitals_, Quantum Sci. and Tech. **9**, 015005 (2023) </kbd>  
<kbd v-click="3"> <sup>3</sup> Friis, _Reasonable fermionic quantum information theories require relativity_, New J. Phys. **18**, 033014 (2016) </kbd>  
<kbd v-click="3"> <sup>4</sup> Szalay _et al._, _Fermionic systems for quantum information people_, J. Phys. A: Math. Theor. **54**, 393001 (2021) </kbd>  
<kbd v-click="3"> <sup>5</sup> Parez _et al._, _The Fate of Entanglement_, arXiv:2402.06677 (2024) [submitted to SciPost Physics]</kbd>


---
layout: default
transition: slide-up
---

# Why symmetry resolved?

<br />

<div class="neversink-pink-light-scheme ns-c-bind-scheme"> 
&nbsp; Operationally accessible entanglement: parity superselection rule (P-SSR)
</div>  

&nbsp; <kbd>[...]</kbd>

<div class="neversink-sky-light-scheme ns-c-bind-scheme"> 
&nbsp; Removing trivial entanglement from charge fluctuations: Charge Super-Selection Rule (N-SSR) 
</div> 

<v-clicks>

- We expect a noninteracting metal to be very entangled in real space   
- But in momentum space it is trivially solved with Slater determinants!   
- At weak coupling it is well approximated by Hartree-Fock theory    

</v-clicks>  

<v-clicks>

&nbsp;&nbsp;&nbsp; -> Such real-space entanglement can be **simulated with a simple classical algorithm**   

&nbsp;&nbsp;&nbsp; -> ==Arguably not relevant for quantum technologies!==

<AdmonitionType type="tip" title="Idea" width="450px" v-drag="[495,432,450,73]">
Removing all charge superpositions, we may uncover nontrivial real-space entanglement (if any!)
</AdmonitionType>

</v-clicks>


---
layout: default
transition: view-transition
---


<div class="neversink-emerald-scheme ns-c-bind-scheme"> 


# &nbsp; Symmetries of a Hubbard dimer (in a mixed state) 
</div>

<div class="grid w-full h-fit grid-cols-5 grid-rows-2 mt-10 mb-auto">

  <div class="grid-item grid-col-span-3"><img src="/images/dimer_rdm.svg" class="h-full w-auto mr-2" /></div>
  
  <div class="grid-item grid-col-span-2 ml-7"> 

  <v-clicks>

  - The Hubbard model conserves the charge $N$ (and magnetization $m$)
  - Of course this does not imply a local conservation of $n_i$ and $n_j$
  - So in general we have quantum superpositions (off-diagonals)    
    ==**->** entanglement between $i$ and $j$==
    <div class="flex justify-center my-4">
    <img src="/images/dimer_entangled.svg" width="200" />
    </div>

  </v-clicks></div>

  <div class="grid-item grid-col-span-3 text-center h-fit">

  <kbd> Adapted from: Ding _et al._, J. Chem. Theory Comput. **17**, 1, 79–95 (2021) </kbd>

  </div>
</div>

---


<div class="neversink-emerald-scheme ns-c-bind-scheme"> 

# &nbsp; Symmetries of a Hubbard dimer (in a mixed state) 

</div>

<div class="grid w-full h-fit grid-cols-4 grid-rows-1 mt-10 mb-auto">

  <div class="grid-item grid-col-span-2 h-91"><img src="/images/dimer_sym.svg" class="h-full w-auto ml-5 " />   
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <kbd> Rotated to highlight single-site symmetries  </kbd></div>

  <div class="grid-item grid-col-span-2 ml-7"> 

  - So in general we have quantum superpositions (off-diagonals)    
    ==**->** entanglement between $i$ and $j$==
    <div class="flex justify-left my-4 ml-17 ">
    <img src="/images/dimer_entangled.svg" width="150" />
    </div>  

  <v-clicks depth=2>

  - But **local** SSRs inhibit all quantum superpositions except:
    - holon-doublon coupling   
      ${\color{#F43F5E}\rho_{_\mathrm{hd}} \!\!=\, \mid \uparrow\downarrow \rangle\langle \bullet\!\mid \otimes \mid\!\bullet \rangle\langle \uparrow\downarrow \mid}$ 
    - antiferro fluctuations  
      ${\color{DeepSkyBlue}\rho_{_{\uparrow\downarrow}} \!\!=\, \mid \uparrow \rangle\langle \downarrow \mid \otimes \mid\downarrow\rangle\langle \uparrow\mid}$ 

  </v-clicks></div>

</div>

---
layout: section
color: rose
title: Results
---

# Results from Cluster-DMFT


Across both the `interaction-driven` and `density-driven` Mott transitions

---
layout: full
color: white
title: CDMFT
---

<div class="neversink-rose-scheme ns-c-bind-scheme"> 

# &nbsp; Cluster Dynamical Mean-Field Theory at zero temperature

</div>

<div class="grid w-full h-fit grid-cols-3 grid-rows-2 mt-20 mb-auto">
<div v-click=1 class="grid-item grid-col-span-1"><img src="/images/cdmft.svg" /></div>
<div v-click=2 class="grid-item grid-col-span-1"><img src="/images/cdmft_bath.svg" /></div>
<div v-click=3 class="grid-item grid-col-span-1"><img src="/images/cdmft_ed.svg" /></div>

<div v-click=1 class="grid-item grid-col-span-1 text-center h-fit m-3">   
<hr/>

We tile the lattice in real space

</div> 

<div v-click=2 class="grid-item grid-col-span-1 text-center h-fit m-3">   
<hr/>

Then map to an impurity model

</div>

<div v-click=3 class="grid-item grid-col-span-1 text-center h-fit m-3">   
<hr/>

&nbsp; Finally we discretize the bath

</div>

</div>


---
layout: full
title: MIT
transition: slide-left
---

<div class="neversink-rose-scheme ns-c-bind-scheme"> 

# &nbsp; Interaction-driven paramagnetic MIT

</div>

<div class="grid w-full h-fit grid-cols-3 grid-rows-1 mt-7 mb-auto">
<div class="grid-item grid-col-span-2 mb-3"><img src="/images/half_sym.svg" width=700/></div>
<div class="grid-item grid-col-span-1 text-center">
<v-click at=0>

<img src="/images/4x2_ladder.svg" class="w-50 ml-15 mt-0.5" />
<img src="/images/shells_inkscaped.svg" class="w-150 ml-3 mt-5 mb-5" />

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; <kbd> G.Bellomia _et al._, PRB **109**, 115104 </kbd>

</v-click>
</div>
<div class="grid-item grid-col-span-2 text-center h-fit">

<hr/>

Symmetry-resolved versus full entanglement between sites $\langle i j \rangle$

</div>
</div>



---
layout: full
title: Doping
transition: slide-up
---

<div class="neversink-rose-scheme ns-c-bind-scheme"> 

# &nbsp; Doping-driven delocalization

</div>

<div class="grid w-full h-fit grid-cols-3 grid-rows-1 mt-7 mb-auto">
<div class="grid-item grid-col-span-2 mb-4.5"><img src="/images/doped_sym.svg" width=700/></div>
<div class="grid-item grid-col-span-1 ml-15">
<v-clicks at=0>

  - We dope the Mott insulator found at $U/D=2.3$
  - Both $E_{\langle ij \rangle}^\mathrm{hd}$ and $E_{\langle ij \rangle}^{\uparrow\downarrow}$ decrease in the bad metal up to $\delta\simeq0.2$
  - The spin-singlet $E_{\langle ij \rangle}^{\uparrow\downarrow}$ vanishes in the normal Fermi liquid, while there is some residual $E_{\langle ij \rangle}^\mathrm{hd}$...

</v-clicks>
</div>
<div class="grid-item grid-col-span-2 text-center h-fit">

<hr/>

Symmetry-resolved versus full entanglement between sites $\langle i j \rangle$

</div>
</div>

---
layout: full
title: Phase Diagram
color: slate-light
---

<div class="neversink-slate-scheme ns-c-bind-scheme"> 

# &nbsp; $(U\text{-}\mu)$ phase diagram in $E_{\langle ij \rangle}^\mathrm{hd}$ and $E_{\langle ij \rangle}^{\uparrow\downarrow}$

</div>

<div class="grid w-full h-fit grid-cols-2 grid-rows-1 mt-10 mb-auto">
<div class="grid-item grid-col-span-1"><img src="/images/HDphases.svg" class="w-80 ml-15"/></div>
<div class="grid-item grid-col-span-1"><img src="/images/RVBphases.svg" class="w-80 ml-15" /></div>

</div>




---
layout: iframe-right
title: Advertisement
url: 
slide_info: true
transition: view-transition
---

# Experimental measures?

<br/>

<v-click>

  Unfortunately hard to directly access it...

  <br/>  

</v-click>

<v-click>

  We **just announced on arxiv** an indirect witness of nonlocal quantum correlations  

</v-click>

<v-click>

  ==**->** Easily measured in cold-atom lattices== 

</v-click>
  
<v-click>

  ==**->** Directly accessible in local theories== 

  <br/>

</v-click>


---
layout: iframe-right
title: Web-View
url: https://arxiv.org/html/2506.18709v1#abstract
slide_info: false
---

# Experimental measures?

<br/>



  Unfortunately hard to directly access it...

  <br/>  





  We **just announced on arxiv** an indirect witness of nonlocal quantum correlations  





  ==**->** Easily measured in cold-atom lattices== 



  ==**->** Directly accessible in local theories== 

  <br/>



  Please read it, if interested! 🤠
  <QRCode value="https://arxiv.org/abs/2506.18709" :size="100" render-as='svg' class="float-right mr-7 mt-2"/>


---
layout: image
image: /images/Venice.jpg
slide_info: false
---
