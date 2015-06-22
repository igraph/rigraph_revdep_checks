# Setup

## Platform

|setting  |value                        |
|:--------|:----------------------------|
|version  |R version 3.2.0 (2015-04-16) |
|system   |x86_64, darwin13.4.0         |
|ui       |X11                          |
|language |(EN)                         |
|collate  |en_US.UTF-8                  |
|tz       |America/New_York             |

## Packages

|package    |*  |version   |date       |source         |
|:----------|:--|:---------|:----------|:--------------|
|ape        |   |3.3       |2015-05-29 |CRAN (R 3.2.0) |
|igraphdata |   |0.2.2     |2015-04-09 |CRAN (R 3.2.0) |
|irlba      |   |1.0.3     |2014-01-25 |CRAN (R 3.2.0) |
|lazyeval   |   |0.1.10    |2015-01-02 |CRAN (R 3.2.0) |
|magrittr   |   |1.5       |2014-11-22 |CRAN (R 3.2.0) |
|NMF        |   |0.20.6    |2015-05-26 |CRAN (R 3.2.0) |
|rgl        |   |0.95.1201 |2014-12-21 |CRAN (R 3.2.0) |
|scales     |   |0.2.4     |2014-04-22 |CRAN (R 3.2.0) |

# Check results
185 checked out of 185 dependencies 

# Known errors

- [x] FCMapper Negative loop and KK layout in example.
      Solution is to switch to another layout. Need to email.

# Cannot check

- [ ] gemtc Neeeds `BRugs` package, needs to check on Linux.
- [ ] mlDNA Need extra package, links to GTK? Cairo?
- [ ] pathClass Extra packages that I cannot install.
- [ ] RGraphics Needs ggobi.
- [ ] RQDA Needs GTK?
- [ ] SeqGrapheR Extra packages, rggobi.

# Sent email to maintainers about the problem

- [x] BoolNet Warnings about docs links, fine. Email them.
- [x] causaleffect
    - Replaces an import, need to email them.
    - Has a bug, uses 0 eid, which is not caught in igraph 0.7.1
- [x] clickstream union overridden, need to email them
- [x] fuzzyMM Replacing union?
- [x] loe Replace previous import diversity.
- [x] nat `knn` import overwritten.
- [x] netgen Replacing imports: `normalize`.
- [x] restlos `normalize` import replaced
- [x] SINGLE replaced import `permute`
- [x] TDA Replace imported `knn`.
- [x] FCMapper Negative loop and KK layout in example.
      Solution is to switch to another layout. Need to email.

# Problematic packages after the first round

- [x] bio3d
    - `plot.igraph` needs to be exported. Fixed.
    - Other error. Seems unrelated.
- [x] BoolNet Warnings about docs links, fine. Email them.
- [x] causaleffect
    - Replaces an import, need to email them.
    - graph.formula broken from another package?
- [x] clickstream union overridden, need to email them
- [x] comato
    - `layout.spring` Fixed.
    - Example error. Fixed.
- [x] fanovaGraph Error in example. Fixed.
- [x] FCMapper Error.
- [x] FisHiCal Data type version. Fixed.
- [x] fuzzyMM Replacing union?
- [x] gemtc Neeeds `BRugs` package, needs to check on Linux.
- [x] intergraph Older data type version. Fixed.
- [x] loe
    - Replace previous import diversity.
    - layout.kamada.kawai has no `start` argument? Fixed.
- [x] mlDNA Need extra package, links to GTK? Cairo?
- [x] modMax Bug in `neighbors`? Fixed.
- [x] nat `knn` import overwritten.
- [x] netassoc Negative weight in KK layout. Fixed.
- [x] netgen Replacing imports: `normalize`.
- [x] netgsa Data type version. Fixed.
- [x] pathClass Extra packages.
- [x] PBC Multiple errors. Fixed.
- [x] popgraph Older data type. Fixed.
- [x] PROFANCY Older data type. Fixed.
- [x] rags2ridges neighbors() bug. Fixed.
- [x] RcmdrPlugin.RMTCJags ??? fixed
- [x] ReliabilityTheory Data type version. Fixed.
- [x] restlos `normalize` import replaced
- [x] RGraphics Needs extra. ggobi.
- [x] RQDA Needs GTK?
- [x] SDDE Data type version. Fixed.
- [x] secrlinear Data type version. Fixed.
- [x] SeqGrapheR Extra packages, rggobi.
- [x] SINGLE replaced import `permute`
- [x] SOMbrero Data type version. Fixed.
- [x] SubpathwayGMir Data type version. Fixed.
- [x] TDA Replace imported `knn`.
- [x] timeordered Error.
- [x] treemap `layout.fruchterman.reingold` arguments
- [x] VineCopula Error.
- [x] xergm Needs extra.


# Packages initially found problematic

- [x] adegenet `plot.igraph`, `print.igraph` exports, plus U
- [x] ARTIVA `layout.spring` and `layout.svd` were removed. Fixed.
- [x] arulesViz `Rgraphviz` not available. Need to install.
- [x] backShift Needs `graph` package.
- [x] bc3net Unrelated.
- [x] BDgraph `plot.igraph` needs to be exported. Fixed.
- [x] bio3d
    - `plot.igraph` needs to be exported. Fixed.
    - Data format version
- [x] bipartite Unrelated.
- [x] BoolNet Warnings about docs links, fine. Email them.
- [x] c3net Unrelated.
- [x] camel Unrelated.
- [x] causaleffect
    - Replaces an import, need to email them.
    - graph.formula broken from another package?
- [x] cccd Error.
- [x] CePa Unrelated. 
- [x] CIDnetworks `plot.igraph` export
- [x] clickstream union overridden, need to email them
- [x] comato
    - `layout.spring` Fixed.
    - Example error
- [x] ConnMatTools Unrelated.
- [x] corclass Unrelated
- [x] cvxclustr Unrelated.
- [x] DCGL Need `limma` pkg.
- [x] dcGOR Extra packages.
- [x] DiffCorr Need extra packages.
- [x] diffusionMap Unrelated.
- [x] dils Unrelated
- [x] dna Unrelated
- [x] dnet Need extra pkgs.
- [x] Dominance `plot.igraph` export fixed.
- [x] dpa Unrelated.
- [x] dynatopmodel Unrelated.
- [x] enaR Unrelated.
- [x] ESEA Need `graph` package.
- [x] fanovaGraph Error in example.
- [x] fbRanks Unrelated.
- [x] FCMapper Error.
- [x] FedData Need extra packages.
- [x] FisHiCal Data type version.
- [x] flare Unrelated.
- [x] FrF2 Unrelated.
- [x] fuzzyMM Replacing union?
- [x] G1DBN Unrelated.
- [x] gemtc Neeeds `BRugs` package.
- [x] GeneReg Unrelated.
- [x] gRain Need `graph` and `Rgraphviz`.
- [x] gRapfa Unrelated.
- [x] gRbase Need extra packages.
- [x] gRim Needs extra packages.
- [x] gromovlab `plot.igraph` export
- [x] huge Unrelated.
- [x] igraphtosonia Unrelated.
- [x] InteractiveIGraph `plot.igraph` needs to be exported.
- [x] intergraph Older data type version.
- [x] iRefR Needs extra packages.
- [x] JGL Unrelated.
- [x] kknn Unrelated.
- [x] knitrBootstrap Unrelated.
- [x] lava `graph` `Rgraphviz` needed.
- [x] lcd Unrelated.
- [x] locits U
- [x] loe
    - Replace previous import diversity.
    - layout.kamada.kawai has no `start` argument?
- [x] markovchain `plot.igraph` not exported.
- [x] matie `plot.igraph` export
- [x] micropan Unrelated.
- [x] miniCRAN `plot.igraph` not exported.
- [x] mlDNA Need extra package, links to GTK? Cairo?
- [x] modMax Bug in `neighbors`?
- [x] mRMRe `plot.igraph` needs exported.
- [x] nat `knn` import overwritten.
- [x] netassoc Error.
- [x] netClass Needs extra packages.
- [x] netgen Replacing imports: `normalize`.
- [x] netgsa Data type version.
- [x] nets U
- [x] NetSim U
- [x] nettools Extra packages.
- [x] netweavers Extra packages.
- [x] optrees `plot.igraph` export
- [x] osmar U
- [x] outbreaker Needs GSL.
- [x] packdep Needs extra packages.
- [x] PAGI U
- [x] pathClass Extra packages.
- [x] PBC Multiple errors.
- [x] pcalg Extra packages.
- [x] PGRdup U
- [x] phangorn Extra package.
- [x] phyloTop U
- [x] popgraph Older data type.
- [x] poplite Extra package.
- [x] poppr `plot.igraph`
- [x] ppiPre Extra packages.
- [x] PROFANCY Older data type.
- [x] qdap `plot.igraph` + U
- [x] qtlnet Needs `graph` package.
- [x] QuACN NEeds extra packages.
- [x] rags2ridges neighbors() bug.
- [x] rbmn U
- [x] RCA U
- [x] RcmdrPlugin.RMTCJags ???
- [x] RDS `plot.igraph` export
- [x] ReliabilityTheory Data type version.
- [x] rEMM Extra packages.
- [x] restlos `normalize` import replaced
- [x] RevEcoR `plot.igraph`
- [x] rgp U
- [x] RGraphics Needs extra.
- [x] RNetLogo U
- [x] ror `plot.igraph` export
- [x] rPref U
- [x] RQDA Needs GTK?
- [x] rtop U
- [x] sand Extra packages.
- [x] SDDE DAta type version.
- [x] secrlinear Data type version.
- [x] SEMID U
- [x] semPlot U
- [x] sensitivity `plot.igraph` export
- [x] SeqGrapheR Extra packages.
- [x] sglasso `plot.igraph` export
- [x] sharpshootR `plot.igraph`
- [x] shp2graph U
- [x] SID Needs extra pkgs.
- [x] simcausal `plot.igraph` export
- [x] SINGLE replaced import `permute`
- [x] SOMbrero Data type version.
- [x] spacejam U
- [x] spatgraphs U
- [x] spdep U
- [x] SPMS Needs extra.
- [x] SSN U
- [x] stm `plot.igraph`
- [x] structSSI Extra pkgs.
- [x] SubpathwayGMir Data type version.
- [x] tcR U
- [x] TDA Replace imported `knn`.
- [x] timeordered Error.
- [x] tnet U
- [x] treemap `layout.fruchterman.reingold` arguments
- [x] TunePareto U
- [x] VineCopula Error.
- [x] xergm Needs extra.

## adegenet (1.4-2)
Maintainer: Thibaut Jombart <t.jombart@imperial.ac.uk>

```
checking whether package âadegenetâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/adegenet.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## ARTIVA (1.2.3)
Maintainer: S. Lebre <sophie.lebre@icube.unistra.fr>

```
checking R code for possible problems ... NOTE
traceNetworks: no visible global function definition for
  âlayout.springâ
traceNetworks: no visible global function definition for âlayout.svdâ
```
```
DONE
Status: 1 NOTE
```

## arulesViz (1.0-0)
Maintainer: Michael Hahsler <mhahsler@lyle.smu.edu>

```
checking package dependencies ... ERROR
Packages suggested but not available: âRgraphvizâ âgraphâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## backShift (0.1.1)
Maintainer: Christina Heinze <heinze@stat.math.ethz.ch>

```
checking whether package âbackShiftâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/backShift.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## bc3net (1.0.2)
Maintainer: Ricardo de Matos Simoes <r.dematossimoes@qub.ac.uk>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
Authors@R field gives more than one person with maintainer role:
  Ricardo de Matos Simoes <r.dematossimoes@qub.ac.uk> [aut, cre]
  Frank Emmert-Streib <f.emmert-streib@qub.ac.uk> [aut, cre]
```
```
checking top-level files ... NOTE
Non-standard file/directory found at top level:
  âdocsâ
```
```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âMatrixâ âc3netâ âigraphâ âinfotheoâ âlatticeâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
.mat2igraph: no visible global function definition for
  âgraph.data.frameâ
.mat2igraph: no visible global function definition for âEâ
.mat2igraph: no visible global function definition for âE<-â
.mat2igraph: no visible global function definition for âVâ
.mat2igraph: no visible global function definition for âadd.verticesâ
.mat2igraph: no visible global function definition for âV<-â
.mat2igraph: no visible global function definition for âgraphâ
bc3net: no visible global function definition for âc3â
bc3net: no visible global function definition for âforceSymmetricâ
c3mtc: no visible global function definition for âc3â
c3mtc: no visible global function definition for âforceSymmetricâ
mimwrap: no visible global function definition for âdiscretizeâ
mimwrap: no visible global function definition for âmutinformationâ
```
```
DONE
Status: 4 NOTEs
```

## BDgraph (2.18)
Maintainer: Abdolreza Mohammadi <a.mohammadi@rug.nl>

```
checking R code for possible problems ... NOTE
bdgraph.sim: no visible global function definition for âplot.igraphâ
compare: no visible global function definition for âplot.igraphâ
plot.bdgraph: no visible global function definition for âplot.igraphâ
plot.simulate: no visible global function definition for âplot.igraphâ
select: no visible global function definition for âplot.igraphâ
summary.bdgraph: no visible global function definition for
  âplot.igraphâ
```
```
DONE
Status: 1 NOTE
```

## bio3d (2.2-2)
Maintainer: Barry Grant <bjgrant@umich.edu>

```
checking dependencies in R code ... NOTE
Missing or unexported object: âigraph::plot.igraphâ
```
```
checking examples ... ERROR
Running examples in âbio3d-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: prune.cna
> ### Title: Prune A cna Network Object
> ### Aliases: prune.cna
> ### Keywords: utility
> 
> ### ** Examples
> 
> 
> # Load the correlation network
> attach(hivp)
> 
> # Read the starting PDB file to determine atom correspondence
> pdbfile <- system.file("examples/hivp.pdb", package="bio3d")
> pdb <- read.pdb(pdbfile)
> 
> # Plot coarse grain network based on dynamically coupled communities
> par(mfcol=c(1,2), mar=c(0,0,0,0))
> plot.cna(net)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: plot.cna -> <Anonymous> -> update_es_ref -> check_version
Execution halted
```
```
checking tests ... ERROR
Running the tests in âtests/testthat.Râ failed.
Last 13 lines of output:
  .......... .......... .......... .......... ..........
  .......... .......... .......... .......... ..........
  .......... .......... .......... .......... 
  downloaded 590 KB
  
  testthat results ================================================================
  OK: 253 SKIPPED: 0 FAILED: 3
  1. Error: SSE assignment still works 
  2. Error: struct.aln still works 
  3. Error: fit.xyz() gets the same results as VMD 
  
  Error: testthat unit tests failed
  Execution halted
```
```
DONE
Status: 2 ERRORs, 1 NOTE
```

## bipartite (2.05)
Maintainer: Carsten F. Dormann <carsten.dormann@biom.uni-freiburg.de>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.wine
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
DONE
Status: 2 NOTEs
```

## BoolNet (2.1.1)
Maintainer: Hans A. Kestler <hans.kestler@uni-ulm.de>

```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'plotAttractors.Rd':
  â[igraph]{layout}â â[igraph:plot.graph]{plot.igraph}â

Missing link or links in documentation object 'plotNetworkWiring.Rd':
  â[igraph]{layout}â â[igraph:plot.graph]{plot.igraph}â
  â[igraph:plot.graph]{igraph.plotting}â

Missing link or links in documentation object 'plotPBNTransitions.Rd':
  â[igraph]{layout}â â[igraph:plot.graph]{plot.igraph}â

Missing link or links in documentation object 'plotSequence.Rd':
  â[igraph]{layout}â â[igraph:plot.graph]{plot.igraph}â

Missing link or links in documentation object 'plotStateGraph.Rd':
  â[igraph]{layout}â â[igraph:plot.graph]{plot.igraph}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
DONE
Status: 1 WARNING
```

## c3net (1.1.1)
Maintainer: Gokmen Altay <altayscience@gmail.com>

```
checking examples ... ERROR
Running examples in âc3net-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: c3net
> ### Title: All in one function to infer network with C3NET
> ### Aliases: c3net
> ### Keywords: misc
> 
> ### ** Examples
> 
> data(expdata)
> data(truenet)
> 
> net <- c3net(expdata, network=TRUE)
Loading required package: tcltk
XIO:  fatal IO error 35 (Resource temporarily unavailable) on X server "/private/tmp/com.apple.launchd.rULzlZIqm8/org.macosforge.xquartz:0"
      after 95 requests (95 known processed) with 0 events remaining.
```
```
DONE
Status: 1 ERROR
```

## camel (0.2.0)
Maintainer: Xingguo Li <xingguo.leo@gmail.com>

```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.slim
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking compiled code ... NOTE
File âcamel/libs/camel.soâ:
  Found â_randâ, possibly from ârandâ (C)
    Object: âSFGen.oâ
  Found â_srandâ, possibly from âsrandâ (C)
    Object: âSFGen.oâ

Compiled code should not call entry points which might terminate R nor
write to stdout/stderr instead of to the console, nor the system RNG.

See âWriting portable packagesâ in the âWriting R Extensionsâ manual.
```
```
DONE
Status: 2 NOTEs
```

## causaleffect (1.1.1)
Maintainer: Santtu Tikka <santtuth@gmail.com>

```
checking whether package âcausaleffectâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âigraph::paâ when loading âcausaleffectâ
See â/Users/gaborcsardi/works/igraph/revdep_check/causaleffect.Rcheck/00install.outâ for details.
```
```
checking examples ... ERROR
Running examples in âcausaleffect-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: causal.effect
> ### Title: Identify a causal effect
> ### Aliases: causal.effect
> 
> ### ** Examples
> 
> library(igraph)

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union

