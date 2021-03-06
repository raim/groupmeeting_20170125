--- 

title       : The Transcriptional Landscape of Budding Yeast
subtitle    : and the Gummiband Modell
author      : Rainer Machne
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : mathjax       # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides

---   &twocol .lineheight

<style>
.title-slide {
  background-image:url(assets/img/220px-DNA_orbit_animated.gif), url(http://goo.gl/EpXln);
  background-position: right bottom;
  background-repeat: repeat-y;
}

.title-slide hgroup > h1{
 font-family: 'Oswald', 'Helvetica', sanserif; 
}
.title-slide hgroup > h1{
 font-family: 'Oswald', 'Helvetica', sanserif; 
}

.title-slide hgroup > h1, 
.title-slide hgroup > h2 {
  color: #00FFFF ;  /* ; #EF5150*/
}
.title-slide hgroup > p {
  color: #FF0000 ;  /* ; #EF5150*/
}
</style>

<style>
oq {
    background-color:yellow;
    color:#CC2904;
    font-weight: bold;
}
</style>
<style>
em {
  font-style: italic
}
</style>
<style>
.smalltext {
    font-size: 50%;
}
.largetext {
    font-size: 120%;
}
</style>
<style>
hoc {
    color:#FF0000;
    font-weight: bold;
}
loc {
    color:#0000FF;
    font-weight: bold;
}
clB {
    color:#00FF00;
    font-weight: bold;
}
clC {
    color:#00FFFF;
    font-weight: bold;
}
</style> 
## Deoxyribonucleic acid

*** =left
<img src="assets/img/220px-DNA_orbit_animated.gif" height="500">
</br><font size=-1>Richard Wheeler (Zephyris) at en.wikipedia</font>

*** =right

</br></br>

<img src="assets/img/model_feedback.png"  height="180">

</br></br>
Global Regulatory Mechanisms?<br><br>

<div style='text-align: right;'>growth homeostasis</br>cell differentiation</br>sporulation</br>...</div>

Direct Impact of Cell Physiology</br>on Chromosome Structure & Transcription?

--- &twocolbigright

## Chromatin 

*** =left
<img src="assets/img/lee07_clusters_major.png"  height="580">
*** =right

<img src="assets/img/tuliCoarse_li06_timecourse_ranges_major_nrm.png" width="300"></br>
<img src="assets/img/ATP_ADP.png"  width="300"><img src="assets/img/model_feedback.png"  height="100">


<img src="assets/img/remodeling_atp.png"  height="200">

ATP-dependent Nucleosome Remodeling.</br>
A Global Growth Regulatory Feedback?

--- &twocolbigright

## Chromatin 

*** =left
<img src="assets/img/lee07_clusters_major.png"  height="580">
*** =right

<img src="assets/img/nocetti16_ranges_major.png"  height="150">


<font size=-1>raw time-series:</font>|<font size=-1>temporal mean ratio:</div></font>
---|---
|
<img src="assets/img/nucl_nocetti16_movie_.gif"  height="170">|<img src="assets/img/nucl_nocetti16_movie_ts_.gif"  height="170">


<font size=-2>Nocetti & Whitehouse, GenesDevel 2016: *Nucleosome
repositioning underlies dynamic gene expression.*</font>

--- .lineheight .listheight

## Genome
<font size=-0.5>
<img src="assets/img/chromosome_01.png"  height="12">I   </br>
<img src="assets/img/chromosome_02.png"  height="12">II	 </br>
<img src="assets/img/chromosome_03.png"  height="12">III </br>
<img src="assets/img/chromosome_04.png"  height="12">IV	 </br>
<img src="assets/img/chromosome_05.png"  height="12">V   </br>
<img src="assets/img/chromosome_06.png"  height="12">VI  </br>
<img src="assets/img/chromosome_07.png"  height="12">VII </br>
<img src="assets/img/chromosome_08.png"  height="12">VIII</br>
<img src="assets/img/chromosome_09.png"  height="12">IX  </br>
<img src="assets/img/chromosome_10.png"  height="12">X   </br>
<img src="assets/img/chromosome_11.png"  height="12">XI  </br>
<img src="assets/img/chromosome_12.png"  height="12">XII </br>
<img src="assets/img/chromosome_13.png"  height="12">XIII</br>
<img src="assets/img/chromosome_14.png"  height="12">XIV </br>
<img src="assets/img/chromosome_15.png"  height="12">XV  </br>
<img src="assets/img/chromosome_16.png"  height="12">XVI </br>
<img src="assets/img/chromosome_17.png"  height="12">mitochondrial
</font>

* Stream-lined genome; co-evolution with fruits; fermentation specialist
or generalist?
* 16 Nuclear Chromosomes, 1 Mitochondrial Genome, 1 Plasmid</br>
12 Megabases, 5700-6000 protein-coding genes
* <b>Unclear extent and function of non-coding transcription!</b>

---.lineheight .listheight &twocolbigleft

## The Experiment
***=left
<img src="assets/img/sampling.png"  height="300">

### Data pipeline, part I:

1. Take samples, extract ~100 &mu;g total RNA<br> by Kalesh's method!
2. Send off to Beijing Genome Institute for <br>strand-specific RNAseq @ 1k $ per sample
***=right

<img src="assets/img/fermentor_detailed.png" height="200">
<br><oq>reactor magic:</oq>

2 <hoc>HOC</hoc> and 2&frac12; <loc>LOC</loc> phases sampled

--- .listheight .smalltext

### The Data: Primary Segment 0417

<img src="assets/img/primseg_00417.png"  height="300">

1. RNA-seq time-series from bottom to top
2. Transcribed units as reported in 2-3 papers:<br>
ORF: open reading frames, AS: antisense (putative and manually curated)<br>
SUT: stable untranslated, CUT: cryptic unstable, and XUT: Xrn1-sensitive unstable transcripts 
3. Annotated genome features
4. MNase time-series (Nocetti & Whitehouse 2016)  &larr; <b>Nucleosomes</b>

`https://gitlab.com/raim/genomeBrowser` 

--- 

### Expressed Domain 003

<img src="assets/img/domain_003_33kb.png"  height="300">

--- #foo

## Data Pipeline, part II: `KARL`

2. Send 'reads' (`fastq.gz`) files to Berni in Leipzig (Stephan Bernhart) &rarr;
`segemehl` <br/>
<img src="assets/img/burns.jpg" height="145"><img src="assets/img/studlasa.gif" height="145"> 
and
retrieve <b>mapping of reads to genome</b> as <b>read counts!</b>
3. Contemplate over data ... do other stuff ... contemplate more over data ... annoy lots of math people with it ...cyanos ... contemplate yet some more over data ... annoy Studla ...<br/>
4. `KARL`:<br/>
<img src="assets/img/anadenobolus_arboreus.png" height="100">, the<br/>
<img src="assets/img/segmentier.svg" height="45">
5. ... contemplate over data again ...

<script>
$("#foo ol").attr('start', 3)
</script>

--- 

### Similarity-Based Segmentation of Multi-Dimensional Signals by `KARL`

<img src="assets/img/primseg_00436_ash_ash.png" height="250">
<img src="assets/img/T.ash_D.dcash_K.12_S.icor_E.3_M.175_osc_K8.png"  height="250">

1. Cut genome, 2x12 Mb, into digestable chunks (`primary segments`)
2. For each chunk, cluster read-counts; here: similar to previous approch,<br>
take Discrete Fourier Transform `DFT` (scale components) &<br>
cluster selected (de-noised!) `DFT` components
3. Calculate cluster-cluster and cluster-position similarities
4. Feed hungry `KARL`: <b>to find coherently expressed regions</b>



--- .largetext

### Similarity-Based Segmentation of Multi-Dimensional Signals by `KARL`

<img src="assets/img/primseg_00436_ash_ash.png" height="250">
<img src="assets/img/T.ash_D.dcash_K.12_S.icor_E.3_M.175_osc_K8.png"  height="250">


1. Score time series coherence from positions \(j\) to \(i\): \(s(i,j,\mathcal{C})\)
2. Maximize scoring matrix: \(S_{i,\mathcal{C}}\)

$$latex
\begin{equation*} \begin{aligned}
 s(i,j,\mathcal{C})=& -M + \sum_{k=i}^j \tilde\Delta(\mathcal{C}_k,\mathcal{C})\\ 
 S_{i,\mathcal{C}} =& \max_{j \le i} \max_{\mathcal{D}\ne\mathcal{C}} S_{j-1,\mathcal{D}} + s(j,i,\mathcal{C})
\end{aligned} \end{equation*}$$

--- 

### Similarity-Based Segmentation of Multi-Dimensional Signals by `KARL`

<img src="assets/img/primseg_00436_ash_ash.png" height="250">
<img src="assets/img/T.ash_D.dcash_K.12_S.icor_E.3_M.175_osc_K8.png"  height="250">


<br>
<font size=6>
... and `backtrace` over score matrix \(S_{i,\mathcal{C}}\): 

&rarr; <b>find optimal segment breakpoints</b>
</font>

---.listheight

### Finding Optimal Parameters: 108 parameter sets

<img src="assets/img/segmentations_PCA12_dctrafo.png" height="350">
<img src="assets/img/segmentations_PCA12_exponent.png" height="350">

__*PCA of several segmentation characteristica*__, grouped by:<br>

* Data pre-processing (left: dcraw/dcash)<br> 
* `Karl` parameters, here, exponent on Pearson correlation in 
similarity measure (right)

---
### Recovery of Known Transcripts
<img src="assets/img/ORF_ratioTotal_clustered.png" height="400">
<img src="assets/img/SUT_ratioTotal_clustered.png" height="400">

Good recovery of known protein-coding genes.<br>
Random recovery of reported non-coding transcripts!

---
### Recovery of Known Transcripts
<img src="assets/img/A_ratioTotal_clustered.png" height="400">
<img src="assets/img/D_ratioTotal_clustered.png" height="400">

Much better recovery of <hoc>HOC (A)</hoc> than of <loc>LOC (D)</loc> protein-coding transcripts;<br> 
ribosomes, amino acid synthesis, etc: important growth genes!</br>

---.centertext
## The Result: Pervasive Transcription during <loc>LOC</loc>

<img src="assets/img/T.ash_D.dcash_K.20_S.icor_E.5_M.175_timeseries.png" height="450">

## ... defined and conserved growth genes during <hoc>HOC</hoc>

--- 

### Domain 122

<img src="assets/img/domain_122_106kb.png"  width="900">


--- 

### Domain 046

<img src="assets/img/domain_046_69kb.png" width="900">

--- 

### Primary Segment 0273

<img src="assets/img/primseg_00273.png"  height="300">

--- 

### Primary Segment 0271

<img src="assets/img/primseg_00271.png"  height="300">

--- 

### Primary Segment 0436

<img src="assets/img/primseg_00436.png" height=300>

<div class="centered">fail ;( </div> 

tiny osci segment divergent to SRG1 not recognized

--- {.build}

## Slide

> 1. Point 1
> 2. Point 2

.build text
