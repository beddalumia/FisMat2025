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

&nbsp;&nbsp;&nbsp; -> Such real-space entanglement can be **simulated with a trivial classical algorithm**   

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
---

# Results from Cluster-DMFT


Across both the `interaction-driven` and `density-driven` Mott transitions

---
layout: full
color: white
title: Results
---

<div class="neversink-rose-scheme ns-c-bind-scheme"> 

# &nbsp; Interaction-driven paramagnetic MIT

</div>
<br/>

&nbsp; Cluster Dynamical Mean-Field Theory at zero temperature:

<div class="grid w-full h-fit grid-cols-3 grid-rows-2 mt-5 mb-auto">
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
title: Full Layout - 2 Col Fig
---

<div class="neversink-rose-scheme ns-c-bind-scheme"> 

# &nbsp; Interaction-driven paramagnetic MIT

</div>
<br/>

&nbsp; Cluster Dynamical Mean-Field Theory at zero temperature:

<div class="grid w-full h-fit grid-cols-3 grid-rows-2 mt-10 mb-auto">
<div class="grid-item grid-col-span-2"><img src="/images/armitage_quanta.jpg" width=200/></div>
<div class="grid-item grid-col-span-1"><img src="/images/armitage_quanta.jpg" width=250/></div>
<div class="grid-item grid-col-span-2 text-center h-fit">

**Figure show this**: this is a two column figure

</div>
</div>



---
layout: credits
color: navy
speed: 1.0
loop: true
---

<div class="grid text-size-4 grid-cols-3 w-3/4 gap-y-10 auto-rows-min ml-auto mr-auto">
<div class="grid-item text-center mr-0- col-span-3">
  
  This one has `speed: 4.0` and `loop: true` in the front matter
</div>
<div class="grid-item text-center mr-0- col-span-3">
  <strong>Cast</strong><br> 
  <span class="font-size-3 mt-0">(In order of appearance)</span>
</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Study 1</strong></div>
<div class="grid-item col-span-2">Person 1 <i>as PhD student</i>&nbsp;<mdi-open-in-new class="font-size-3 mb-0.5" /><br/>Person 2 <i>as Co-PI</i>&nbsp;<mdi-open-in-new class="font-size-3 mb-0.5" /></div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Study 2</strong></div>
<div class="grid-item col-span-2">Person 3 <i>as Postdoc</i>&nbsp;<mdi-open-in-new class="font-size-3 mb-0.5" /><br/>Person 4 <i>as Co-PI</i>&nbsp;<mdi-open-in-new class="font-size-3 mb-0.5" /></div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Experiments</strong></div>
<div class="grid-item col-span-2">Smile 🫠</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Funding</strong></div>
<div class="grid-item col-span-2">National Science Foundation<br/>
National Institute of Health</div>
<div class="grid-item text-right mr-4 col-span-1"><strong>Slides</strong></div>
<div class="grid-item col-span-2">
Slidev<br/>
Unocss<br/>
Figma<br/>
Vuejs<br/>
Vite<br/>
</div>
<div class="grid-item col-span-3 text-center mt-180px mb-auto font-size-1.5rem"><strong>Questions?</strong></div>
</div>


---
layout: image-left
image: /images/armitage_quanta.jpg
class: mycoolclass
---

<br />

# Image left

This is the `layout: image-left` layout.

---
layout: image-right
image: /images/armitage_quanta.jpg
slide_info: false
class: mycoolclass
---

# Image right

This is the `layout: image-right` layout.

---
layout: image
image: /images/armitage_quanta.jpg
title: Image Layout
---


---
layout: iframe-right
title: iframe Right Layout
# the web page source
url: https://arxiv.org/html/2506.18709v1#abstract

# a custom class name to the content
class: my-cool-content-on-the-right
slide_info: false
---

# This is a website on the right

This is useful for showing a website but loads live on the web so requires and internet connection.

---
layout: two-cols-title
columns: is-6
align: l-lt-lt
title: Two Cols Title - Header (Info)
---

:: title ::

# `two-cols-title`

:: left ::

This is `layout: two-cols-title`. 

- There are three slots: `:: title ::`, `:: left ::`, and `:: right ::` along with the default which is implicit before any named slots.

- It additionally provides three configuration options in the slide YAML front matter:
  `color`, `columns` and `align`.

:: right ::

- `color` is the color scheme.

- `columns` is the relative spacing given to the left versus right column. The overall space is divided into 12 columns. Instructions like `is-5` will give 5 units to the left and 7 to the right.