> 
> # simplify = FALSE to allow multiple edges
> g <- graph.formula(X -+ Y, Z -+ X, Z -+ Y , X -+ Z, Z -+ X, simplify = FALSE) 
> 
> # Here the bidirected edge between X and Z is set to be unobserved in graph g
> # This is denoted by giving them a description attribute with the value "U"
> # The edges in question are the fourth and the fifth edge
> g <- set.edge.attribute(graph = g, name = "description", index = c(4,5), value = "U") 
> 
> res <- causal.effect(y = "Y", x = "X", G = g)
Error in simple_es_index(x, ii) : Unknown edge selected
Calls: causal.effect ... as.igraph.es -> inherits -> [ -> [.igraph.es -> simple_es_index
Execution halted
```
```
DONE
Status: 1 ERROR, 1 WARNING
```

## cccd (1.5)
Maintainer: David J. Marchette <dmarchette@gmail.com>

```
checking examples ... ERROR
Running examples in âcccd-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: cccd
> ### Title: Class Cover Catch Digraph
> ### Aliases: cccd cccd.rw cccd.classify cccd.classifier cccd.classifier.rw
> ###   cccd.multiclass.classifier cccd.multiclass.classify plot.cccd
> ###   plot.cccdClassifier
> ### Keywords: graphs
> 
> ### ** Examples
> 
> set.seed(456330)
> z <- matrix(runif(1000),ncol=2)
> ind <- which(z[,1]<.5 & z[,2]<.5)
> x <- z[ind,]
> y <- z[-ind,]
> g <- cccd(x,y)
> C <- cccd.classifier(x,y)
Error in graph(n = vc, edges, directed = (mode == "directed")) : 
  'edges' must be numeric of character
Calls: cccd.classifier ... dominate.greedy -> graph.adjacency -> graph.adjacency.sparse -> graph
Execution halted
```
```
DONE
Status: 1 ERROR
```

## CePa (0.5)
Maintainer: Zuguang Gu <jokergoo@gmail.com>

```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âigraphâ âsnowâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.cepa plot.cepa.all plot.pathway.catalogue print.cepa
  print.cepa.all print.pathway.catalogue
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
centrality: no visible global function definition for âvcountâ
centrality: no visible global function definition for âdegreeâ
centrality: no visible global function definition for âbetweennessâ
cepa.all.parallel.by.snow: no visible global function definition for
  âmakeClusterâ
cepa.all.parallel.by.snow: no visible global function definition for
  âclusterCallâ
cepa.all.parallel.by.snow: no visible global function definition for
  âclusterApplyâ
cepa.all.parallel.by.snow: no visible global function definition for
  âstopClusterâ
generate.pathway: no visible global function definition for
  âgraph.edgelistâ
pathway.nodes: no visible global function definition for âvcountâ
pathway.nodes: no visible global function definition for
  âget.vertex.attributeâ
plot.igraph2: no visible binding for global variable âlayout.randomâ
plot.igraph2: no visible global function definition for âVâ
plot.igraph2: no visible global function definition for âEâ
plot.igraph2: no visible global function definition for âget.edgelistâ
plot.igraph2: no visible global function definition for âecountâ
plotGraph: no visible global function definition for âVâ
plotGraph: no visible global function definition for âV<-â
plotGraph: no visible global function definition for âEâ
plotGraph: no visible global function definition for âE<-â
plotGraph : layout.method: no visible global function definition for
  âlayout.reingold.tilfordâ
radiality: no visible global function definition for âshortest.pathsâ
radiality: no visible global function definition for âvcountâ
radiality: no visible global function definition for âdiameterâ
reach: no visible global function definition for âEâ
reach: no visible global function definition for âshortest.pathsâ
report: no visible global function definition for âwrite.graphâ
spread: no visible global function definition for âEâ
spread: no visible global function definition for âshortest.pathsâ

Found the following calls to attach():
File âCePa/R/report.Râ:
  attach(replacement, warn.conflicts = FALSE)
See section âGood practiceâ in â?attachâ.
```
```
checking Rd line widths ... NOTE
Rd file 'cepa.Rd':
  \usage lines wider than 90 characters:
     cepa(dif = NULL, bk = NULL, mat = NULL, label = NULL, pc, pathway = NULL, id = NULL, cen = "equal.weight",
         cen.name = if(is.function(cen)) deparse(substitute(cen)) else if(mode(cen) == "name") deparse(cen) else cen,

Rd file 'cepa.all.Rd':
  \examples lines wider than 100 characters:
     label = read.cls("http://mcube.nju.edu.cn/jwang/lab/soft/cepa/P53.cls", treatment="MUT", control="WT")

Rd file 'cepa.all.parallel.Rd':
  \usage lines wider than 90 characters:
     cepa.all.parallel(dif = NULL, bk = NULL, mat = NULL, label = NULL, pc, cen = default.centralities,
  \examples lines wider than 100 characters:
     label = read.cls("http://mcube.nju.edu.cn/jwang/lab/soft/cepa/P53.cls", treatment="MUT", control="WT")

Rd file 'cepa.ora.Rd':
  \usage lines wider than 90 characters:
              cen.name = if(is.function(cen)) deparse(substitute(cen)) else if(mode(cen) == "name") deparse(cen) else cen,

Rd file 'cepa.univariate.Rd':
  \usage lines wider than 90 characters:
         cen.name = if(is.function(cen)) deparse(substitute(cen)) else if(mode(cen) == "name") deparse(cen) else cen,

Rd file 'cepa.univariate.all.Rd':
  \examples lines wider than 100 characters:
     label = read.cls("http://mcube.nju.edu.cn/jwang/lab/soft/cepa/P53.cls", treatment="MUT", control="WT")

Rd file 'plotGraph.Rd':
  \usage lines wider than 90 characters:
         graph.node.max.size = 20, graph.node.min.size = 3, graph.layout.method = NULL, ...)                 

Rd file 'read.cls.Rd':
  \examples lines wider than 100 characters:
     label = read.cls("http://mcube.nju.edu.cn/jwang/lab/soft/cepa/P53.cls", treatment="MUT", control="WT")

Rd file 'report.Rd':
  \usage lines wider than 90 characters:
            template.file = paste(system.file(package = "CePa"), "/extdata/cepa.template", sep=""),

These lines will be truncated in the PDF manual.
```
```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'plotGraph.Rd':
  â[igraph]{layout}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
DONE
Status: 1 WARNING, 4 NOTEs
```

## CIDnetworks (0.8.1)
Maintainer: Beau Dabbs <bdabbs@andrew.cmu.edu>

```
checking whether package âCIDnetworksâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/CIDnetworks.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## clickstream (1.1.4)
Maintainer: Michael Scholz <michael.scholz@uni-passau.de>

```
checking whether package âclickstreamâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âigraph::unionâ when loading âclickstreamâ
See â/Users/gaborcsardi/works/igraph/revdep_check/clickstream.Rcheck/00install.outâ for details.
```
```
DONE
Status: 1 WARNING
```

## comato (1.0)
Maintainer: Andreas Muehling <andreas.muehling@tum.de>

```
checking R code for possible problems ... NOTE
plot.conceptmap: no visible global function definition for
  âlayout.springâ
plot.conceptmaps: no visible global function definition for
  âlayout.springâ
```
```
checking examples ... ERROR
Running examples in âcomato-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: plot.conceptmaps
> ### Title: Plotting a series of concept maps
> ### Aliases: plot.conceptmaps
> 
> ### ** Examples
> 
> #Create concept maps from three random graphs
> require("igraph")
Loading required package: igraph

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union

> g1 = set.vertex.attribute(erdos.renyi.game(5, 0.7, type="gnp"), "name", value=1:5)
> g2 = set.vertex.attribute(erdos.renyi.game(5, 0.7, type="gnp"), "name", value=1:5)
> g3 = set.vertex.attribute(erdos.renyi.game(5, 0.7, type="gnp"), "name", value=1:5)
> E(g1)$name <- rep("", length(E(g1)))
> E(g2)$name <- rep("", length(E(g2)))
> E(g3)$name <- rep("", length(E(g3)))
> #Create conceptmaps object from three conceptmap objects
> simple_cms = conceptmaps(list(conceptmap(g1), conceptmap(g2), conceptmap(g3)))
> 
> plot(simple_cms, layout="spring")
Error in as.vector(y) : argument "y" is missing, with no default
Calls: plot ... union.default -> <Anonymous> -> unique -> as.vector
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## ConnMatTools (0.1.5)
Maintainer: David M. Kaplan <dmkaplan2000@gmail.com>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
eigs: no visible global function definition for âarpackâ
```
```
DONE
Status: 2 NOTEs
```

## corclass (0.1)
Maintainer: Andrei Boutyline <andrei.boutyline@gmail.com>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âCairoâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
Package in Depends field not imported from: âigraphâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.cca print.cca
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
.cormat.to.igraph: no visible global function definition for
  âgraph.adjacencyâ
cca: no visible global function definition for
  âleading.eigenvector.communityâ
plot.cca: no visible binding for global variable âlayout.kamada.kawaiâ
plot.cca: no visible global function definition for âdelete.edgesâ
plot.cca: no visible global function definition for âEâ
plot.cca: no visible global function definition for âCairoPDFâ
```
```
DONE
Status: 3 NOTEs
```

## cvxclustr (1.1.1)
Maintainer: Eric C. Chi <ecchi1105@gmail.com>

```
checking line endings in Makefiles ... NOTE
Found the following Makefile(s) without a final LF:
  src/Makevars
Some âmakeâ programs ignore lines not ending in LF.
```
```
DONE
Status: 1 NOTE
```

## DCGL (2.1.2)
Maintainer: Bao-Hong Liu <bhliu@scbit.org>

```
checking package dependencies ... ERROR
Package required but not available: âlimmaâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## dcGOR (1.0.4)
Maintainer: Hai Fang <hfang@cs.bris.ac.uk>

```
checking whether package âdcGORâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/dcGOR.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## DiffCorr (0.4.1)
Maintainer: Atsushi Fukushima <atsushi.fukushima@riken.jp>

```
checking package dependencies ... ERROR
Packages required but not available: âpcaMethodsâ âmulttestâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## diffusionMap (1.1-0)
Maintainer: Joseph Richards <joeyrichar@gmail.com>

```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.dmap print.dmap
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
DONE
Status: 1 NOTE
```

## dils (0.8.1)
Maintainer: Stephen R. Haptonstahl <srh@haptonstahl.org>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âRcppâ âigraphâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
EdgelistFromIgraph: no visible global function definition for
  âget.adjacencyâ
EdgelistFromIgraph: no visible global function definition for âVâ
EdgelistFromIgraph: no visible global function definition for âvcountâ
IgraphFromEdgelist: no visible global function definition for
  âgraph.adjacencyâ
IgraphFromEdgelist: no visible global function definition for âVâ
IgraphFromEdgelist: no visible global function definition for âV<-â
MeasureNetworkInformation: no visible binding for global variable
  âbetweennessâ
MeasureNetworkInformation: no visible global function definition for
  âvcountâ
MeasureNetworkInformation : SampleIgraph: no visible global function
  definition for âecountâ
MeasureNetworkInformation : SampleIgraph: no visible global function
  definition for âdelete.edgesâ
MeasureNetworkInformation : SampleIgraph: no visible global function
  definition for âEâ
RelativeNetworkInformation: no visible binding for global variable
  âbetweennessâ
RssSuggestedNetwork: no visible global function definition for
  âget.adjacencyâ
RssSuggestedNetwork: no visible global function definition for
  âis.directedâ
RssSuggestedNetwork: no visible global function definition for âvcountâ
RssSuggestedNetwork: no visible global function definition for
  âgraph.adjacencyâ
RssSuggestedNetwork: no visible global function definition for
  âgraph.densityâ
```
```
DONE
Status: 3 NOTEs
```

## dna (1.1-1)
Maintainer: Ryan Gill <ryan.gill@louisville.edu>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
network.modules: no visible global function definition for
  âgraph.emptyâ
network.modules: no visible global function definition for
  âadd.verticesâ
network.modules: no visible global function definition for âadd.edgesâ
network.modules: no visible global function definition for âtkplotâ
network.modules: no visible global function definition for âVâ
```
```
DONE
Status: 2 NOTEs
```

## dnet (1.0.6)
Maintainer: Hai Fang <hfang@cs.bris.ac.uk>

```
checking package dependencies ... ERROR
Packages required but not available:
  âsupraHexâ âgraphâ âRgraphvizâ âBiobaseâ

Package suggested but not available: âlimmaâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## Dominance (1.0.0)
Maintainer: Knut Krueger <Knut.Krueger@equine-science.de>  
Bug reports: see maintainer

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
checking R code for possible problems ... NOTE
Sociogram: no visible global function definition for âplot.igraphâ
```
```
checking examples ... ERROR
Running examples in âDominance-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: Sociogram
> ### Title: Social Network Graphs
> ### Aliases: Sociogram
> ### Keywords: ~kwd1 ~kwd2
> 
> ### ** Examples
> 
> 
> 
> ## you can eihter use:
> data_sheet=data.frame   ("action.from"=c(1,4,2,3,4,3,4,3,4,3,4,3,4,3,4),
+                    "action.to"=c(4,1,1,4,3,4,3,4,3,4,3,4,3,4,3),
+                    "kind.of.action"= c(4,1,1,4,3,4,3,4,3,4,3,4,3,4,3),stringsAsFactors=FALSE)
> items= data.frame ("Name"=c("item1","item2","item3","item4","item5","item6") ,
+                    "item.number"=c(1:6),stringsAsFactors=FALSE)
> actions=data.frame("name.of.action"= c("leading","following","approach","bite","threat to bite",
+                    "kick","threat to kick", "chase","retreat"),
+                    "action.number"=c(1:9),
+                    "classification"=c(1,2,1,1,1,1,1,1,2) ,
+                    "weighting"=c(1,-1,1,1,1,1,1,1,-1),stringsAsFactors=FALSE)
> ## all  encounters  without leading and following
> bytes= "001111111"  
> Sociogram(data_sheet,items=items,actions=actions,bytes)
Error in Sociogram(data_sheet, items = items, actions = actions, bytes) : 
  could not find function "plot.igraph"
Execution halted
```
```
DONE
Status: 1 ERROR, 2 NOTEs
```

## dpa (1.0-3)
Maintainer: Emile Chappin <e.j.l.chappin@tudelft.nl>

```
checking R code for possible problems ... NOTE
dpa.analysis.options : OnOK: warning in assign("rbVal", rbVal, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.options : OnOK : OnSave: warning in assign("time_column",
  time_column, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.analysis.options : OnOK : OnSave: warning in assign("intervalVal",
  intervalVal, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.analysis.options : OnOK : OnSave :
  dpa.analysis.options.ticks.enter: warning in assign("NumTick",
  NumTick, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.analysis.performDPA : dpa.specifyModel: warning in assign("row",
  row, env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.specifyModel: warning in
  assign("variables", baseVariables, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem", sem, env = .GlobalEnv): partial argument match of 'env'
  to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem.DPA", sem.DPA, env = .GlobalEnv): partial argument match
  of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem.standardized", sem.standardized, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("relevantData", relevantData, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem.results.coefficients", sem.results.coefficients, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem.results.parameters", sem.results.parameters, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("sem.results.statistics", sem.results.statistics, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA : dpa.analysis.doPerform: warning in
  assign("listOfTicks", listOfTicks, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("listOfTicks", NULL, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("sem.DPA", NULL, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("sem.standardized", NULL,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("sem.results.parameters",
  NULL, env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("sem.results.statistics",
  NULL, env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.performDPA: warning in assign("sem.results.coefficients",
  NULL, env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.analysis.saveDPA: warning in assign("dpaFileName", dpaFileName, env
  = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadData: warning in assign("ak1", ak1, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("ak2", ak2, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("dbServerType",
  dbServerType, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.data.loadDataFromDatabase: warning in assign("dbServer", dbServer,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("dbName", dbName, env
  = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("dbTable", dbTable,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("UserName", UserName,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDatabase: warning in assign("Password", Password,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.data.loadDataFromDisk: warning in assign("dataFileName",
  dataFileName, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.data.loadDataFromDisk: warning in assign("e", e, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.generate.lag: warning in assign("dataframe", dataframe, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.incrementValue: warning in assign("i", i, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.relations.addRelations: warning in assign("relations", relations,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.relations.addRelations: warning in assign("time_column",
  time_column, env = .GlobalEnv): partial argument match of 'env' to
  'envir'
dpa.relations.addRelations: warning in assign("e", e, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.relations.loadRelations: warning in assign("relations", relations,
  env = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.results.setGraphDir: warning in assign("graphDir", graphDir, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.results.viewNodePlots : dpa.results.plotNodes : dpa.plot.scatter:
  warning in png(file = paste(graphDir, "/scatter_", xcolumn, "_",
  ycolumn, "_", ".png", sep = ""), res = 300, width = 3000, height =
  2000): partial argument match of 'file' to 'filename'
dpa.results.viewNodePlots : dpa.results.plotNodesWithTime :
  dpa.plot.scatter: warning in png(file = paste(graphDir, "/scatter_",
  xcolumn, "_", ycolumn, "_", tick, ".png", sep = ""), res = 300, width
  = 3000, height = 2000): partial argument match of 'file' to
  'filename'
dpa.results.viewRelationsPlots : dpa.plot.graph: warning in png(file =
  paste(graphDir, "/graph_", "relation", ".png", sep = ""), res = 92,
  width = 1000, height = 1000): partial argument match of 'file' to
  'filename'
dpa.results.viewRelationsPlots : dpa.plot.graph: warning in png(file =
  paste(graphDir, "/graph_", "relation_", format(tickNumber, width =
  4), ".png", sep = ""), res = 92, width = 1000, height = 1000):
  partial argument match of 'file' to 'filename'
dpa.start: warning in assign("e", e, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.start: warning in assign("listOfTicks", listOfTicks, env =
  .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.start: warning in assign("relations", relations, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.start: warning in assign("row", row, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.start: warning in assign("sem.DPA", sem.DPA, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.start: warning in assign("sem.results.coefficients",
  sem.results.coefficients, env = .GlobalEnv): partial argument match
  of 'env' to 'envir'
dpa.start: warning in assign("sem.results.parameters",
  sem.results.parameters, env = .GlobalEnv): partial argument match of
  'env' to 'envir'
dpa.start: warning in assign("sem.results.statistics",
  sem.results.statistics, env = .GlobalEnv): partial argument match of
  'env' to 'envir'
dpa.start: warning in assign("sem.standardized", sem.standardized, env
  = .GlobalEnv): partial argument match of 'env' to 'envir'
dpa.start: warning in assign("variables", variables, env = .GlobalEnv):
  partial argument match of 'env' to 'envir'
dpa.start: warning in assign("dpa", dpa, env = .GlobalEnv): partial
  argument match of 'env' to 'envir'
dpa.analysis.options: no visible binding for global variable âeâ
dpa.analysis.options : OnOK : OnSave: no visible binding for global
  variable âeâ
dpa.analysis.performDPA : dpa.analysis.doPerform: no visible binding
  for global variable ârbValâ
dpa.analysis.performDPA : dpa.analysis.doPerform: no visible binding
  for global variable âvariablesâ
dpa.analysis.performDPA : dpa.analysis.doPerform: no visible binding
  for global variable âeâ
dpa.analysis.performDPA : dpa.analysis.doPerform: no visible binding
  for global variable âNumTickâ
dpa.analysis.performDPA: no visible binding for global variable ârbValâ
dpa.analysis.performDPA: no visible binding for global variable
  âsem.DPAâ
dpa.analysis.performDPA: no visible binding for global variable âeâ
dpa.analysis.saveDPA: no visible binding for global variable
  âdataFileNameâ
dpa.analysis.saveDPA: no visible binding for global variable
  âsem.results.coefficientsâ
dpa.data.authenticationCancel: no visible binding for global variable
  âak2â
dpa.data.authenticationSubmit: no visible binding for global variable
  âdbServerTypeâ
dpa.data.authenticationSubmit: no visible binding for global variable
  âdbServerâ
dpa.data.authenticationSubmit: no visible binding for global variable
  âdbTableâ
dpa.data.authenticationSubmit: no visible binding for global variable
  âUserNameâ
dpa.data.authenticationSubmit: no visible binding for global variable
  âPasswordâ
dpa.data.authenticationSubmit: no visible global function definition
  for âJDBCâ
dpa.data.authenticationSubmit: no visible global function definition
  for âdbConnectâ
dpa.data.authenticationSubmit: no visible global function definition
  for âdbGetQueryâ
dpa.data.authenticationSubmit: no visible global function definition
  for âdbReadTableâ
dpa.data.checkData : dpa.data.checkData.sort: no visible binding for
  global variable âeâ
dpa.data.checkData : dpa.data.missingRow: no visible binding for global
  variable âeâ
dpa.data.checkData : dpa.data.missingData: no visible binding for
  global variable âeâ
dpa.data.loadCancel: no visible binding for global variable âak1â
dpa.data.loadDataFromDatabase: no visible binding for global variable
  âdpa.data.authentificationCancelâ
dpa.data.loadDataFromDisk: no visible binding for global variable âak1â
dpa.data.saveDataToDisk: no visible binding for global variable âeâ
dpa.exit: no visible binding for global variable âdpaâ
dpa.relations.addRelations: no visible binding for global variable
  âdataframeâ
dpa.relations.editRelations: no visible binding for global variable âeâ
dpa.results.generateCoefficientsPlots : dpa.plot.graph: no visible
  binding for global variable âsem.results.coefficientsâ
dpa.results.generateCoefficientsPlots : dpa.plot.graph: no visible
  binding for global variable âsem.results.parametersâ
dpa.results.generateCoefficientsPlots : dpa.plot.graph: no visible
  binding for global variable âgraphDirâ
dpa.results.generateCoefficientsPlots : dpa.plot.graph: no visible
  binding for global variable âlistOfTicksâ
dpa.results.generateCoefficientsPlots : dpa.plot.graph: no visible
  binding for global variable âeâ
dpa.results.generateFitPlots : dpa.plot.graph: no visible binding for
  global variable âsem.results.statisticsâ
dpa.results.generateFitPlots : dpa.plot.graph: no visible binding for
  global variable âgraphDirâ
dpa.results.generateFitPlots : dpa.plot.graph: no visible binding for
  global variable âlistOfTicksâ
dpa.results.generateFitPlots : dpa.plot.graph: no visible binding for
  global variable âeâ
dpa.results.viewNodePlots: no visible binding for global variable âeâ
dpa.results.viewNodePlots : dpa.results.plotNodes : dpa.plot.scatter:
  no visible binding for global variable âgraphDirâ
dpa.results.viewNodePlots : dpa.results.plotNodes: no visible binding
  for global variable âeâ
dpa.results.viewNodePlots : dpa.results.plotNodesWithTime: no visible
  binding for global variable âeâ
dpa.results.viewNodePlots : dpa.results.plotNodesWithTime :
  dpa.plot.scatter: no visible binding for global variable âgraphDirâ
dpa.results.viewRelationsPlots : dpa.plot.graph: no visible binding for
  global variable ârbValâ
dpa.results.viewRelationsPlots : dpa.plot.graph: no visible binding for
  global variable âgraphDirâ
dpa.results.viewRelationsPlots : dpa.plot.graph: no visible binding for
  global variable âsem.standardizedâ
dpa.results.viewRelationsPlots : dpa.plot.graph: no visible global
  function definition for âplot.igraphâ
dpa.results.viewRelationsPlots: no visible binding for global variable
  âvariablesâ
dpa.results.viewRelationsPlots: no visible binding for global variable
  âeâ

Found the following assignments to the global environment:
File âdpa/R/dpa.râ:
  assign("ak1", ak1, env = .GlobalEnv)
  assign("dataFileName", dataFileName, env = .GlobalEnv)
  assign("e", e, env = .GlobalEnv)
  assign("e", e, env = .GlobalEnv)
  assign("e", e, env = .GlobalEnv)
  assign("ak2", ak2, env = .GlobalEnv)
  assign("dbServerType", dbServerType, env = .GlobalEnv)
  assign("dbServer", dbServer, env = .GlobalEnv)
  assign("dbName", dbName, env = .GlobalEnv)
  assign("dbTable", dbTable, env = .GlobalEnv)
  assign("UserName", UserName, env = .GlobalEnv)
  assign("Password", Password, env = .GlobalEnv)
  assign("relations", relations, env = .GlobalEnv)
  assign("relations", relations, env = .GlobalEnv)
  assign("dataframe", dataframe, env = .GlobalEnv)
  assign("relations", relations, env = .GlobalEnv)
  assign("time_column", time_column, env = .GlobalEnv)
  assign("e", e, env = .GlobalEnv)
  assign("i", i, env = .GlobalEnv)
  assign("rbVal", rbVal, env = .GlobalEnv)
  assign("time_column", time_column, env = .GlobalEnv)
  assign("intervalVal", intervalVal, env = .GlobalEnv)
  assign("NumTick", NumTick, env = .GlobalEnv)
  assign("dpaFileName", dpaFileName, env = .GlobalEnv)
  assign("e", e, env = .GlobalEnv)
  assign("listOfTicks", listOfTicks, env = .GlobalEnv)
  assign("relations", relations, env = .GlobalEnv)
  assign("row", row, env = .GlobalEnv)
  assign("sem.DPA", sem.DPA, env = .GlobalEnv)
  assign("sem.results.coefficients", sem.results.coefficients, 
    env = .GlobalEnv)
  assign("sem.results.parameters", sem.results.parameters, env = .GlobalEnv)
  assign("sem.results.statistics", sem.results.statistics, env = .GlobalEnv)
  assign("sem.standardized", sem.standardized, env = .GlobalEnv)
  assign("variables", variables, env = .GlobalEnv)
  assign("dpa", dpa, env = .GlobalEnv)
File âdpa/R/plot.râ:
  assign("graphDir", graphDir, env = .GlobalEnv)
File âdpa/R/sem.râ:
  assign("row", row, env = .GlobalEnv)
  assign("variables", baseVariables, env = .GlobalEnv)
  assign("sem", sem, env = .GlobalEnv)
  assign("sem.DPA", sem.DPA, env = .GlobalEnv)
  assign("sem.standardized", sem.standardized, env = .GlobalEnv)
  assign("relevantData", relevantData, env = .GlobalEnv)
  assign("sem.DPA", sem.DPA, env = .GlobalEnv)
  assign("sem.results.coefficients", sem.results.coefficients, 
    env = .GlobalEnv)
  assign("sem.results.parameters", sem.results.parameters, env = .GlobalEnv)
  assign("sem.standardized", sem.standardized, env = .GlobalEnv)
  assign("sem.results.statistics", sem.results.statistics, env = .GlobalEnv)
  assign("listOfTicks", listOfTicks, env = .GlobalEnv)
  assign("listOfTicks", NULL, env = .GlobalEnv)
  assign("sem.DPA", NULL, env = .GlobalEnv)
  assign("sem.standardized", NULL, env = .GlobalEnv)
  assign("sem.results.parameters", NULL, env = .GlobalEnv)
  assign("sem.results.statistics", NULL, env = .GlobalEnv)
  assign("sem.results.coefficients", NULL, env = .GlobalEnv)

Found the following calls to attach():
File âdpa/R/dpa.râ:
  attach(dataframe)
  attach(dataframe)
  attach(dataframe)
  attach(dataframe)
File âdpa/R/plot.râ:
  attach(dataframe)
  attach(dataframe)
  attach(dataframe)
See section âGood practiceâ in â?attachâ.
```
```
checking Rd line widths ... NOTE
Rd file 'dpa.generate.lag.Rd':
  \usage lines wider than 90 characters:
     dpa.generate.lag(dataframe = NULL, tickColumn = NULL, sourceColumn = NULL, minLag=1,maxLag=1)

Rd file 'dpa.relations.addRelations.Rd':
  \usage lines wider than 90 characters:
     dpa.relations.addRelations(From_column = NULL, To_column = NULL, Lag_in = NULL, minLag = NULL, maxLag = NULL, Direction = NULL)

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 2 NOTEs
```

## dynatopmodel (1.0)
Maintainer: Peter Metcalfe <p.metcalfe@lancaster.ac.uk>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
DisplayObservedFlows: no visible global function definition for
  âplot.zooâ
GetTimeSeriesInputRange: no visible global function definition for
  âindexâ
RunTOPMODEL: no visible global function definition for âindexâ
SpatialLinesDataFrameToIgraph: no visible global function definition
  for âgraph.data.frameâ
aggregate.qobs: no visible global function definition for âzooâ
aggregate.xts: no visible global function definition for âis.zooâ
aggregate.xts: no visible global function definition for âzooâ
allocate.rain: no visible global function definition for âindexâ
disaggregate.xts: no visible global function definition for âis.zooâ
disaggregate.xts: no visible global function definition for âindexâ
disaggregate.xts: no visible global function definition for âcoredataâ
disp.discharge.selection: no visible global function definition for
  âindexâ
disp.discharges: no visible global function definition for âplot.zooâ
disp.qsim: no visible global function definition for âplot.zooâ
disp.rain: no visible global function definition for âplot.zooâ
fix.obs: no visible global function definition for âna.approxâ
fix.run.dates: no visible global function definition for âindexâ
get.obs: no visible global function definition for âis.zooâ
gof.run: no visible global function definition for âindexâ
init.input: no visible global function definition for âindexâ
read.obs: no visible global function definition for âindexâ
report.series: no visible global function definition for âis.zooâ
report.series: no visible global function definition for âindexâ
subset.zoo: no visible global function definition for âis.zooâ
subset.zoo: no visible global function definition for âindexâ
time.interval.intersection: no visible global function definition for
  âindexâ
write.obs: no visible global function definition for âindexâ
write.proj: no visible global function definition for âwrite.zooâ
```
```
DONE
Status: 2 NOTEs
```

## enaR (2.8.1)
Maintainer: Matthew K. Lau <enaR.maintainer@gmail.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
DONE
Status: 1 NOTE
```

## ESEA (1.0)
Maintainer: Xinrui Shi <xinrui103@163.com>

```
checking package dependencies ... ERROR
Package suggested but not available: âgraphâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## fanovaGraph (1.4.7)
Maintainer: Jana Fruth <fruth@statistik.tu-dortmund.de>

```
checking dependencies in R code ... NOTE
'library' or 'require' calls in package code:
  âmanipulateâ âtcltkâ
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.graphlist print.graphlist
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
plotTk: no visible global function definition for âtclVarâ
plotTk : refresh: no visible global function definition for âtclvalueâ
plotTk: no visible global function definition for âtktoplevelâ
plotTk: no visible global function definition for âtkwm.titleâ
plotTk: no visible global function definition for âtkframeâ
plotTk: no visible global function definition for âtkscaleâ
plotTk: no visible global function definition for âtkpackâ
plotTk: no visible global function definition for âtklabelâ
```
```
checking examples ... ERROR
Running examples in âfanovaGraph-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: estimateGraph
> ### Title: FANOVA graph estimation.
> ### Aliases: estimateGraph print.graphlist
> 
> ### ** Examples
> 
> # Ishigami function, true analytical values: D12 = D23 = 0, D13 =~ 3.374
> q.arg = list(list(min=-pi, max=pi), list(min=-pi, max=pi), list(min=-pi, max=pi)) 
> estimateGraph(f.mat=ishigami.fun, d=3, q.arg=q.arg, n.tot=10000, method="LiuOwen")
Error in graph(as.vector(t(E)), d, FALSE) : Extra arguments in make_graph
Calls: estimateGraph ... maximal.cliques -> is_igraph -> %in% -> match -> graph
Execution halted
```
```
checking tests ... ERROR
Running the tests in âtests/run-all.Râ failed.
Last 13 lines of output:
  11: stop("Extra arguments in make_graph")
  
  testthat results ================================================================
  OK: 6 SKIPPED: 0 FAILED: 6
  1. Error: the full example works as before 
  2. Error: estimateGraph works for different n.tot and d for all methods 
  3. Error: estimateGraph works for very small values 
  4. Error: confint works for estimateGraph 
  5. Error: overall variance and standard sobol indices work 
  6. Error: thresholdIdentification works 
  
  Error: testthat unit tests failed
  Execution halted
```
```
DONE
Status: 2 ERRORs, 3 NOTEs
```

## fbRanks (2.0)
Maintainer: E Holmes <eeholmes@u.washington.edu>

```
checking dependencies in R code ... NOTE
'library' or 'require' calls in package code:
  âRCurlâ âRJSONIOâ âXMLâ âglmnetâ âhttrâ âspeedglmâ âtcltkâ âxtableâ
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
print.fbRanks: no visible global function definition for âxtableâ
rank.teams: no visible global function definition for âspeedglmâ
rank.teams: no visible global function definition for âsparseMatrixâ
rank.teams: no visible binding for global variable âglmnetâ
scrape.custom1: no visible global function definition for âhtmlParseâ
scrape.custom1: no visible global function definition for âgetNodeSetâ
scrape.custom1: no visible global function definition for âxmlValueâ
scrape.custom2: no visible global function definition for
  âreadHTMLTableâ
scrape.custom3: no visible global function definition for
  âreadHTMLTableâ
scrape.custom4: no visible global function definition for
  âreadHTMLTableâ
scrape.demosphere: no visible global function definition for
  âreadHTMLTableâ
scrape.demosphere : getthelink: no visible global function definition
  for âxmlChildrenâ
scrape.demosphere : getthelink: no visible global function definition
  for âxmlAttrsâ
scrape.demosphere: no visible global function definition for âgetURLâ
scrape.demosphere: no visible global function definition for
  âhtmlParseâ
scrape.demosphere.main : getthelink: no visible global function
  definition for âxmlChildrenâ
scrape.demosphere.main : getthelink: no visible global function
  definition for âxmlAttrsâ
scrape.demosphere.main : getthelink: no visible global function
  definition for âxmlValueâ
scrape.demosphere.main : getthelink3: no visible global function
  definition for âxmlChildrenâ
scrape.demosphere.main : getthelink3: no visible global function
  definition for âxmlAttrsâ
scrape.demosphere.main : getthelink3: no visible global function
  definition for âxmlValueâ
scrape.demosphere.main: no visible global function definition for
  âreadHTMLTableâ
scrape.gotsport: no visible global function definition for
  âreadHTMLTableâ
scrape.gotsport.main : getthelink: no visible global function
  definition for âxmlChildrenâ
scrape.gotsport.main : getthelink: no visible global function
  definition for âxmlAttrsâ
scrape.gotsport.main : getthelink: no visible global function
  definition for âxmlValueâ
scrape.gotsport.main: no visible global function definition for âGETâ
scrape.gotsport.main: no visible global function definition for
  âuser_agentâ
scrape.gotsport.main: no visible global function definition for
  âhtmlParseâ
scrape.gotsport.main: no visible global function definition for
  âtext_contentâ
scrape.gotsport.main: no visible global function definition for
  âreadHTMLTableâ
scrape.json1: no visible global function definition for âgetURLâ
scrape.json1: no visible global function definition for âfromJSONâ
scrape.korrio: no visible global function definition for âGETâ
scrape.korrio: no visible global function definition for âuser_agentâ
scrape.korrio: no visible global function definition for
  âreadHTMLTableâ
scrape.korrio: no visible global function definition for âtext_contentâ
scrape.korrio: no visible global function definition for âhtmlParseâ
scrape.korrio: no visible global function definition for âgetNodeSetâ
scrape.korrio: no visible binding for global variable âxmlValueâ
scrape.korrio: no visible global function definition for âxmlAttrsâ
scrape.korrio: no visible global function definition for âcontentâ
scrape.korrio: no visible global function definition for âxmlValueâ
scrape.scoreboard: no visible global function definition for
  âreadHTMLTableâ
scrape.sportaffinity: no visible global function definition for
  âreadHTMLTableâ
scrape.sportaffinity: no visible global function definition for
  âhtmlParseâ
scrape.sportaffinity: no visible global function definition for
  âgetNodeSetâ
scrape.sportaffinity: no visible binding for global variable âxmlValueâ
scrape.sportaffinity.brackets: no visible global function definition
  for âGETâ
scrape.sportaffinity.brackets: no visible global function definition
  for âuser_agentâ
scrape.sportaffinity.brackets: no visible global function definition
  for âhtmlParseâ
scrape.sportaffinity.brackets: no visible global function definition
  for âtext_contentâ
scrape.sportaffinity.brackets: no visible global function definition
  for âgetNodeSetâ
scrape.sportaffinity.brackets : <anonymous>: no visible global function
  definition for âxmlValueâ
scrape.sportaffinity.brackets: no visible global function definition
  for âxmlAttrsâ
scrape.sportaffinity.brackets: no visible global function definition
  for âxmlValueâ
scrape.sportaffinity.main : getthelink3: no visible global function
  definition for âxmlChildrenâ
scrape.sportaffinity.main : getthelink3: no visible global function
  definition for âxmlValueâ
scrape.sportaffinity.main : getthelink3: no visible global function
  definition for âxmlAttrsâ
scrape.sportaffinity.main: no visible global function definition for
  âreadHTMLTableâ
scrape.usclub: no visible global function definition for
  âreadHTMLTableâ
team.name.select : gogetem: no visible global function definition for
  âtclvalue<-â
team.name.select : gogetem: no visible global function definition for
  âtkcurselectionâ
team.name.select : clearteam: no visible global function definition for
  âtclvalue<-â
team.name.select : clearteam: no visible global function definition for
  âtkselection.clearâ
team.name.select : showteam: no visible global function definition for
  âtclvalue<-â
team.name.select : showteam: no visible global function definition for
  âtkcurselectionâ
team.name.select : showteam: no visible global function definition for
  âtclvalueâ
team.name.select : enterteam: no visible global function definition for
  âtclvalue<-â
team.name.select : enterteam: no visible global function definition for
  âtclvalueâ
team.name.select : updateteam: no visible global function definition
  for âtclvalue<-â
team.name.select : updateteam: no visible global function definition
  for âtkcurselectionâ
team.name.select : updateteam: no visible global function definition
  for âtclvalueâ
team.name.select : showlist: no visible global function definition for
  âtclvalue<-â
team.name.select : showlist: no visible global function definition for
  âtclvalueâ
team.name.select : searchteam: no visible global function definition
  for âtclvalue<-â
team.name.select : searchteam: no visible global function definition
  for âtclvalueâ
team.name.select : skipteam: no visible global function definition for
  âtclvalue<-â
team.name.select: no visible global function definition for
  âtktoplevelâ
team.name.select: no visible global function definition for
  âtkwm.titleâ
team.name.select: no visible global function definition for âtkframeâ
team.name.select: no visible global function definition for âtclVarâ
team.name.select: no visible global function definition for âtclObj<-â
team.name.select: no visible global function definition for âtklistboxâ
team.name.select: no visible global function definition for âtkpackâ
team.name.select: no visible global function definition for
  âtkradiobuttonâ
team.name.select: no visible global function definition for âtklabelâ
team.name.select: no visible global function definition for âtkentryâ
team.name.select: no visible global function definition for âtkbuttonâ
team.name.select: no visible global function definition for âtkgridâ
team.name.select: no visible global function definition for
  âtclvalue<-â
team.name.select : <anonymous>: no visible global function definition
  for âtkdestroyâ
team.name.select: no visible global function definition for
  âtkwait.windowâ
```
```
DONE
Status: 2 NOTEs
```

## FCMapper (1.0)
Maintainer: Shaun Turney <shaun.turney@mail.mcgill.ca>

```
checking examples ... ERROR
Running examples in âFCMapper-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: graph.fcm
> ### Title: Fuzzy cognitive map graph
> ### Aliases: graph.fcm
> 
> ### ** Examples
> 
> 
> matrix = matrix(nrow=7,ncol=7)
> matrix[1,] = c(0,-0.5,0,0,1,0,1)
> matrix[2,] = c(1,0,1,0.2,0,0,0.6)
> matrix[3,] = c(0,1,0,0,0,0,0)
> matrix[4,] = c(0.6,0,0,1,0,0,0.1)
> matrix[5,] = c(0,0.5,0,0,1,0,-0.6) 
> matrix[6,] = c(0,0,-1,0,0,0,0)
> matrix[7,] = c(0,0,0,-0.5,0,0,1)
> concept.names = c("A","B","C","D","E","F","G")
> 
> results = nochanges.scenario(matrix,iter=25,concept.names)
> 
> graph.fcm(matrix,concept.sizes=results$Equilibrium_value,concept.names)
Loading required package: tcltk
Error in .Call("R_igraph_layout_kamada_kawai", graph, coords, maxiter,  : 
  At structural_properties.c:4215 : Weight vector must be non-negative, Invalid value
Calls: graph.fcm ... params -> ret -> v -> layout_with_kk -> .Call -> <Anonymous>
Execution halted
```
```
DONE
Status: 1 ERROR
```

## FedData (1.1.0)
Maintainer: R. Kyle Bocinsky <bocinsky@gmail.com>

```
checking package dependencies ... ERROR
Packages suggested but not available: âSSOAPâ âXMLSchemaâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## FisHiCal (1.1)
Maintainer: Yoli Shavit <ys388@cam.ac.uk>

```
checking examples ... ERROR
Running examples in âFisHiCal-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: plotInc
> ### Title: Plot a spatial inconsistency
> ### Aliases: plotInc
> 
> ### ** Examples
> 
>   data(spatialInc)
>   plotInc(1, spatialInc) # no plot since no spatial incosistency was detected
>   plotInc(167, spatialInc) 
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: plotInc ... as.igraph.vs -> inherits -> V -> update_vs_ref -> check_version
Execution halted
```
```
DONE
Status: 1 ERROR
```

## flare (1.5.0)
Maintainer: Xingguo Li <xingguo.leo@gmail.com>

```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.slim
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
DONE
Status: 1 NOTE
```

## FrF2 (1.7-1)
Maintainer: Ulrike Groemping <groemping@beuth-hochschule.de>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âFrF2.catlg128â in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking Rd cross-references ... WARNING
Package unavailable to check Rd xrefs: âDoE.wrapperâ
Missing link or links in documentation object 'CIG.Rd':
  â[igraph]{layout}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
DONE
Status: 1 WARNING, 1 NOTE
```

## fuzzyMM (1.0.1)
Maintainer: Nikolai Gorte <n.gorte@gmail.com>

```
checking whether package âfuzzyMMâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by ârgeos::unionâ when loading âfuzzyMMâ
See â/Users/gaborcsardi/works/igraph/revdep_check/fuzzyMM.Rcheck/00install.outâ for details.
```
```
checking R code for possible problems ... NOTE
create_drn: no visible global function definition for âgetURLâ
create_drn: no visible global function definition for âxmlParseâ
err_region: no visible global function definition for âcoordinates<-â
err_region: no visible global function definition for âproj4string<-â
err_region: no visible global function definition for âCRSâ
err_region: no visible global function definition for âspTransformâ
err_region: no visible global function definition for âcoordinatesâ
err_region: no visible global function definition for âPolygonsâ
err_region: no visible global function definition for âPolygonâ
err_region: no visible global function definition for âSpatialPolygonsâ
imp : <anonymous>: no visible global function definition for
  âdist2Lineâ
lines2segments: no visible global function definition for âcoordinatesâ
lines2segments: no visible global function definition for âLinesâ
lines2segments: no visible global function definition for âLineâ
lines2segments: no visible global function definition for
  âSpatialLinesâ
mm: no visible global function definition for âproj4stringâ
mm: no visible global function definition for âspTransformâ
mm: no visible global function definition for âdist2Lineâ
mm: no visible global function definition for âSpatialPointsDataFrameâ
smp1: no visible global function definition for âbearingâ
smp1: no visible global function definition for âspDistsâ
smp2 : <anonymous>: no visible global function definition for
  âdist2Lineâ
smp2: no visible global function definition for âspDistsâ
smp2 : <anonymous>: no visible global function definition for âspDistsâ
```
```
DONE
Status: 1 WARNING, 1 NOTE
```

## G1DBN (3.1.1)
Maintainer: Sophie Lebre <sophie.lebre@icube.unistra.fr>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âMASSâ âigraphâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
DBNScoreStep1: no visible global function definition for ârlmâ
DBNScoreStep2: no visible global function definition for ârlmâ
```
```
DONE
Status: 3 NOTEs
```

## gemtc (0.6-2)
Maintainer: Gert van Valkenhoef <g.h.m.van.valkenhoef@rug.nl>

```
checking package dependencies ... ERROR
Package suggested but not available: âBRugsâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## GeneReg (1.1.2)
Maintainer: Tao Huang <huangtao@sibs.ac.cn>

```
checking dependencies in R code ... NOTE
'library' or 'require' calls to packages already attached by Depends:
  âigraphâ âsplinesâ
  Please remove these calls from your code.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.GeneReg
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
Found an obsolete/platform-specific call in the following function:
  âtimedelay.lmâ
Found the platform-specific device:
  âx11â
dev.new() is the preferred way to open a new device, in the unlikely
event one is needed.
plot.GeneReg: no visible global function definition for âplot.igraphâ
```
```
checking Rd files ... NOTE
prepare_Rd: GeneReg-package.Rd:12-13: Dropping empty section \usage
prepare_Rd: GeneReg-package.Rd:14-15: Dropping empty section \arguments
```
```
DONE
Status: 4 NOTEs
```

## gRain (1.2-3)
Maintainer: Søren Højsgaard <sorenh@math.aau.dk>

```
checking package dependencies ... ERROR
Package required but not available: âgraphâ

Package suggested but not available: âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## gRapfa (1.0)
Maintainer: Smitha Ankinakatte <Smitha.AA@agrsci.dk>

```
checking examples ... ERROR
Running examples in âgRapfa-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: KL
> ### Title: Kullback-Leibler divergence for APFA models
> ### Aliases: KL
> 
> ### ** Examples
> 
> library(gRapfa)
> data(Wheeze)
> samp <- sample(1:537, 250)
> G <- select.IC(Wheeze[samp,])
Error in NS[as.matrix(ftsc[, c(1, 3)])] <- ftsc[, 2] : 
  subscript out of bounds
Calls: select.IC -> apfa2NS
Execution halted
```
```
DONE
Status: 1 ERROR
```

## gRbase (1.7-0.1)
Maintainer: Søren Højsgaard <sorenh@math.aau.dk>

```
checking package dependencies ... ERROR
Packages required but not available: âRBGLâ âgraphâ âRcppEigenâ

Package suggested but not available: âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## gRim (0.1-17)
Maintainer: Søren Højsgaard <sorenh@math.aau.dk>

```
checking package dependencies ... ERROR
Package suggested but not available: âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## gromovlab (0.6-16)
Maintainer: Volkmar Liebscher <volkmar.liebscher@uni-greifswald.de>

```
checking whether package âgromovlabâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/gromovlab.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## huge (1.2.6)
Maintainer: Tuo Zhao <tzhao5@jhu.edu>

```
checking compiled code ... NOTE
File âhuge/libs/huge.soâ:
  Found â_randâ, possibly from ârandâ (C)
    Object: âSFGen.oâ
  Found â_srandâ, possibly from âsrandâ (C)
    Object: âSFGen.oâ

Compiled code should not call entry points which might terminate R nor
write to stdout/stderr instead of to the console, nor the system RNG.

See âWriting portable packagesâ in the âWriting R Extensionsâ manual.
```
```
DONE
Status: 1 NOTE
```

## igraphtosonia (1.0)
Maintainer: Sean J Westwood <seanjw@stanford.edu>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
DONE
Status: 1 NOTE
```

## InteractiveIGraph (1.0.6.1)
Maintainer: Vygantas Butkus <Vygantas.Butkus@gmail.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking Rd line widths ... NOTE
Rd file 'InteractiveIGraph.Rd':
  \examples lines wider than 100 characters:
     # this is an 'InteractiveIGraph' object, up till now there is not much difference. Just some extra attributes.

Rd file 'MenuAddItems.Rd':
  \examples lines wider than 100 characters:
       Item = list(list(label=msg, RegionParams=list(XBufCof = 0, YBufCof=0.2), RecParams=list(lwd = NA, border=NA), TextParams=list(cex=0.8 ... [TRUNCATED]

These lines will be truncated in the PDF manual.
```
```
checking examples ... ERROR
Running examples in âInteractiveIGraph-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: InteractiveIGraph-package
> ### Title: Interactive igraph
> ### Aliases: InteractiveIGraph-package
> 
> ### ** Examples
> 
> 
> 
> # this is a regular igraph object
> gOrg <- erdos.renyi.game(15, 1/10,  directed = TRUE)
> plot(gOrg) 
> 
> # this is an 'InteractiveIGraph' object, up till now there is not much difference. 
> # Just some extra attributes.
> g = InteractiveIGraph.Constructor(gOrg)
> g = plot(g) 
Error in do.call("plot.igraph", args = PlotParam) : 
  could not find function "plot.igraph"
Calls: plot -> plot.InteractiveIGraph -> do.call
Execution halted
```
```
DONE
Status: 1 ERROR, 2 NOTEs
```

## intergraph (2.0-1)
Maintainer: Michal Bojanowski <m.bojanowski@icm.edu.pl>

```
checking examples ... ERROR
Running examples in âintergraph-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: asDF
> ### Title: Convert network to data frame(s)
> ### Aliases: asDF asDF.igraph asDF.network
> 
> ### ** Examples
> 
> # using method for 'network' objects
> d1 <- asDF(exNetwork)
> str(d1)
List of 2
 $ edges   :'data.frame':	11 obs. of  4 variables:
  ..$ V1   : int [1:11] 2 3 4 5 6 8 10 11 14 12 ...
  ..$ V2   : int [1:11] 1 1 1 1 7 9 11 12 12 13 ...
  ..$ label: chr [1:11] "ba" "ca" "da" "ea" ...
  ..$ na   : logi [1:11] FALSE FALSE FALSE FALSE FALSE FALSE ...
 $ vertexes:'data.frame':	15 obs. of  4 variables:
  ..$ intergraph_id: int [1:15] 1 2 3 4 5 6 7 8 9 10 ...
  ..$ label        : chr [1:15] "a" "b" "c" "d" ...
  ..$ na           : logi [1:15] FALSE FALSE FALSE FALSE FALSE FALSE ...
  ..$ vertex.names : chr [1:15] "a" "b" "c" "d" ...
> 
> # using method for 'igraph' objects
> d2 <- asDF(exIgraph)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: asDF ... as.igraph.es -> inherits -> E -> update_es_ref -> check_version
Execution halted
```
```
checking tests ... ERROR
Running the tests in âtests/testall.Râ failed.
Last 13 lines of output:
  8: dumpAttr(object, "edge")
  9: dumpAttr.igraph(object, "edge")
  10: lapply(nams, function(a) igraph::get.edge.attribute(x, a))
  11: FUN(X[[i]], ...)
  12: igraph::get.edge.attribute(x, a)
  13: as.igraph.es(graph, index)
  14: inherits(e, "igraph.es")
  15: E(graph)
  16: update_es_ref(graph)
  17: check_version(graph)
  18: stop("This graph was created by an old(er) igraph version.\n", "  Call upgrade_graph() on it to use with the current igraph version")
  Error: Test failures
  Execution halted
```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Quitting from lines 99-100 (howto.Rmd) 
Error: processing vignette 'howto.Rmd' failed with diagnostics:
This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
DONE
Status: 2 ERRORs, 1 NOTE
```

## iRefR (1.13)
Maintainer: Antonio Mora <antoniocmora@gmail.com>

```
checking package dependencies ... ERROR
Packages required but not available: âgraphâ âRBGLâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## JGL (2.3)
Maintainer: Patrick Danaher <pdanaher@uw.edu>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ which was already attached by Depends.
  Please remove these calls from your code.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.jgl print.jgl
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking Rd line widths ... NOTE
Rd file 'JGL.Rd':
  \usage lines wider than 90 characters:
     JGL(Y,penalty="fused",lambda1,lambda2,rho=1,weights="equal",penalize.diagonal=FALSE,maxiter=500,tol=1e-5,warm=NULL,return.whole.theta=F ... [TRUNCATED]

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 3 NOTEs
```

## kknn (1.2-5)
Maintainer: Klaus Schliep <klaus.schliep@gmail.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
DONE
Status: 1 NOTE
```

## knitrBootstrap (0.9.0)
Maintainer: Jim Hester <james.f.hester@gmail.com>  
Bug reports: https://github.com/jimhester/knitrBootstrap/issues

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
DONE
Status: 1 NOTE
```

## lava (1.4.0)
Maintainer: Klaus K. Holst <klaus@holst.it>

```
checking package dependencies ... ERROR
Packages suggested but not available: âgraphâ âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## lcd (0.7-3)
Maintainer: Zongming Ma <zongming.ma@gmail.com>

```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âigraphâ âmethodsâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
.break.tree: no visible global function definition for
  âgraph.adjacencyâ
.break.tree: no visible global function definition for âclustersâ
.lcd.cliques: no visible global function definition for
  âgraph.adjacencyâ
.lcd.cliques: no visible global function definition for âcliquesâ
.valid.tree: no visible global function definition for
  âgraph.adjacencyâ
.valid.tree: no visible global function definition for âclustersâ
draw: no visible global function definition for âgraph.emptyâ
draw: no visible global function definition for âadd.verticesâ
draw: no visible global function definition for âVâ
draw: no visible global function definition for âV<-â
draw: no visible global function definition for âadd.edgesâ
draw: no visible global function definition for âplot.igraphâ
draw: no visible global function definition for âtkplotâ
draw: no visible binding for global variable âlayout.reingold.tilfordâ
is.chaingraph: no visible global function definition for
  âgraph.adjacencyâ
is.chaingraph: no visible global function definition for âclustersâ
```
```
DONE
Status: 2 NOTEs
```

## locits (1.4)
Maintainer: Guy Nason <g.p.nason@bristol.ac.uk>

```
checking dependencies in R code ... NOTE
Packages in Depends field not imported from:
  âigraphâ âwavethreshâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
AutoBestBW : specerr: no visible global function definition for
  âaccessDâ
HwdS: no visible global function definition for âIsPowerOfTwoâ
HwdS: no visible global function definition for âwdâ
HwdS: no visible global function definition for âputDâ
Rvarlacf: no visible global function definition for âPsiJâ
Rvarlacf: no visible global function definition for âipndacwâ
Rvarlacf: no visible global function definition for âPsiJmatâ
ewspec3: no visible binding for global variable âmadmadâ
ewspec3: no visible binding for global variable âl2normâ
ewspec3: no visible global function definition for âIsPowerOfTwoâ
ewspec3: no visible global function definition for âwdâ
ewspec3: no visible global function definition for âLocalSpecâ
ewspec3: no visible global function definition for âipndacwâ
ewspec3: no visible global function definition for âaccessDâ
ewspec3: no visible global function definition for âwstâ
ewspec3: no visible global function definition for âthreshold.wstâ
ewspec3: no visible global function definition for âAvBasisâ
ewspec3: no visible global function definition for âputDâ
ewspecHaarNonPer: no visible binding for global variable âmadmadâ
ewspecHaarNonPer: no visible binding for global variable âl2normâ
ewspecHaarNonPer: no visible global function definition for âLocalSpecâ
ewspecHaarNonPer: no visible global function definition for âipndacwâ
ewspecHaarNonPer: no visible global function definition for âaccessDâ
ewspecHaarNonPer: no visible global function definition for âwstâ
ewspecHaarNonPer: no visible global function definition for
  âthreshold.wstâ
ewspecHaarNonPer: no visible global function definition for âAvBasisâ
ewspecHaarNonPer: no visible global function definition for âputDâ
hwtos2: no visible global function definition for âPsiJâ
hwtos2: no visible global function definition for âPsiJmatâ
hwtos2: no visible global function definition for âaccessDâ
hwtos2: no visible global function definition for âwdâ
hwtos2: no visible global function definition for âputDâ
lacf: no visible global function definition for âPsiJmatâ
littlevar: no visible global function definition for âaccessDâ
mkcoef: no visible global function definition for âwdâ
mkcoef: no visible global function definition for âwrâ
mkcoef: no visible global function definition for âguyrotâ
plot.tos: no visible global function definition for âIsPowerOfTwoâ
runmean: no visible global function definition for ârunning.meanâ
summary.tos: no visible global function definition for âaccessDâ
whichlevel: no visible global function definition for âwdâ
whichlevel: no visible global function definition for âwrâ
```
```
DONE
Status: 2 NOTEs
```

## loe (1.0)
Maintainer: Yoshikazu Terada <terada@sigmath.es.osaka-u.ac.jp>

```
checking whether package âloeâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âvegan::diversityâ when loading âloeâ
See â/Users/gaborcsardi/works/igraph/revdep_check/loe.Rcheck/00install.outâ for details.
```
```
checking examples ... ERROR
Running examples in âloe-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: LOE
> ### Title: LOE for a unweighted Graph.
> ### Aliases: LOE
> 
> ### ** Examples
> 
> #################
> #Realizable case#
> #################
> ###############################
> #Create a toy data
> x <- seq(-5,5,by=1)
> y <- seq(1,6,by=1)
> hx1 <- seq(-3.5,-1.5,by=0.5)
> hx2 <- seq(1.5,3.5,by=0.5)
> hy <- seq(2.5,4.5,by=0.5)
> D1 <- matrix(0,66,2)
> for(i in 1:11){
+ 	for(j in 1:6){
+ 		D1[i+11*(j-1),] <- c(x[i],y[j])
+ 	}
+ }
> D2n <- matrix(0,25,2)
> D2p <- matrix(0,25,2)
> for(i in 1:5){
+ 	for(j in 1:5){
+ 		D2n[i+5*(j-1),] <- c(hx1[i],hy[j])
+ 		D2p[i+5*(j-1),] <- c(hx2[i],hy[j])
+ 	}
+ }
> D2n <- D2n[-c(7,9,17,19),]
> D2p <- D2p[-c(7,9,17,19),]
> Data <- rbind(D1,D2n,D2p)
> Data <- scale(Data[order(Data[,1]),], scale=FALSE)
> N <- nrow(Data)
> #Visualization of the original data
> plot(Data,pch=20,xlab="",ylab="",cex=1,col=rainbow(N,start=.7,end=.9),
+ xlim=c(-7,7),ylim=c(-7,7),main="Original data")
> 
> #Creating a k-NN graph based on Data
> DM <- as.matrix(dist(Data))
> ADM <- make.kNNG(DM,k=25)
> 
> #plot of the adjacency matrix
> AADM <- ADM
> diag(AADM) <- NA
> image(AADM[N:1,],col=topo.colors(3),ann=FALSE,axes=FALSE)
> 
> #Apply some graph embedding methods
> LE <-spec.emb(A=ADM,2,norm=FALSE)
> result.LOE <- LOE(ADM=ADM,p=2,c=0.1,method="BFGS",report=1000,iniX=LE)
initial  value 590.780031 
final  value 0.000000 
converged
> 
> #Procrustes transform
> PLOE <- procrustes(Data,scale(result.LOE$X,scale=FALSE), scale = TRUE)$Yrot
> plot(PLOE,pch=20,xlab="",ylab="",cex=1,col=rainbow(N,start=.7,end=.9),
+ xlim=c(-7,7),ylim=c(-7,7),main="LOE")
> ###############################
> 
> #############
> #This function provide appropriate vectors of xlim and ylim
> #for given embedding matrix X.
> #############
> make.lim <- function(X){
+ 			mima <- matrix(0, 2,2)
+ 			mima[,1] <- apply(X, 2, min)
+ 			mima[,2] <- apply(X, 2, max)
+ 			han <- mima[,2] - mima[,1]
+ 			cent <-  (mima[,2] + mima[,1])/2
+ 			tmpr <- max(han)+max(han)*0.05
+ 			for(s in 1:2){
+ 				mima[s,] <- c(cent[s]-tmpr/2,cent[s]+tmpr/2)
+ 			}
+ 			return(mima)
+ 		}
> ##############################
> #Standered graph-drawing task#
> ##############################
> ###############################
> ADM <- as.matrix( get.adjacency(graph.famous("Thomassen")) )
> TG <- graph.adjacency(ADM)
> 
> #Apply some graph embedding methods
> LE <-spec.emb(A=ADM,2,norm=FALSE)
> KK <- layout.kamada.kawai(TG,maxiter=1000,start=LE)
Error in layout.kamada.kawai(TG, maxiter = 1000, start = LE) : 
  unused argument (start = LE)
Execution halted
```
```
DONE
Status: 1 ERROR, 1 WARNING
```

## markovchain (0.2.1)
Maintainer: Giorgio Alfredo Spedicato <spedicato_giorgio@yahoo.it>  
Bug reports: http://github.com/spedygiorgio/markovchain/issues

```
checking R code for possible problems ... NOTE
plot,markovchain-missing: no visible global function definition for
  âplot.igraphâ
```
```
checking running R code from vignettes ... ERROR
Errors in running code in vignettes:
when running code in âan_introduction_to_markovchain_package.Rnwâ
  ...

    union


> plot(mcWeather, layout = layout.fruchterman.reingold, 
+     main = "Weather transition matrix")

  When sourcing 'an_introduction_to_markovchain_package.R':
Error: could not find function "plot.igraph"
Execution halted

```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...

Attaching package: 'igraph'

The following objects are masked from 'package:stats':

    decompose, spectrum

The following object is masked from 'package:base':

    union


Error: processing vignette 'an_introduction_to_markovchain_package.Rnw' failed with diagnostics:
 chunk 13 (label = mcPlot) 
Error in plot(mcWeather, layout = layout.fruchterman.reingold, main = "Weather transition matrix") : 
  could not find function "plot.igraph"
Execution halted

```
```
DONE
Status: 1 ERROR, 2 NOTEs
```

## matie (1.2)
Maintainer: Hugh Murrell <hugh.murrell@gmail.com>

```
checking whether package âmatieâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/matie.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## micropan (1.0)
Maintainer: Lars Snipen <lars.snipen@nmbu.no>

```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.Binomix plot.Fasta plot.Panmat plot.Panpca plot.Pantree
  plot.Rarefac str.Binomix str.Fasta str.Panmat str.Panpca str.Pantree
  str.Rarefac summary.Binomix summary.Fasta summary.Panmat
  summary.Panpca summary.Pantree summary.Rarefac
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
DONE
Status: 1 NOTE
```

## miniCRAN (0.2.4)
Maintainer: Andrie de
 Vries <andrie@revolutionanalytics.com>  
Bug reports: https://github.com/RevolutionAnalytics/miniCRAN/issues

```
checking dependencies in R code ... NOTE
Missing or unexported object: âigraph::plot.igraphâ
```
```
checking examples ... ERROR
Running examples in âminiCRAN-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: makeDepGraph
> ### Title: Create dependency graph from available packages.
> ### Aliases: makeDepGraph
> 
> ### ** Examples
> 
> 
> 
> 
> availPkgs <- cranJuly2014
> 
> ## Not run: 
> ##D availPkgs <- pkgAvail(
> ##D   repos = c(CRAN="http://cran.revolutionanalytics.com"),
> ##D   type="source"
> ##D   )
> ## End(Not run)
> 
> 
> # Create dependency graph using stored database of available packages
> p <- makeDepGraph(
+   c("ggplot2", "forecast"), 
+   availPkgs = availPkgs
+ )
Loading required namespace: igraph
> 
> if(require(igraph)) plot(p)
Loading required package: igraph

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union

Error: 'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted
```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Quitting from lines 59-62 (miniCRAN-dependency-graph.rmd) 
Error: processing vignette 'miniCRAN-dependency-graph.rmd' failed with diagnostics:
'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted

```
```
DONE
Status: 1 ERROR, 2 NOTEs
```

## mlDNA (1.1)
Maintainer: Chuang Ma <chuangma2006@gmail.com>

```
checking package dependencies ... ERROR
Package suggested but not available: âGeneSelectorâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## modMax (1.0)
Maintainer: Maria Schelling <schelling.rmaintainer@vodafone.de>

```
checking whether package âmodMaxâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âgtools::permuteâ when loading âmodMaxâ
See â/Users/gaborcsardi/works/igraph/revdep_check/modMax.Rcheck/00install.outâ for details.
```
```
checking examples ... ERROR
Running examples in âmodMax-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: extremalOptimization
> ### Title: Extremal optimization (EO) algorithms
> ### Aliases: extremalOptimization pcseoss
> ### Keywords: Extremal Optimization Community Modularity Random Local
> ###   Search Agent Social Networks PCSEO-SS algorithm Community structure
> ###   Conflict pairwise constraints large-scale network
> 
> ### ** Examples
> 
> 
> #weighted network
> randomgraph <- erdos.renyi.game(10, 0.3, type="gnp",directed = FALSE, loops = FALSE)
> 
> #to ensure that the graph is connected
> vertices <- which(clusters(randomgraph)$membership==1)  
> graph <- induced.subgraph(randomgraph,vertices)
> graph <- set.edge.attribute(graph, "weight", value=runif(ecount(graph),0,1))
> 
> adj <- get.adjacency(graph, attr="weight")
> result <- extremalOptimization(adj)
Error in switch(mode, out = 1, `in` = 2, all = 3, total = 3) : 
  EXPR must be a length 1 vector
Calls: extremalOptimization ... callExtremalOptimization -> calculateLambda -> neighbors
Execution halted
```
```
DONE
Status: 1 ERROR, 1 WARNING
```

## mRMRe (2.0.5)
Maintainer: Benjamin Haibe-Kains <benjamin.haibe.kains@utoronto.ca>

```
checking R code for possible problems ... NOTE
visualize,mRMRe.Network: no visible global function definition for
  âplot.igraphâ
```
```
checking examples ... ERROR
Running examples in âmRMRe-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: visualize
> ### Title: mRMRe Network display
> ### Aliases: visualize visualize,mRMRe.Network-method
> ### Keywords: methods
> 
> ### ** Examples
> 
> set.thread.count(2)
[1] 2
> data(cgps)
> feature_data <- mRMR.data(data =  data.frame(cgps.ge))
> 
> # Build an mRMR-based network and display it
> network <- new("mRMRe.Network", data = feature_data, target_indices = c(1),
+ 				levels = c(3, 1), layers = 2)
> visualize(network)
Error in visualize(network) : could not find function "plot.igraph"
Calls: visualize -> visualize
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## nat (1.6.6)
Maintainer: Greg Jefferis <jefferis@gmail.com>  
Bug reports: https://github.com/jefferis/nat/issues

```
checking whether package ânatâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by ânabor::knnâ when loading ânatâ
See â/Users/gaborcsardi/works/igraph/revdep_check/nat.Rcheck/00install.outâ for details.
```
```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'ngraph.Rd':
  â[igraph]{attributes}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
checking examples ... ERROR
Running examples in ânat-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: MBL.surf
> ### Title: Surface object (hxsurf) for the left mushroom body in FCWB
> ###   template space
> ### Aliases: MBL.surf
> 
> ### ** Examples
> 
> plot3d(kcs20)
X Error of failed request:  BadDrawable (invalid Pixmap or Window parameter)
  Major opcode of failed request:  14 (X_GetGeometry)
  Resource id in failed request:  0x0
  Serial number of failed request:  708
  Current serial number in output stream:  708
```
```
checking tests ... ERROR
Running the tests in âtests/test-all.Râ failed.
Last 13 lines of output:
  4: graph(NULL, n = 1) at test-seglist.R:50
  5: stop("'edges' must be numeric of character")
  
  testthat results ================================================================
  OK: 642 SKIPPED: 0 FAILED: 5
  1. Failure (at test-neuroml-io.R#36): parse neuroml files 
  2. Failure (at test-ngraph.R#63): equivalence of seglist and swc methods for as.ngraph.neuron 
  3. Failure (at test-ngraph.R#64): equivalence of seglist and swc methods for as.ngraph.neuron 
  4. Failure (at test-ngraph.R#65): equivalence of seglist and swc methods for as.ngraph.neuron 
  5. Error: convert graph to seglist 
  
  Error: testthat unit tests failed
  Execution halted
```
```
DONE
Status: 2 ERRORs, 2 WARNINGs
```

## netassoc (0.4.3)
Maintainer: Benjamin Blonder <bblonder@gmail.com>

```
checking examples ... ERROR
Running examples in ânetassoc-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: makenetwork
> ### Title: Infer species-association network
> ### Aliases: makenetwork
> 
> ### ** Examples
> 
> # generate random data
> set.seed(1)
> nsp <- 10
> nsi <- 5
> m_obs <- floor(matrix(rgamma(nsp*nsi,shape=5),ncol=nsi,nrow=nsp))
> m_nul <- floor(matrix(rexp(nsp*nsi,rate=0.05),ncol=nsi,nrow=nsp))
> 
> n <- makenetwork(m_obs, m_nul, numnulls=50, plot=TRUE)
Generating null replicates........................................................done.
Calculating co-occurrence scores...1 2 0.022 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 3 0.044 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 4 0.067 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 5 0.089 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 6 0.111 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 7 0.133 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 8 0.156 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 9 0.178 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
1 10 0.200 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 3 0.222 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 4 0.244 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 5 0.267 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 6 0.289 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 7 0.311 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 8 0.333 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 9 0.356 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
2 10 0.378 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 4 0.400 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 5 0.422 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 6 0.444 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 7 0.467 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 8 0.489 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 9 0.511 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
3 10 0.533 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 5 0.556 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 6 0.578 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 7 0.600 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 8 0.622 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 9 0.644 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
4 10 0.667 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
5 6 0.689 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
5 7 0.711 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
5 8 0.733 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
5 9 0.756 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
5 10 0.778 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
6 7 0.800 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
6 8 0.822 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
6 9 0.844 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
6 10 0.867 obs. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .Warning in cor(x = veci_nul, y = vecj_nul, method = whichmethod) :
  the standard deviation is zero
. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
7 8 0.889 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
7 9 0.911 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
7 10 0.933 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
8 9 0.956 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
8 10 0.978 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
9 10 1.000 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. 
...done.
Calculating standardized effect sizes......done.
Applying kappa threshold......done.
Building network......done.
Error in .Call("R_igraph_layout_kamada_kawai", graph, coords, maxiter,  : 
  At structural_properties.c:4215 : Weight vector must be non-negative, Invalid value
Calls: makenetwork ... layout.auto -> layout_with_kk -> .Call -> <Anonymous>
Execution halted
```
```
DONE
Status: 1 ERROR
```

## netClass (1.2.1)
Maintainer: Yupeng Cun <yupeng.cun@gmail.com>

```
checking package dependencies ... ERROR
Packages required but not available: âAnnotationDbiâ âgraphâ âsamrâ

Packages suggested but not available: âBiobaseâ âKEGG.dbâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## netgen (1.1)
Maintainer: Jakob Bossek <j.bossek@gmail.com>  
Bug reports: https://github.com/jakobbossek/netgen/issues

```
checking whether package ânetgenâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âigraph::normalizeâ when loading ânetgenâ
  Warning: replacing previous import by âstringr::%>%â when loading ânetgenâ
See â/Users/gaborcsardi/works/igraph/revdep_check/netgen.Rcheck/00install.outâ for details.
```
```
DONE
Status: 1 WARNING
```

## netgsa (2.0)
Maintainer: Jing Ma <mjing@umich.edu>

```
checking examples ... ERROR
Running examples in ânetgsa-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: NetGSA
> ### Title: Network-based Gene Set Analysis
> ### Aliases: NetGSA
> 
> ### ** Examples
> 
> set.seed(1)
> library(igraph)
> data(netgsaex)
> 
> A1 = netgsaex$A1
> A2 = netgsaex$A2
> B = netgsaex$B
> x = netgsaex$x
> y = netgsaex$y
> 
> ##Visualize the networks
> par(mar = c(0.5, 0.5, 3, 0.5))
> plot(netgsaex$g.alt, vertex.size = 5, vertex.label = NA, main="Network - alt")
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: plot ... as.igraph.es -> inherits -> E -> update_es_ref -> check_version
Execution halted
```
```
DONE
Status: 1 ERROR
```

## nets (0.1)
Maintainer: Christian Brownlees <christian.brownlees@upf.edu>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
checking dependencies in R code ... NOTE
Package in Depends field not imported from: âigraphâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
nets: no visible global function definition for âgraph.adjacencyâ
nets: no visible global function definition for âVâ
nets: no visible global function definition for âV<-â
```
```
DONE
Status: 3 NOTEs
```

## NetSim (0.9)
Maintainer: Christoph Stadtfeld <c.stadtfeld@rug.nl>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
Package in Depends field not imported from: âRcppâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  add_effect.AttributeMultinomialChoiceNetworkChangeModel
  add_effect.MultinomialChoiceNetworkChoiceChangeModel
  as.double.NetSimAttributeContainer as.matrix.NetSimNetwork
  as.numeric.NetSimAttributeContainer create_effect.AttributeEffect
  create_effect.AttributeOneModeNetworkEffect
  create_effect.MultiplexNetworkEffect
  create_effect.OneModeNetworkEffect
  create_effect.SimilarityAttributeOneModeNetworkEffect
  create_effect.UnknownType create_effect.character
  print.NetSimAttributeContainer print.NetSimNetwork
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking line endings in Makefiles ... NOTE
Found the following Makefile(s) without a final LF:
  src/Makevars
Some âmakeâ programs ignore lines not ending in LF.
```
```
checking for GNU extensions in Makefiles ... NOTE
GNU make is a SystemRequirements.
```
```
checking compiled code ... NOTE
File âNetSim/libs/NetSim.soâ:
  Found â_randâ, possibly from ârandâ (C)
    Object: âutils/Random.oâ
  Found â_srandâ, possibly from âsrandâ (C)
    Object: âutils/Random.oâ

Compiled code should not call entry points which might terminate R nor
write to stdout/stderr instead of to the console, nor the system RNG.

See âWriting portable packagesâ in the âWriting R Extensionsâ manual.
```
```
DONE
Status: 5 NOTEs
```

## nettools (1.0.1)
Maintainer: Michele Filosi <filosi@fbk.eu>

```
checking package dependencies ... ERROR
Packages required but not available: ârootSolveâ âdtwâ âWGCNAâ âminetâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## netweavers (1.1)
Maintainer: Elizabeth Ribble <emcclel3@msudenver.edu>

```
checking package dependencies ... ERROR
Packages required but not available: âBiocGenericsâ âBiobaseâ âlimmaâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## optrees (1.0)
Maintainer: Manuel Fontenla <manu.fontenla@gmail.com>

```
checking R code for possible problems ... NOTE
repGraph: no visible global function definition for âplot.igraphâ
```
```
checking examples ... ERROR
Running examples in âoptrees-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: getMinimumArborescence
> ### Title: Computes a minimum cost arborescence
> ### Aliases: getMinimumArborescence
> 
> ### ** Examples
> 
> # Graph
> nodes <- 1:4
> arcs <- matrix(c(1,2,2, 1,3,3, 1,4,4, 2,3,3, 2,4,4, 3,2,3,
+                  3,4,1, 4,2,1, 4,3,2),byrow = TRUE, ncol = 3)
> # Minimum cost arborescence
> getMinimumArborescence(nodes, arcs)

 Minimum cost spanning arborescence 
 Algorithm: Edmonds 
 Stages:  2 | Time:  0.005 
 ------------------------------
      head     tail    weight 
         1        3         3
         3        4         1
         4        2         1
 ------------------------------
                   Total = 5 

Error in repGraph(nodes, arcs, tree = msa$tree.arcs, directed = TRUE,  : 
  could not find function "plot.igraph"
Calls: getMinimumArborescence -> repGraph
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## osmar (1.1-7)
Maintainer: Thomas Schlesinger <tho.schlesinger@googlemail.com>

```
checking dependencies in R code ... NOTE
'library' or 'require' calls in package code:
  âigraphâ âspâ
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
as_igraph : <anonymous>: no visible global function definition for
  âdistHaversineâ
as_igraph: no visible global function definition for âgraph.edgelistâ
as_igraph: no visible global function definition for âEâ
as_igraph: no visible global function definition for âE<-â
as_sp_lines: no visible global function definition for âLinesâ
as_sp_points: no visible global function definition for
  âSpatialPointsDataFrameâ
as_sp_polygons: no visible global function definition for âPolygonsâ
as_sp_polygons: no visible global function definition for
  âSpatialPolygonsâ
as_sp_polygons: no visible global function definition for
  âSpatialPolygonsDataFrameâ
make_SLDF: no visible global function definition for âSpatialLinesâ
make_SLDF: no visible global function definition for
  âSpatialLinesDataFrameâ
osm_crs: no visible global function definition for âCRSâ
ways_nodes2Line: no visible global function definition for âLineâ
ways_nodes2Polygon: no visible global function definition for âPolygonâ
```
```
checking data for non-ASCII characters ... NOTE
  Note: found 80 marked UTF-8 strings
```
```
DONE
Status: 3 NOTEs
```

## outbreaker (1.1-5)
Maintainer: Thibaut Jombart <t.jombart@imperial.ac.uk>

```
checking whether package âoutbreakerâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/outbreaker.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## packdep (0.3.1)
Maintainer: Marco Scutari <marco.scutari@gmail.com>

```
checking package dependencies ... ERROR
Package suggested but not available: âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## PAGI (1.0)
Maintainer: Junwei Han <hanjunwei1981@163.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking R code for possible problems ... NOTE
CalGIF: no visible binding for global variable âPAGIDataâ
CalGIF2: no visible binding for global variable âPAGIDataâ
PAGI.Main: no visible binding for global variable âPAGIDataâ
getclass.labels: no visible binding for global variable âExampleDataâ
getdataset: no visible binding for global variable âExampleDataâ
```
```
checking Rd line widths ... NOTE
Rd file 'CalGIF.Rd':
  \examples lines wider than 100 characters:
     ###calculate the global influence factor (GIF) by using the random walk with restart (RWR) algorithm###
     #Each element is the GIF score and whose name correspond to gene symbol in the gene expression data. 
     #Each element is the GIF score and whose name correspond to gene symbol in the gene expression data. 

Rd file 'PAGI.Main.Rd':
  \examples lines wider than 100 characters:
     #Its columns include "Gene number in the (sorted) pathway", "gene symbol from the gene express data",
     #"location of the gene in the sorted gene list", "the T-score of gene between two biological states",
     #Its columns include "Gene number in the (sorted) pathway", "gene symbol from the gene express data",
     #"location of the gene in the sorted gene list", "the T-score of gene between two biological states",

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 3 NOTEs
```

## pathClass (0.9.4)
Maintainer: Marc Johannes <JohannesMarc@gmail.com>

```
checking package dependencies ... ERROR
Packages required but not available: âaffyâ âBiobaseâ

Packages suggested but not available: âhu6800.dbâ âgolubEsetsâ

Depends: includes the non-default packages:
  âsvmpathâ âkernlabâ âaffyâ âBiobaseâ âROCRâ âigraphâ âlpSolveâ
Adding so many packages to the search path is excessive and importing
selectively is preferable.

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## PBC (1.2)
Maintainer: Van Trung Pham <trungpv88@gmail.com>

```
checking examples ... ERROR
Running examples in âPBC-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: PBC-class
> ### Title: Class "PBC" for the PBC model
> ### Aliases: getRoot,PBC-method getGraph,PBC-method getF,PBC-method
> ###   getNIteration,PBC-method getDxf,PBC-method getDxdyf,PBC-method
> ###   getGraf,PBC-method getGradxf,PBC-method getGradxdyf,PBC-method
> ###   getBINMAT,PBC-method getModel,PBC-method setDensity,PBC-method
> ###   setGradient,PBC-method pbcPlot,PBC-method pbcPlot getDxdyf getDxf
> ###   getF getGradxdyf getGradxf getGraf setGradient setDensity
> ###   phi.student1 phi.student phi.norm margin compute gradxf2.student
> ###   gradxf.norm gradxdyphi2.student gradxdyphi.norm getModel getRoot
> ###   getNIteration getGraph dxf.student dxf.norm dxdyphi.student
> ###   dxdyphi.norm getBINMAT draw getBinMat pbc igraph-class PBC-class
> 
> ### ** Examples
> 
> ## PBC class information
> showClass("PBC")
Class "PBC" [package "PBC"]

Slots:
                                                                        
Name:        root      graph          f        dxf      dxdyf       graf
Class:  character     igraph expression expression expression expression
                                                                        
Name:      gradxf   gradxdyf     BINMAT      model    density   gradient
Class: expression expression     matrix  character    numeric     vector
                 
Name:  nIteration
Class:    numeric
> ## Create a PBC object with linking family "Gumbel"
> g <- graph.formula(X1-X3,X2-X3,X3-X4,X4-X5,simplify = FALSE)
> pbcObj <- pbc(g, model="gumbel")
Error in matrix(res, ncol = 2, byrow = TRUE) : 
  unimplemented type 'expression' in 'copyMatrix'
Calls: pbc ... as.igraph.es -> inherits -> na.omit -> E -> ends -> matrix
Execution halted
```
```
checking tests ... ERROR
Running the tests in âtests/optim.Râ failed.
Last 13 lines of output:
  > ## Parameters ##
  > ################
  > theta <- runif(4)
  > g <- graph.formula(X1-X4,X4-X2,X2-X3,X4-X5,simplify = FALSE)
  > 
  > ##########################
  > ## PBC objects Creation ##
  > ##########################
  > myPBCGumbel <- pbcGumbel(g)
  Error in matrix(res, ncol = 2, byrow = TRUE) : 
    unimplemented type 'expression' in 'copyMatrix'
  Calls: pbcGumbel ... as.igraph.es -> inherits -> na.omit -> E -> ends -> matrix
  Execution halted
```
```
checking running R code from vignettes ... ERROR
Errors in running code in vignettes:
when running code in âPBC.Rnwâ
  ...


> g <- graph.formula(X1 - X2, X2 - X3, X3 - X4, X4 - 
+     X5, simplify = FALSE)

> myPBC <- pbcGumbel(g)

  When sourcing âPBC.Râ:
Error: unimplemented type 'expression' in 'copyMatrix'
Execution halted

```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Loading required package: igraph

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union


Error: processing vignette 'PBC.Rnw' failed with diagnostics:
 chunk 3 
Error in matrix(res, ncol = 2, byrow = TRUE) : 
  unimplemented type 'expression' in 'copyMatrix'

Execution halted

```
```
DONE
Status: 3 ERRORs, 1 NOTE
```

## pcalg (2.2-0)
Maintainer: Markus Kalisch <kalisch@stat.math.ethz.ch>

```
checking package dependencies ... ERROR
Packages required but not available: âgraphâ âRBGLâ

Package suggested but not available: âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## PGRdup (0.2)
Maintainer: J. Aravind <aravindj@nbpgr.ernet.in>

```
checking Rd cross-references ... NOTE
Package unavailable to check Rd xrefs: âRecordLinkageâ
```
```
DONE
Status: 1 NOTE
```

## phangorn (1.99-13)
Maintainer: Klaus Schliep <klaus.schliep@gmail.com>

```
checking package dependencies ... ERROR
Package suggested but not available: âseqLogoâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## phyloTop (1.1.1)
Maintainer: Michael Boyd <mboyd855@gmail.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
DONE
Status: 1 NOTE
```

## popgraph (1.4)
Maintainer: Rodney J. Dyer <rjdyer@vcu.edu>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking examples ... ERROR
Running examples in âpopgraph-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: theme_empty
> ### Title: A blank theme for plotting networks
> ### Aliases: theme_empty
> 
> ### ** Examples
> 
> data(lopho)
> require(ggplot2)
> require(igraph)
> layout <- layout.fruchterman.reingold( lopho )
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: layout.fruchterman.reingold -> E -> update_es_ref -> check_version
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## poplite (0.99.16)
Maintainer: Daniel Bottomly <bottomly@ohsu.edu>

```
checking package dependencies ... ERROR
Package suggested but not available: âVariantAnnotationâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## poppr (1.1.5)
Maintainer: Zhian N. Kamvar <kamvarz@science.oregonstate.edu>  
Bug reports: https://github.com/grunwaldlab/poppr/issues

```
checking whether package âpopprâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/poppr.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## ppiPre (1.7)
Maintainer: Yue Deng <anfdeng@163.com>

```
checking package dependencies ... ERROR
Packages required but not available: âAnnotationDbiâ âGOSemSimâ âGO.dbâ

Packages which this enhances but not available for checking:
  âKEGG.dbâ âorg.Hs.eg.dbâ âorg.Sc.sgd.dbâ âorg.Ag.eg.dbâ
  âorg.Pt.eg.dbâ âorg.Rn.eg.dbâ âorg.Ss.eg.dbâ âorg.At.tair.dbâ
  âorg.Bt.eg.dbâ âorg.Ce.eg.dbâ âorg.Cf.eg.dbâ âorg.Dm.eg.dbâ
  âorg.Dr.eg.dbâ âorg.EcK12.eg.dbâ âorg.EcSakai.eg.dbâ âorg.Gg.eg.dbâ
  âorg.Mm.eg.dbâ âorg.Mmu.eg.dbâ âorg.Pf.plasmo.dbâ âorg.Xl.eg.dbâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## PROFANCY (1.0)
Maintainer: Qianlan Yao <yaoqianlan@yahoo.com>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ which was already attached by Depends.
  Please remove these calls from your code.
```
```
checking R code for possible problems ... NOTE
getCandidates: no visible binding for global variable âenvDataâ
getGraph: no visible binding for global variable âenvDataâ
getProvidedDiseaseName: no visible binding for global variable
  âenvDataâ
getSeed: no visible binding for global variable âenvDataâ
getTopDiseaseMetabolites: no visible binding for global variable
  âenvDataâ
```
```
checking running R code from vignettes ... ERROR
Errors in running code in vignettes:
when running code in âPROFANCY.Rnwâ
  ...

> diseaseName <- ProvidedDiseaseName[17]

> example1 <- getTopDiseaseMetabolites(diseaseName = diseaseName, 
+     network = "EHMN", seedDefault = TRUE, showTop = 30, candidateDefault = TRUE)

  When sourcing âPROFANCY.Râ:
Error: This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Loading required package: Matrix
Loading required package: lattice
Loading required package: igraph

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union


Error: processing vignette 'PROFANCY.Rnw' failed with diagnostics:
 chunk 3 
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
DONE
Status: 1 ERROR, 3 NOTEs
```

## qdap (2.2.1)
Maintainer: Tyler Rinker <tyler.rinker@gmail.com>  
Bug reports: http://github.com/trinker/qdap/issues

```
checking R code for possible problems ... NOTE
plot.cm_distance: no visible global function definition for
  âplot.igraphâ
print.Network: no visible global function definition for âplot.igraphâ
print.animated_discourse_map : <anonymous>: no visible global function
  definition for âplot.igraphâ
print.animated_formality : <anonymous>: no visible global function
  definition for âplot.igraphâ
print.animated_lexical_classification : <anonymous>: no visible global
  function definition for âplot.igraphâ
print.animated_polarity : <anonymous>: no visible global function
  definition for âplot.igraphâ
print.discourse_map: no visible global function definition for
  âplot.igraphâ
print.phrase_net: no visible global function definition for
  âplot.igraphâ
word_network_plot: no visible global function definition for
  âplot.igraphâ
```
```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'plot.cm_distance.Rd':
  â[igraph]{layout}â

Missing link or links in documentation object 'word_associate.Rd':
  â[igraph]{layout}â

Missing link or links in documentation object 'word_network_plot.Rd':
  â[igraph]{igraph.vertex.shapes}â â[igraph]{layout}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
DONE
Status: 1 WARNING, 1 NOTE
```

## qtlnet (1.3.6)
Maintainer: Brian S. Yandell <byandell@wisc.edu>

```
checking package dependencies ... ERROR
Package required but not available: âgraphâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## QuACN (1.8.0)
Maintainer: Karl G. Kugler <kg.kugler@gmail.com>

```
checking package dependencies ... ERROR
Packages required but not available: âgraphâ âRBGLâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## rags2ridges (1.4)
Maintainer: Carel F.W. Peeters <cf.peeters@vumc.nl>

```
checking examples ... ERROR
Running examples in ârags2ridges-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: GGMpathStats
> ### Title: Gaussian graphical model node pair path statistics
> ### Aliases: GGMpathStats
> 
> ### ** Examples
> 
> ## Obtain some (high-dimensional) data
> p = 25
> n = 10
> set.seed(333)
> X = matrix(rnorm(n*p), nrow = n, ncol = p)
> colnames(X)[1:25] = letters[1:25]
> 
> ## Obtain regularized precision under optimal penalty
> OPT <- optPenalty.LOOCVauto(X, lambdaMin = .5, lambdaMax = 30)
> 
> ## Determine support regularized standardized precision under optimal penalty
> PC0 <- sparsify(OPT$optPrec, threshold = "localFDR")$sparseParCor
Step 1... determine cutoff point
Step 2... estimate parameters of null distribution and eta0
Step 3... compute p-values and estimate empirical PDF/CDF
Step 4... compute q-values and local fdr
Step 5... prepare for plotting

- Retained elements:  11 
- Corresponding to 3.67 % of possible edges 
 
> 
> ## Obtain information on mediating and moderating paths between nodes 14 and 23
> pathStats <- GGMpathStats(PC0, 14, 23, verbose = TRUE, prune = FALSE)
Error in switch(mode, out = 1, `in` = 2, all = 3, total = 3) : 
  EXPR must be a length 1 vector
Calls: GGMpathStats -> neighbors
Execution halted
```
```
DONE
Status: 1 ERROR
```

## rbmn (0.9-2)
Maintainer: Jean-Baptiste Denis <Jean-Baptiste.Denis@jouy.inra.fr>

```
checking dependencies in R code ... NOTE
Package in Depends field not imported from: âMASSâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
bn2nbn: no visible binding for global variable âbn.fitâ
nbn2bnfit: no visible global function definition for âmodel2networkâ
nbn2bnfit: no visible global function definition for âcustom.fitâ
simulate8mn: no visible global function definition for âmvrnormâ
```
```
DONE
Status: 2 NOTEs
```

## RCA (1.4.5)
Maintainer: Yuan Wang <wangyuanvivien@post.harvard.edu>

```
checking whether package âRCAâ can be installed ... [70s/71s] WARNING
Found the following significant warnings:
  glpenv01.c:130:48: warning: incompatible integer to pointer conversion returning 'int' from a function with result type 'ENV *' (aka 'struct ENV *') [-Wint-conversion]
  glpenv01.c:138:43: warning: incompatible integer to pointer conversion returning 'int' from a function with result type 'ENV *' (aka 'struct ENV *') [-Wint-conversion]
See â/Users/gaborcsardi/works/igraph/revdep_check/RCA.Rcheck/00install.outâ for details.
```
```
checking top-level files ... NOTE
Non-standard files/directories found at top level:
  âmatrix.pmtâ âstack.pmtâ âvector.pmtâ
```
```
checking compiled code ... NOTE
File âRCA/libs/RCA.soâ:
  Found â_randâ, possibly from ârandâ (C)
    Objects: âRCAlib.oâ, âcs_randperm.oâ
  Found â_srandâ, possibly from âsrandâ (C)
    Objects: âRCAlib.oâ, âcs_randperm.oâ

Compiled code should not call entry points which might terminate R nor
write to stdout/stderr instead of to the console, nor the system RNG.

See âWriting portable packagesâ in the âWriting R Extensionsâ manual.
```
```
DONE
Status: 1 WARNING, 2 NOTEs
```

## RcmdrPlugin.RMTCJags (1.0)
Maintainer: Marcelo Goulart Correia <mgoulart.inc@gmail.com>

```
checking whether package âRcmdrPlugin.RMTCJagsâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/RcmdrPlugin.RMTCJags.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## RDS (0.7-2)
Maintainer: Mark S. Handcock <handcock@stat.ucla.edu>

```
checking dependencies in R code ... NOTE
Missing or unexported object: âigraph::plot.igraphâ
```
```
checking examples ... ERROR
Running examples in âRDS-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: read.rdsat
> ### Title: Import data from the 'RDSAT' format as an 'rds.data.frame'
> ### Aliases: read.rdsat
> 
> ### ** Examples
> 
> fn <- paste0(path.package("RDS"),"/extdata/nyjazz.rdsat")
> rd <- read.rdsat(fn)
> plot(rd)
Error: 'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## ReliabilityTheory (0.1.4)
Maintainer: Louis Aslett <aslett@stats.ox.ac.uk>

```
checking examples ... ERROR
Running examples in âReliabilityTheory-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: systemGraphToGenerator
> ### Title: Construct a Continuous-time Markov Chain Generator
> ### Aliases: systemGraphToGenerator
> ### Keywords: generator matrix system signature
> 
> ### ** Examples
> 
> # Get the generator representing a repairable 5 component 'bridge' system with
> # failure rate 1 and repair rate 365.
> data(sccsO5)
> G <- systemGraphToGenerator(sccsO5[[18]]$graph, 1, 365)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: systemGraphToGenerator -> V -> update_vs_ref -> check_version
Execution halted
```
```
DONE
Status: 1 ERROR
```

## rEMM (1.0-9)
Maintainer: Michael Hahsler <mhahsler@lyle.smu.edu>

```
checking package dependencies ... ERROR
Packages suggested but not available: âgraphâ âRgraphvizâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## restlos (0.1-3)
Maintainer: Steffen Liebscher <steffen.liebscher@wiwi.uni-halle.de>

```
checking whether package ârestlosâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âigraph::normalizeâ when loading ârestlosâ
See â/Users/gaborcsardi/works/igraph/revdep_check/restlos.Rcheck/00install.outâ for details.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  plot.flood plot.pMST plot.rdela
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
DONE
Status: 1 WARNING, 1 NOTE
```

## RevEcoR (0.99.2)
Maintainer: Yang Cao <yiluheihei@gmail.com>

```
checking whether package âRevEcoRâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/RevEcoR.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## rgp (0.4-1)
Maintainer: Oliver Flasch <oliver.flasch@fh-koeln.de>

```
checking dependencies in R code ... NOTE
'library' or 'require' call to âigraphâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
exprToIgraph: no visible global function definition for âgraphâ
exprToIgraph: no visible global function definition for âVâ
exprToIgraph: no visible global function definition for âV<-â
multiNicheGeneticProgramming: no visible binding for global variable
  âsfClusterApplyLBâ
multiNicheGeneticProgramming: no visible binding for global variable
  âsfExportâ
multiNicheSymbolicRegression: no visible binding for global variable
  âsfClusterApplyLBâ
multiNicheSymbolicRegression: no visible binding for global variable
  âsfExportâ
```
```
DONE
Status: 2 NOTEs
```

## RGraphics (2.0-12)
Maintainer: Paul Murrell <paul@stat.auckland.ac.nz>

```
checking package dependencies ... ERROR
Packages suggested but not available:
  âgraphâ âhyperdrawâ âhypergraphâ ârggobiâ âRgraphvizâ âSVGAnnotationâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## RNetLogo (1.0-1)
Maintainer: Jan C. Thiele <rnetlogo@gmx.de>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
DONE
Status: 1 NOTE
```

## ror (1.2)
Maintainer: Tommi Tervonen <tommi@smaa.fi>

```
checking dependencies in R code ... NOTE
Package in Depends field not imported from: âROI.plugin.glpkâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
Missing or unexported object: âigraph::plot.igraphâ
```
```
checking Rd line widths ... NOTE
Rd file 'utagms.Rd':
  \examples lines wider than 100 characters:
     stopifnot(necrel == matrix(c(TRUE, FALSE, FALSE, TRUE, TRUE, FALSE, TRUE, TRUE, TRUE), ncol=3, byrow=TRUE))
     stopifnot(posrel == matrix(c(TRUE, TRUE, FALSE, TRUE, TRUE, FALSE, TRUE, TRUE, TRUE), ncol=3, byrow=TRUE))
     necrel <- utagms(performances, strongPrefs=NULL, indifPrefs=strongPrefs, necessary=TRUE, strictVF=TRUE)

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 2 NOTEs
```

## rPref (0.5)
Maintainer: Patrick Roocks <mail@p-roocks.de>

```
checking for GNU extensions in Makefiles ... NOTE
GNU make is a SystemRequirements.
```
```
DONE
Status: 1 NOTE
```

## RQDA (0.2-7)
Maintainer: HUANG Ronggui <ronggui.huang@gmail.com>

```
checking package dependencies ... NOTE
Package which this enhances but not available for checking: ârjpodâ
```
```
checking whether package âRQDAâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/RQDA.Rcheck/00install.outâ for details.
Status: 1 ERROR, 1 NOTE
```

## rtop (0.3-45)
Maintainer: Jon Olav Skoien <jon.skoien@gmail.com>

```
checking dependencies in R code ... NOTE
'library' or 'require' calls in package code:
  âigraphâ âintamapâ
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking R code for possible problems ... NOTE
netProp: no visible global function definition for âgraph.data.frameâ
netProp: no visible global function definition for âtopological.sortâ
netProp: no visible global function definition for âVâ
netProp: no visible global function definition for âneighborsâ
```
```
DONE
Status: 2 NOTEs
```

## sand (1.0.2)
Maintainer: Gabor Csardi <csardi.gabor@gmail.com>  
Bug reports: https://github.com/kolaczyk/sand/issues

```
checking package dependencies ... ERROR
Packages suggested but not available: âGO.dbâ âGOstatsâ âorg.Sc.sgd.dbâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## SDDE (1.0.0)
Maintainer: Etienne Lord <m.etienne.lord@gmail.com>

```
checking examples ... ERROR
Running examples in âSDDE-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: complete_network
> ### Title: compare two given networks (original and augmented, presented as
> ###   undirected graphs) using a path analysis
> ### Aliases: complete_network
> 
> ### ** Examples
> 
> ## Searching the sample data (containing 11 original nodes and 3 augmented nodes)
> data(Sample_1)
> result <- complete_network(g1, g2)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: complete_network -> V -> update_vs_ref -> check_version
Execution halted
```
```
DONE
Status: 1 ERROR
```

## secrlinear (1.0.5)
Maintainer: Murray Efford <murray.efford@otago.ac.nz>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
checking examples ... ERROR
Running examples in âsecrlinear-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: Arvicola
> ### Title: Water Vole Capture Dataset
> ### Aliases: arvicola
> ### Keywords: datasets
> 
> ### ** Examples
> 
> 
> summary(arvicola)
Object class      capthist 
Detector type     multi 
Detector number   88 
Average spacing   19.80165 m 
x-range           163.85 835.61 m 
y-range           457.67 684.59 m 
Counts by occasion 
                   1  2  3  4  5  6 Total
n                 16 11 18 12 16 11    84
u                 16  2  6  1  1  0    26
f                  7  3  4  5  3  4    26
M(t+1)            16 18 24 25 26 26    26
losses             0  0  0  0  0  0     0
detections        16 11 18 12 16 11    84
detectors visited 16 11 18 12 16 11    84
detectors used    88 88 88 88 88 88   528

> head(traps(arvicola))
          x      y
0.A  164.86 609.69
0.B  164.86 609.69
20.A 163.85 629.66
20.B 163.85 629.66
40.A 164.88 649.19
40.B 164.88 649.19
> 
> ## for speed, pre-compute distance matrix
> userd <- networkdistance (traps(arvicola), glymemask, glymemask)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: networkdistance -> cbind -> V -> update_vs_ref -> check_version
Execution halted
```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Warning in engine$weave(file, quiet = quiet, encoding = enc) :
  The vignette engine knitr::rmarkdown is not available, because the rmarkdown package is not installed. Please install it.
Warning in in_dir(opts_knit$get("root.dir") %n% input_dir(), evaluate::evaluate(code,  :
  You changed the working directory to /Users/gaborcsardi/works/igraph/revdep_check/secrlinear.Rcheck/secrlinear/extdata (probably via setwd()). It will be restored to /Users/gaborcsardi/works/igraph/revdep_check/secrlinear.Rcheck/vign_test/secrlinear/vignettes. See the Note section in ?knitr::knit
Quitting from lines 72-74 (secrlinear-vignette.Rmd) 
Error: processing vignette 'secrlinear-vignette.Rmd' failed with diagnostics:
non-numeric argument to binary operator
Execution halted

```
```
DONE
Status: 1 ERROR, 2 NOTEs
```

## SEMID (0.1)
Maintainer: Mathias Drton <md5@uw.edu>

```
checking dependencies in R code ... NOTE
Package in Depends field not imported from: âigraphâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
graphID.genericID: no visible global function definition for
  âgraph.maxflowâ
graphID.genericID: no visible global function definition for
  âgraph.adjacencyâ
graphID.globalID: no visible global function definition for
  âgraph.maxflowâ
graphID.globalID: no visible global function definition for
  âgraph.adjacencyâ
graphID.nonID: no visible global function definition for
  âgraph.maxflowâ
graphID.nonID: no visible global function definition for
  âgraph.adjacencyâ
```
```
DONE
Status: 2 NOTEs
```

## semPlot (1.0.1)
Maintainer: Sacha Epskamp <mail@sachaepskamp.com>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
checking dependencies in R code ... NOTE
'library' or 'require' call to âMplusAutomationâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  semPlotModel.S4
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
semPlotModel.mplus.model: no visible global function definition for
  âreadModelsâ
```
```
DONE
Status: 4 NOTEs
```

## sensitivity (1.11.1)
Maintainer: Bertrand Iooss <biooss@yahoo.fr>

```
checking dependencies in R code ... NOTE
Missing or unexported object: âigraph::plot.igraphâ
```
```
DONE
Status: 1 NOTE
```

## SeqGrapheR (0.4.8.3)
Maintainer: Petr Novak <petr@umbr.cas.cz>

```
checking package dependencies ... ERROR
Packages required but not available: âBiostringsâ ârggobiâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## sglasso (1.2.1)
Maintainer: Luigi Augugliaro <luigi.augugliaro@unipa.it>

```
checking R code for possible problems ... NOTE
gplot.fglasso: no visible global function definition for âplot.igraphâ
gplot.sglasso: no visible global function definition for âplot.igraphâ
```
```
checking examples ... ERROR
Running examples in âsglasso-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: gplot.fglasso
> ### Title: Plotting Sparse Factorial Dynamic Gaussian Graphical Model
> ### Aliases: gplot.fglasso
> ### Keywords: models
> 
> ### ** Examples
> 
> N <- 50
> tp <- 3
> p <- 3
> X <- matrix(rnorm(N * p * tp), N, tp * p)
> S <- crossprod(X) / N
> model <- list(lag0 = c(s = "c", n = "ut"), lag1 = c(s = "t", n = "t"))
> out.fglasso <- fglasso(S = S, model = model, tp = tp, p = p)
> gplot(out.fglasso, rhoid = 50, sub.tp1 = "First graph", 
+    sub.tp2 = "Second graph")
Error in gplot.fglasso(out.fglasso, rhoid = 50, sub.tp1 = "First graph",  : 
  could not find function "plot.igraph"
Calls: gplot -> gplot.fglasso
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## sharpshootR (0.7-2)
Maintainer: Dylan Beaudette <dylan.beaudette@ca.usda.gov>

```
checking whether package âsharpshootRâ can be installed ... ERROR
Installation failed.
See â/Users/gaborcsardi/works/igraph/revdep_check/sharpshootR.Rcheck/00install.outâ for details.
Status: 1 ERROR
```

## shp2graph (0-2)
Maintainer: Binbin Lu <lubinbin220@gmail.com>

```
checking R code for possible problems ... NOTE
footpoint.nodes: no visible global function definition for
  âcoordinatesâ
nt.connect: no visible global function definition for âbboxâ
nt.connect: no visible global function definition for
  âas.SpatialLines.SLDFâ
nt.connect: no visible global function definition for
  âSpatialLinesDataFrameâ
ptsinnt.view: no visible global function definition for âbboxâ
readshpnw: no visible global function definition for âcoordinatesâ
```
```
DONE
Status: 1 NOTE
```

## SID (1.0)
Maintainer: Jonas Peters <jonas.peters@tuebingen.mpg.de>

```
checking package dependencies ... ERROR
Package required but not available: âRBGLâ

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## simcausal (0.2.0)
Maintainer: Oleg Sofrygin <oleg.sofrygin@gmail.com>  
Bug reports: https://github.com/osofr/simcausal/issues

```
checking dependencies in R code ... NOTE
Missing or unexported object: âigraph::plot.igraphâ
```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
...automatically assigning order attribute to some nodes...
node race, order:1
node W1, order:2
node W2, order:3
node W3, order:4
node Anode, order:5
node Y, order:6
using the following vertex attributes: 
120.8NAcircle0
using the following edge attributes: 
0.50.40.8black
Quitting from lines 916-919 (simcausal_vignette.Rnw) 
Error: processing vignette 'simcausal_vignette.Rnw' failed with diagnostics:
'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted

```
```
DONE
Status: 2 NOTEs
```

## SINGLE (1.3)
Maintainer: Ricardo Pio Monti <ricardo.monti08@gmail.com>

```
checking whether package âSINGLEâ can be installed ... WARNING
Found the following significant warnings:
  Warning: replacing previous import by âdse::permuteâ when loading âSINGLEâ
See â/Users/gaborcsardi/works/igraph/revdep_check/SINGLE.Rcheck/00install.outâ for details.
```
```
DONE
Status: 1 WARNING
```

## SOMbrero (1.0)
Maintainer: Nathalie Villa-Vialaneix <nathalie.villa@toulouse.inra.fr>

```
checking examples ... ERROR
Running examples in âSOMbrero-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: projectIGraph
> ### Title: Compute the projection of a graph on a grid
> ### Aliases: projectIGraph.somRes projectIGraph
> ### Keywords: methods
> 
> ### ** Examples
> 
> data(lesmis)
> set.seed(7383)
> mis.som <- trainSOM(x.data=dissim.lesmis, type="relational", nb.save=10)
> proj.lesmis <- projectIGraph(mis.som, lesmis)
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Calls: projectIGraph ... projectGraph -> V -> update_vs_ref -> check_version
Execution halted
```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...

The following object is masked from 'package:base':

    union


***********************************************************

      This is 'SOMbrero' package, v 1.0

Citation details with citation('SOMbrero')

Further information with help(SOMbrero)...

Use sombreroGUI() to start the Graphical Interface.

Warning! This package has been implemented by girls.
Default colors may not be suited for men.

***********************************************************
Quitting from lines 84-87 (doc-relationalSOM.Rmd) 
Error: processing vignette 'doc-relationalSOM.Rmd' failed with diagnostics:
This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## spacejam (1.1)
Maintainer: Arend Voorman <voorma@uw.edu>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Title field: should not end in a period.
```
```
checking dependencies in R code ... NOTE
'library' or 'require' call to âMatrixâ which was already attached by Depends.
  Please remove these calls from your code.
Packages in Depends field not imported from:
  âMatrixâ âigraphâ âsplinesâ
  These packages need to be imported from (in the NAMESPACE file)
  for when this namespace is loaded but not attached.
```
```
checking R code for possible problems ... NOTE
SJ: no visible binding for global variable âbsâ
SJ: no visible global function definition for âget.adjacencyâ
SJ : <anonymous>: no visible global function definition for
  âgraph.adjacencyâ
SJ: no visible binding for global variable âecountâ
SJ.dag: no visible binding for global variable âbsâ
SJ.dag : <anonymous>: no visible global function definition for
  âgraph.adjacencyâ
SJ.dag: no visible binding for global variable âecountâ
SJpath: no visible global function definition for âget.adjacencyâ
SJpath : <anonymous>: no visible global function definition for
  âgraph.adjacencyâ
generate.dag.data: no visible global function definition for âvcountâ
generate.dag.data: no visible global function definition for
  âtopological.sortâ
generate.dag.data: no visible global function definition for
  âneighborsâ
grpsel: no visible global function definition for âMatrixâ
moralize: no visible global function definition for âvcountâ
moralize: no visible global function definition for âas.undirectedâ
moralize: no visible global function definition for âget.adjacencyâ
moralize: no visible global function definition for âadd.edgesâ
moralize: no visible global function definition for âsimplifyâ
plot.SJ: no visible global function definition for
  âlayout.fruchterman.reingoldâ
plot.SJ.dag: no visible global function definition for
  âlayout.fruchterman.reingoldâ
print.SJ: no visible binding for global variable âecountâ
print.SJ: no visible global function definition for âecountâ
print.SJ.dag: no visible binding for global variable âecountâ
print.SJ.dag: no visible global function definition for âecountâ
rdag: no visible global function definition for âgraph.adjacencyâ
```
```
checking Rd line widths ... NOTE
Rd file 'SJ.Rd':
  \examples lines wider than 100 characters:
     #with standard deviations of 1, 0.5 and 0.5, (i.e. giving more weight to linear association than quadratic or cubic)
     #Fit conditional independence graph at one lambda , using the default basis functions (cubic polynomials).
     plot(g, layout=mylayout, edge.color = "gray50", vertex.color = "red", vertex.size = 3, vertex.label = NA, edge.arrow.size = 0.4, main=" ... [TRUNCATED]

Rd file 'generate.dag.data.Rd':
  \usage lines wider than 90 characters:
     generate.dag.data(g, n, basesd = 1, basemean = 0, bfuns = function(x){cbind(x, x^2, x^3)}, 
  \examples lines wider than 100 characters:
     #with standard deviations of 1, 0.5 and 0.5, (i.e. giving more weight to linear association than quadratic or cubic)

Rd file 'spacejam-package.Rd':
  \examples lines wider than 100 characters:
     #with standard deviations of 1, 0.5 and 0.5, (i.e. giving more weight to linear association than quadratic or cubic)
     plot(g, layout=mylayout, edge.color = "gray50", vertex.color = "red", vertex.size = 3, vertex.label = NA, edge.arrow.size = 0.4, main=" ... [TRUNCATED]

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 4 NOTEs
```

## spatgraphs (2.62)
Maintainer: Tuomas Rajala <tuomas.rajala@iki.fi>

```
checking top-level files ... NOTE
Non-standard files/directories found at top level:
  âToAdd.TXT0â âchange.logâ
```
```
checking dependencies in R code ... NOTE
'library' or 'require' call to âMatrixâ in package code.
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  cut.sg plot.sg plot.sgadj plot.sgc print.sg print.sgadj print.sgc
  summary.sg summary.sgc t.sg t.sgadj
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
igraph2sg: no visible global function definition for âget.adjlistâ
plot.sg: no visible global function definition for ârgl.linesâ
plot.sgc: no visible binding for global variable âspheres3dâ
plot.sgc: no visible binding for global variable âpoints3dâ
sg2igraph: no visible global function definition for âgraph.data.frameâ
sg2sparse: no visible global function definition for âsparseMatrixâ
```
```
checking Rd line widths ... NOTE
Rd file 'spatgraphs-package.Rd':
  \examples lines wider than 100 characters:
             pp3d<-list(x=r*sin(tau)*cos(phi),y=r*cos(phi)*cos(tau),z=r*cos(phi),n=n,window=list(x=w,y=w,z=w))

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 5 NOTEs
```

## spdep (0.5-88)
Maintainer: Roger Bivand <Roger.Bivand@nhh.no>

```
checking installed package size ... NOTE
  installed size is  5.3Mb
  sub-directories of 1Mb or more:
    data   1.1Mb
    doc    1.5Mb
    etc    1.7Mb
```
```
DONE
Status: 1 NOTE
```

## SPMS (2.0)
Maintainer: Xiaomeng Ni <ni380910405@yahoo.cn>

```
checking package dependencies ... ERROR
Packages suggested but not available: âRBGLâ âgraphâ âEBImageâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## SSN (1.1.5)
Maintainer: Jay Ver Hoef <ver.hoef@SpatialStreamNetworks.com>

```
checking installed package size ... NOTE
  installed size is  5.1Mb
  sub-directories of 1Mb or more:
    doc       1.1Mb
    lsndata   2.5Mb
```
```
checking examples ... ERROR
Running examples in âSSN-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: SimulateOnSSN
> ### Title: Simulating Data on Spatial Stream Networks
> ### Aliases: SimulateOnSSN
> 
> ### ** Examples
> 
> #######################################
> ## example 1: Gaussian data, 2 networks
> #######################################
> 
> library(SSN)
> set.seed(101)
> ## simulate a SpatialStreamNetwork object
> raw1.ssn <- createSSN(n = c(10,10),
+     obsDesign = binomialDesign(c(50,50)), predDesign = binomialDesign(c(100,100)),
+ 	importToR = TRUE, path = paste(tempdir(),"/sim1", sep = ""))
> plot(raw1.ssn)
> 
> ## create distance matrices, including between predicted and observed
> createDistMat(raw1.ssn, "preds", o.write=TRUE, amongpred = TRUE)
> 
> ## look at the column names of each of the data frames
> names(raw1.ssn)
$Obs
 [1] "locID"      "upDist"     "pid"        "netID"      "rid"       
 [6] "ratio"      "shreve"     "addfunccol" "NEAR_X"     "NEAR_Y"    

$preds
 [1] "locID"      "upDist"     "pid"        "netID"      "rid"       
 [6] "ratio"      "shreve"     "addfunccol" "NEAR_X"     "NEAR_Y"    

> 
> ## extract the observed and predicted data frames
> raw1DFobs <- getSSNdata.frame(raw1.ssn, "Obs")
> raw1DFpred <- getSSNdata.frame(raw1.ssn, "preds")
> 
> ## add a continuous covariate randomly
> raw1DFobs[,"X1"] <- rnorm(length(raw1DFobs[,1]))
> raw1DFpred[,"X1"] <- rnorm(length(raw1DFpred[,1]))
> 
> ## add a categorical covariate randomly
> raw1DFobs[,"F1"] <- as.factor(sample.int(3,length(raw1DFobs[,1]), replace = TRUE))
> raw1DFpred[,"F1"] <- as.factor(sample.int(3,length(raw1DFpred[,1]), replace = TRUE))
> 
> ## simulate Gaussian data
> sim1.out <- SimulateOnSSN(raw1.ssn,
+ 	ObsSimDF = raw1DFobs,
+ 	PredSimDF = raw1DFpred,
+ 	PredID = "preds",
+ 	formula = ~ X1 + F1,
+ 	coefficients = c(1, .5, -1, 1),
+ 	CorModels = c("Exponential.tailup", "Exponential.taildown"),
+ 	use.nugget = TRUE,
+ 	use.anisotropy = FALSE,
+ 	CorParms = c(2, 5, 2, 5, 0.1),
+ 	addfunccol = "addfunccol")
> 
> ## Columns of design matrix, coefficients argument applied to these
> sim1.out$FixedEffects
       Xnames Coefficient
1 (Intercept)         1.0
2          X1         0.5
3         F12        -1.0
4         F13         1.0
> 
> ## extract the ssn.object
> sim1.ssn <- sim1.out$ssn.object
> 
> ## extract the observed and predicted data frames, now with simulated values
> sim1DFobs <- getSSNdata.frame(sim1.ssn, "Obs")
> sim1DFobs[,"Sim_Values"]
  [1] -1.22221603  4.63912013  2.61728318  2.08787430  2.79048827  1.64033148
  [7]  3.49540946  1.99945533  5.72195878  1.20537606  2.99037210  1.67877369
 [13] -0.51200212  1.35291928  3.99476133  0.70740751  1.01256425  5.38907795
 [19]  2.76542504  3.36835225  1.51621684  1.96676706  1.81892768 -0.80520080
 [25]  0.05693503  0.69611890  0.07005844  2.86270046  1.93813656  1.66973468
 [31]  3.95391369  1.16850219  0.36026058 -1.10791594  0.12566414 -1.43834661
 [37]  0.69236606  2.59446507  1.69784809  3.52564693  1.06980961 -0.30536485
 [43] -0.09252584  1.58185562  1.97110922  2.39896065  2.70699895  2.89575511
 [49]  2.82499131  2.98420754 -0.22938636  1.20469100  1.94339172  1.50021304
 [55]  2.30724767  1.63846283  0.65354338 -0.36399753  2.19599708 -0.55693252
 [61] -2.45291734  3.19421460 -2.26737820  0.99835279  0.37491736 -0.88000103
 [67]  1.34138560  3.01037830  0.96254576  0.23918404  3.32474447  2.23326315
 [73]  1.87103880  2.48801876  0.23901987 -1.20189523  1.45746703 -1.45504862
 [79] -2.47756017  0.81722022  0.98496416 -2.40688920  1.09409146 -1.14140862
 [85]  2.80984996 -0.15283142  2.76631989 -1.49042589  2.55362768 -1.07074101
 [91]  0.53528971  2.61915527 -2.89275396  0.09577112  0.46590269  1.39517740
 [97]  1.42268596  0.59728284 -2.95525195  4.57564676
> sim1DFpred <- getSSNdata.frame(sim1.ssn, "preds")
> sim1DFpred[,"Sim_Values"]
  [1]  0.90022179 -0.41282611  4.04054785  3.29128707  3.33055418  2.84417972
  [7] -2.78260315  2.07483716  3.17869484 -0.60004571  2.90952775 -0.64288100
 [13] -0.03491546  4.67513772  4.76810022  3.68529578  1.13991597  1.70658724
 [19]  1.12762684  1.41887483  0.45311675  0.88622539  5.46857129  1.32914323
 [25]  0.64484278  3.34303984  0.15421007  2.18519934  1.36442289  4.87824147
 [31]  1.65248755  2.43422956  0.71373275  1.94060359  1.92271221  3.53886042
 [37]  3.16735849  1.68087713  1.91498299  0.42178747  0.57373418  2.73271917
 [43] -0.32626370  0.77176114  1.01788214  2.41854045  6.32744102  1.37179285
 [49] -0.70787537 -1.40514483  0.63303383 -0.48877376 -0.52145761  3.05408689
 [55] -0.28282582  2.71714904  3.86713443  4.76398834  0.21383758  2.16347844
 [61]  4.25314770  3.84701713  3.50128009  3.77780398  0.43647427  1.31199011
 [67] -1.22953430  2.74217901  0.26494851  2.49376613  0.91615371  2.35073005
 [73]  1.77085946  0.46187341  1.37541422  0.08820810  4.51074452 -0.44896499
 [79]  1.72817983 -1.13197006  3.10548018  4.49461712  2.10152842  4.69690834
 [85]  3.39922575  3.16603618 -1.12129236  3.75663566  1.58317379  4.26059766
 [91]  0.91838379  1.91024851  4.09803929  2.14609306  0.98833217  2.75162381
 [97]  1.81045836  0.87533777  0.63199948  0.18344066 -1.54025210  0.23425787
[103]  0.80153991  0.94887259  0.06943306  2.39996953 -1.41065690  1.00739854
[109] -3.83899461 -0.53752253 -0.28800064 -0.25210009  0.31297603  1.78450093
[115]  5.05302283  2.48839069 -1.30079354 -0.62959345  0.62667206  4.95014964
[121]  1.95043133  0.14525495  3.01857698  0.35436941  0.78416368  0.22548448
[127]  2.04326741  0.06874216 -2.07524148 -0.88005153  2.30160356 -2.36412541
[133]  2.19116972 -0.41121250  5.00110689  1.68382117  1.45023533  0.81779967
[139] -0.84480430 -1.73482270  2.62198854 -2.61896318  3.42261897  4.26309575
[145]  3.26525695  3.17263882  2.65645933  1.71130230  3.44862809  0.20268776
[151]  1.15200580  0.44839442  1.36702546  0.11790512 -0.24375402  1.57702866
[157]  1.77033570 -2.99595711  2.37607936  3.65182474  2.18867494  3.45299200
[163]  0.26978345  4.53104868  1.87604903 -1.65134014  2.07875823  1.88976928
[169]  1.20580964 -1.05023794  0.47757510  3.27415777  3.02438409 -0.16796632
[175]  2.59291582  1.34009753  1.63429809 -1.09995260 -0.25282263  1.93945274
[181]  2.84386817  3.66277324 -0.86760097  0.31237487  2.48537729  0.37393541
[187] -1.54643205  5.08228036 -3.37771315 -0.08407991 -2.35993735  1.37779282
[193]  1.79250206 -0.18933285 -0.37120536  1.14680133 -0.90535391 -0.76086874
[199] -0.37739976  6.00019593
> 
> ## plot the simulated observed values
> plot(sim1.ssn, "Sim_Values")
> 
> ## store simulated prediction values, and then create NAs in their place
> sim1preds <- sim1DFpred[,"Sim_Values"]
> sim1DFpred[,"Sim_Values"] <- NA
> sim1.ssn <- putSSNdata.frame(sim1DFpred, sim1.ssn, "preds")
> 
> # NOT RUN, IT TAKES A MINUTE OR SO
> ## fit a model to see how well we estimate simulation parameters
> #fitSimGau <- glmssn(Sim_Values ~ X1 + F1, ssn.object = sim1.ssn,
> #	 CorModels = c("Exponential.tailup", "Exponential.taildown"),
> #	 addfunccol = "addfunccol")
> # LOAD A STORED VERSION INSTEAD
> data(modelFits)
> #make sure fitSimGau has the correct path, will vary for each users installation
> #predictions depend on distance matrix created earlier with createDistMat function
> #path of this lsn directory was created with createSSN
> fitSimGau$ssn.object@path <- paste(tempdir(),"/sim1", sep = "")
> 
> summary(fitSimGau)

Call:
glmssn(formula = Sim_Values ~ X1 + F1, ssn.object = sim1.ssn, 
    CorModels = c("Exponential.tailup", "Exponential.taildown"), 
    addfunccol = "addfunccol")

Residuals:
    Min      1Q  Median      3Q     Max 
-3.4017 -1.1714  0.4401  1.1060  4.6293 

Coefficients:
            Estimate Std. Error t value Pr(>|t|)    
(Intercept) -0.65419    0.45644  -1.433    0.155    
X1           0.41216    0.06982   5.903   <2e-16 ***
F11          0.00000         NA      NA       NA    
F12         -1.09780    0.14820  -7.408   <2e-16 ***
F13          1.27425    0.14291   8.917   <2e-16 ***
---
Signif. codes:  0 â***â 0.001 â**â 0.01 â*â 0.05 â.â 0.1 â â 1

Covariance Parameters:
     Covariance.Model Parameter Estimate
   Exponential.tailup   parsill  3.22828
   Exponential.tailup     range  4.24424
 Exponential.taildown   parsill  0.00140
 Exponential.taildown     range  9.09635
               Nugget   parsill  0.08062

Residual standard error: 1.81942
Generalized R-squared: 0.7705965
> 
> ## make predictions
> pred1.ssn <- predict(fitSimGau,"preds")
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + 1):(n +  :
  NaNs produced
> par(bg = "grey60")
> plot(pred1.ssn, color.palette = terrain.colors(10))
Error in quantile.default(cexVals, seq(0, 1, by = 0.2)) : 
  missing values and NaN's not allowed if 'na.rm' is FALSE
Calls: plot ... plot.glmssn.predict -> quantile -> quantile.default
Execution halted
```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## stm (1.0.8)
Maintainer: Brandon Stewart <bstewart@fas.harvard.edu>

```
checking dependencies in R code ... NOTE
Missing or unexported objects:
  âigraph::plot.igraphâ âtm::metaâ
```
```
checking examples ... ERROR
Running examples in âstm-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: plot.topicCorr
> ### Title: Plot a topic correlation graph
> ### Aliases: plot.topicCorr
> 
> ### ** Examples
> 
> #This function becomes more useful with larger numbers of topics.
> #it is demonstrated here with a small model simply to show how the syntax works.
> cormat <- topicCorr(gadarianFit)
> plot(cormat)
Error: 'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted
```
```
checking running R code from vignettes ... [25s/47s] ERROR
Errors in running code in vignettes:
when running code in âstmVignette.Rnwâ
  ...
> plot.STM(poliblogPrevFit, type = "summary", xlim = c(0, 
+     0.4))

> mod.out.corr <- topicCorr(poliblogPrevFit)

> plot.topicCorr(mod.out.corr)

  When sourcing âstmVignette.Râ:
Error: 'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted

```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
stm v1.0.8 (2014-11-07) successfully loaded. See ?stm for help.

Error: processing vignette 'stmVignette.Rnw' failed with diagnostics:
 chunk 25 
Error : 'plot.igraph' is not an exported object from 'namespace:igraph'
Execution halted

```
```
DONE
Status: 2 ERRORs, 2 NOTEs
```

## structSSI (1.1.1)
Maintainer: Kris Sankaran <kriss1@stanford.edu>

```
checking package dependencies ... ERROR
Package required but not available: âmulttestâ

Package suggested but not available: âphyloseqâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

## SubpathwayGMir (1.0)
Maintainer: Li Feng <biofengfeng@sina.com>

```
checking running R code from vignettes ... ERROR
Errors in running code in vignettes:
when running code in âSubpathwayGMir.Rnwâ
  ...

> DirectGraphList <- GetK2riData("MetabolicGEGEEMGraph")

> DirectInteGraphList <- getInteGraphList(DirectGraphList, 
+     relations)

  When sourcing âSubpathwayGMir.Râ:
Error: This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
checking re-building of vignette outputs ... NOTE
Error in re-building vignettes:
  ...
Attaching package: âXMLâ

The following object is masked from âpackage:toolsâ:

    toHTML

Loading required package: igraph

Attaching package: âigraphâ

The following objects are masked from âpackage:statsâ:

    decompose, spectrum

The following object is masked from âpackage:baseâ:

    union


Error: processing vignette 'SubpathwayGMir.Rnw' failed with diagnostics:
 chunk 3 
Error in check_version(graph) : 
  This graph was created by an old(er) igraph version.
  Call upgrade_graph() on it to use with the current igraph version
Execution halted

```
```
DONE
Status: 1 ERROR, 1 NOTE
```

## tcR (2.0)
Maintainer: Vadim Nazarov <vdm.nazarov@gmail.com>  
Bug reports: https://github.com/imminfo/tcr/issues

```
checking installed package size ... NOTE
  installed size is  5.5Mb
  sub-directories of 1Mb or more:
    data   1.2Mb
    doc    3.9Mb
```
```
DONE
Status: 1 NOTE
```

## TDA (1.3)
Maintainer: Fabrizio Lecci <lecci@cmu.edu>

```
checking whether package âTDAâ can be installed ... [22s/25s] WARNING
Found the following significant warnings:
  Warning: replacing previous import by âigraph::knnâ when loading âTDAâ
See â/Users/gaborcsardi/works/igraph/revdep_check/TDA.Rcheck/00install.outâ for details.
```
```
DONE
Status: 1 WARNING
```

## timeordered (0.9.8)
Maintainer: Benjamin Blonder <bblonder@gmail.com>

```
checking examples ... ERROR
Running examples in âtimeordered-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: shortesttimepath
> ### Title: Determines a path (shortest by the least time) between a vertex
> ###   at a start time and another vertex at any later time.
> ### Aliases: shortesttimepath
> ### Keywords: ~kwd1 ~kwd2
> 
> ### ** Examples
> 
> data(ants)
> allindivs <- c(union(ants$VertexFrom, ants$VertexTo), "NULL1", "NULL2")
> g <- generatetonetwork(ants, allindivs)
> stp <- shortesttimepath(g, "WBGG", 927, "Q")
Warning in .Call("R_igraph_get_shortest_paths", graph, as.igraph.vs(graph,  :
  At structural_properties.c:4517 :Couldn't reach some vertices
Error in eval(expr, envir, enclos) : object 'X' not found
Calls: shortesttimepath ... tail -> [ -> [.igraph.vs -> lazy_eval -> eval -> eval
Execution halted
```
```
DONE
Status: 1 ERROR
```

## tnet (3.0.11)
Maintainer: Tore Opsahl <tore@opsahl.co.uk>

```
checking DESCRIPTION meta-information ... NOTE
Deprecated license: CC BY-NC 3.0 + file LICENSE
```
```
checking dependencies in R code ... NOTE
'library' or 'require' call to âsurvivalâ which was already attached by Depends.
  Please remove these calls from your code.
```
```
checking Rd line widths ... NOTE
Rd file 'growth_l.Rd':
  \usage lines wider than 90 characters:
      growth_l(net, perspective = "actor", effects, window=NULL, binary=FALSE, nstrata=10, seed=NULL, regression=TRUE) 

Rd file 'weighted_richclub_w.Rd':
  \usage lines wider than 90 characters:
     weighted_richclub_w(net, rich="k", reshuffle="weights", NR=1000, nbins=30, seed=NULL, directed=NULL)

These lines will be truncated in the PDF manual.
```
```
DONE
Status: 3 NOTEs
```

## treemap (2.2)
Maintainer: Martijn Tennekes <mtennekes@gmail.com>

```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'treegraph.Rd':
  â[igraph:layout]{layout}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
checking examples ... ERROR
Running examples in âtreemap-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: treegraph
> ### Title: Create a tree graph
> ### Aliases: treegraph
> 
> ### ** Examples
> 
> data(business)
> treegraph(business, index=c("NACE1", "NACE2", "NACE3", "NACE4"), show.labels=FALSE)
> treegraph(business[business$NACE1=="F - Construction",],
+     index=c("NACE2", "NACE3", "NACE4"), show.labels=TRUE, truncate.labels=c(2,4,6))
> treegraph(business[business$NACE1=="F - Construction",],
+     index=c("NACE2", "NACE3", "NACE4"), show.labels=TRUE, truncate.labels=c(2,4,6),
+     vertex.layout=igraph::layout.fruchterman.reingold)
Error in (function (graph, coords = NULL, dim = 2, niter = 500, start.temp = sqrt(vcount(graph)),  : 
  unused arguments (circular = TRUE, root = 1)
Calls: treegraph -> do.call -> <Anonymous>
Execution halted
```
```
DONE
Status: 1 ERROR, 1 WARNING
```

## TunePareto (2.4)
Maintainer: Hans Kestler <hans.kestler@uni-ulm.de>

```
checking DESCRIPTION meta-information ... NOTE
Malformed Description field: should contain one or more complete sentences.
```
```
checking dependencies in R code ... NOTE
'library' or 'require' calls in package code:
  âgslâ âigraphâ âsnowfallâ
  Please use :: or requireNamespace() instead.
  See section 'Suggested packages' in the 'Writing R Extensions' manual.
```
```
checking S3 generic/method consistency ... NOTE
Found the following apparent S3 methods exported but not registered:
  predict.TuneParetoModel print.TuneParetoClassifier
  print.TuneParetoModel print.TuneParetoResult
See section âRegistering S3 methodsâ in the âWriting R Extensionsâ
manual.
```
```
checking R code for possible problems ... NOTE
plotDominationGraph: no visible global function definition for
  âgraph.adjacencyâ
plotDominationGraph: no visible global function definition for
  âlayout.normâ
sampleCombinations: no visible global function definition for
  âqrng_allocâ
sampleCombinations: no visible global function definition for
  âqrng_getâ
tunePareto: no visible global function definition for âsfLibraryâ
tunePareto : <anonymous>: no visible global function definition for
  âsfLibraryâ
tunePareto: no visible global function definition for âsfExportâ
tunePareto: no visible global function definition for âsfLapplyâ
tunePareto.NaiveBayes: no visible binding for global variable
  âNaiveBayesâ
```
```
checking Rd cross-references ... WARNING
Missing link or links in documentation object 'plotDominationGraph.Rd':
  â[igraph:plot.graph]{plot.igraph}â

See section 'Cross-references' in the 'Writing R Extensions' manual.

```
```
DONE
Status: 1 WARNING, 4 NOTEs
```

## VineCopula (1.5)
Maintainer: Tobias Erhardt <tobias.erhardt@tum.de>

```
checking examples ... ERROR
Running examples in âVineCopula-Ex.Râ failed
The error most likely occurred in:

> base::assign(".ptime", proc.time(), pos = "CheckExEnv")
> ### Name: RVinePIT
> ### Title: Probability Integral Transformation for R-Vine Copula Models
> ### Aliases: RVinePIT
> 
> ### ** Examples
> 
> # load data set
> data(daxreturns)
> 
> # select the R-vine structure, families and parameters
> RVM <- RVineStructureSelect(daxreturns[,1:3], c(1:6))
Warning: 'get.edge' is deperecated, please use 'ends' instead.
Warning: 'get.edge' is deperecated, please use 'ends' instead.
Error in RVineMatrix(M, family = Type, par = Param, par2 = Params2, names = nam) : 
  Error in the structure matrix.
Calls: RVineStructureSelect -> as.RVM -> RVineMatrix
Execution halted
```
```
DONE
Status: 1 ERROR
```

## xergm (1.4.1)
Maintainer: Philip Leifeld <philip.leifeld@uni-konstanz.de>

```
checking package dependencies ... ERROR
Package required but not available: âstatnetâ

Package suggested but not available: âRSienaâ

The suggested packages are required for a complete check.
Checking can be attempted without them by setting the environment
variable _R_CHECK_FORCE_SUGGESTS_ to a false value.

See section âThe DESCRIPTION fileâ in the âWriting R Extensionsâ
manual.
Status: 1 ERROR
```