- The <code>align</code> parameter determines how the columns look. The notation is for example
  <code>align: l-cm-cm</code>. The first part is for the header, the second for the left column, the third part is for the right column. The first letter is (<code>c</code> for center, <code>l</code> for left, <code>r</code> for right), the second letter
  is vertical alignment (<code>t</code> for top, <code>m</code> for middle, <code>b</code> for bottom). Only c/l/r works for the header.




---
layout: side-title
side: l
color: violet
titlewidth: is-4
align: rm-lm
title: Side Title Layout (Another)
---

:: title ::

# `side-title`

# <mdi-arrow-right />

:: content ::

This is `layout: side-title` with `side: left` in the front matter.

```yaml
side: left
color: violet
titlewidth: is-4
align: rm-lm
```



---
layout: side-title
side: r
color: pink-light
titlewidth: is-6
align: lm-lb
title: Side Title Layout (Another)
---

:: title ::
 
# `side-title`

# <mdi-arrow-right />

:: content ::

This is `layout: side-title` with `side: right` in the front matter.

```yaml
side: right
color: pink-light
titlewidth: is-6
align: lm-lb
```




---
layout: default
---

# Extras

In addition to these custom layouts, the **Neversink** theme includes a few custom components that can be used in your slides. These include sticky notes, speech bubbles, cute icons, QR codes, and more.  The next few slides walks through them:

<div class="ns-c-tight">

- admonitions
- sticky notes
- speech bubbles
- cute icons
- QR codes
</div>

---
layout: two-cols-title
columns: is-6
title: Bubbles
---

<SpeechBubble position="l" color='sky' shape="round"  v-drag="[83,364,274,109]">

Hello, I'm a **speech bubble**! I'm a longer speech bubble. I'm still going.
</SpeechBubble>

:: title ::

# Bubbles

:: left ::

- Bubbles are moveable elements that act as speech bubbles
- They can be configured for where you want the arrow to point
- The can be move around if you enable `v-drag` on the element

:: right ::

<SpeechBubble position="bl" color='amber-light' shape="round">

Hello, I'm a **speech bubble**! I'm a longer speech bubble. I'm still going.
Hello, I'm a **speech bubble**! I'm a longer speech bubble. I'm still going.
Hello, I'm a **speech bubble**! I'm a longer speech bubble. I'm still going.
</SpeechBubble>

---
layout: default
title: Sticky Notes
---

<StickyNote color="amber-light" textAlign="left" width="180px" title="Title" v-drag="[66,318,185,171]">

Hello, I'm a **sticky note**.
</StickyNote>

<StickyNote color="sky-light" textAlign="left" width="180px" title="This is my title" v-drag="[375,306,180,180,-15]">

Hello, I'm also a **sticky note** but am blue sky title.
</StickyNote>

<StickyNote color="pink-light" textAlign="left" width="180px"  v-drag="[667,299,185,171,8]">

Hello, I'm also a **sticky note** but I lack a title.
</StickyNote>

# Sticky Notes

- Sticky notes are moveable elements you can use for notes.
- Syntax is

```js
<StickyNote color="amber-light" textAlign="left" width="180px" title="Title" v-drag>
  Hello, I'm a **sticky note**.
</StickyNote>
```


---
layout: default
title: QR Codes
---

# In-line QR Codes

- Send people to a url with a easy to configure QR code

```vue
<QRCode value="https://arxiv.org/abs/2308.13706" :size="200" render-as="svg" />
```

<br />
Result:

<QRCode value="https://arxiv.org/html/2308.13706" :size="200" render-as='svg'/>



---
layout: default
title: Lines
---

# Lines

<Line :x1=0 :y1=0 :x2=200 :y2=200 :width=2 color='red' v-drag="[326,136,250,250]" />




---
layout: side-title
side: left
color: lime
titlewidth: is-4
align: rm-lt
title: LaTeX Example
---

:: title ::

# <mdi-math-integral-box /> LaTeX Equations

Yeah it does this fine

<Mug :size="80" mood="excited" color="#FDA7DC" v-drag="[342,288,77,80]" />

:: content ::

Inline equations: $\sqrt{3x-1}+(1+x)^2$

Block rendering:

$$
\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}
$$

Line highlighting with clicks!

$$
{1|3|all}
\begin{array}{c}
\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\
\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\
\nabla \cdot \vec{\mathbf{B}} & = 0
\end{array}
$$


