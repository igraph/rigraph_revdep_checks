
# More problems, found by CRAN

## Known problems

- [x] FCMapper. Cannot fix, they need to update their package.
      I emailed them already.
- [x] PBC I have no idea what's wrong here, wrote them an email.
- [x] SDDE. No idea what's wrong, cannot fix. Emailed them.
- [x] SSN. Cannot fix, their example relies on fine details. Wrote them an email.
- [x] causaleffect. They have a bug, I emailed them. 
      They import packages that export the same names. I emailed them.
- [x] netassoc. Negative loop for KK, emailed them.
- [x] fanovaGraph Relies on cliques returning numeric vectors, emailed them.
      https://github.com/cran/fanovaGraph/blob/master/tests/testthat/test_fullexample.R#L78
- [x] intergraph Has some saved igraph objects that they need to update, emailed them.
- [x] modMax Need to convert vs to numeric, emailed them.
      https://github.com/cran/modMax/blob/003ebaa010b8d130a5914dc2bc6cb3eab9496930/R/generalFunctions.R#L229
- [x] nat They need to update test cases, emailed them.
      https://github.com/cran/nat/blob/master/tests/testthat/test-neuroml-io.R#L37
	  https://github.com/cran/nat/blob/master/tests/testthat/test-ngraph.R#L63-L65
- [x] outbreaker They have a bug, emailed them.
      https://github.com/cran/outbreaker/blob/a2dee31ebebba37e1a48c3de90570e198f2e9b7c/R/plot.R#L171
- [x] pcalg They have a bug, is.nan should be is.na here:
      https://github.com/cran/pcalg/blob/5ebec0ca94df959929a250513a81e73a14c68c76/R/pcalg.R#L7403
- [x] ppiPre They need to update, emailed them. Need lapply(..., as.vector) here:
	  https://github.com/cran/ppiPre/blob/1154c7cc92a778f9d054ccb43c3b2a7a11b5e8e1/R/TopologicSims.r#L316
- [ ] treemap They have a bug, I emailed them.
      https://github.com/cran/treemap/blob/cfa1f28fd3c6bda6fc3a8f1c8208170833f4f131/R/treegraph.R#L98


## Conflicting imports

- [x] FedData They import packages that export the same names. I emailed them.
- [x] clickstream. They import packages that export the same names. I emailed them.
- [x] gromovlab They import packages that export the same names. I emailed them.
- [x] netweavers They import packages that export the same names. I emailed them.
- [x] arulesViz Emailed about conflicting imports. Fixed Error.
- [x] causaleffect. They import packages that export the same names. I emailed them.

## Summary

- [x] Compilation warnings. Fixed.

- [x] BoolNet. Fixed.
- [x] CePa. Fixed.
- [x] FCMapper. Cannot fix, they need to update their package.
      I emailed them already.
- [x] FedData They import packages that export the same names. I emailed them.
- [x] FisHiCal. Fixed.
- [x] FrF2. Fixed.
- [x] PBC I have no idea what's wrong here, wrote them an email.
- [x] PROFANCY. Fixed.
- [x] QuACN. Fixed.
- [x] RCA. Fixed.
- [x] ReliabilityTheory. Fixed.
- [x] SDDE. No idea what's wrong, cannot fix. Emailed them.
- [x] SINGLE They import packages that export the same names. I emailed them.
- [x] SOMbrero. Fixed.
- [x] SSN. Cannot fix, their example relies on fine details. Wrote them an email.
- [x] SeqGrapheR Does not seem to be my problem.
- [x] SubpathwayGMir
- [x] TDA They import packages that export the same names. I emailed them.
- [x] VineCopula Fixed
- [x] adegenet The crash happens with the current igraph as well, the same way
- [x] arulesViz Emailed about conflicting imports. Fixed Error.
- [x] causaleffect. They have a bug, I emailed them. 
      They import packages that export the same names. I emailed them.
- [x] cccd Fixed
- [x] clickstream. They import packages that export the same names. I emailed them.
- [x] dnet. Fixed
- [x] fanovaGraph
- [x] fuzzyMM They import packages that export the same names. I emailed them.
- [x] gRapfa Fixed
- [x] gemtc Fixed
- [x] gromovlab They import packages that export the same names. I emailed them.
- [x] intergraph Has some saved igraph objects that they need to update, emailed them.
- [x] loe They import packages that export the same names. I emailed them.
- [x] modMax
- [x] nat They need to update test cases, emailed them.
- [x] netassoc. Negative loop for KK, emailed them.
- [x] netgen They import packages that export the same names. I emailed them.
- [x] netweavers They import packages that export the same names. I emailed them.
- [x] optrees Fixed
- [x] outbreaker They have a bug, emailed them.
- [x] pcalg
- [x] popgraph Fixed.
- [x] poplite Fixed
- [x] ppiPre
- [x] qdap Fixed
- [x] restlos They import packages that export the same names. I emailed them.
- [x] secrlinear Fixed
- [x] structSSI The phyloseq issue does not seem to be my problem. The other one fixed.
- [x] timeordered Fixed.
- [x] treemap They have a bug, I emailed them.

> Package: FisHiCal
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98FisHiCal-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: plotInc
>   > ### Title: Plot a spatial inconsistency
>   > ### Aliases: plotInc
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   >   data(spatialInc)
>   >   plotInc(1, spatialInc) # no plot since no spatial incosistency was =
> detected
>   >   plotInc(167, spatialInc) =
> 
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>    *** caught segfault ***
>   address (nil), cause 'unknown'
>   =
> 
>   Traceback:
>    1: base::.Call("R_igraph_mybracket", graph, 10L, PACKAGE =3D "igraph")=
> 
>    2: get_vs_ref(graph)
>    3: update_vs_ref(graph)
>    4: V(g)
>    5: inherits(v, "igraph.vs")
>    6: as.igraph.vs(graph, index)
>    7: get.vertex.attribute(g, "membership", index =3D V(g))
>    8: plotInc(167, spatialInc)
>   aborting ...
>   Segmentation fault
> 
> Package: PBC
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98PBC-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: PBC-class
>   > ### Title: Class "PBC" for the PBC model
>   > ### Aliases: getRoot,PBC-method getGraph,PBC-method getF,PBC-method
>   > ###   getNIteration,PBC-method getDxf,PBC-method getDxdyf,PBC-method
>   > ###   getGraf,PBC-method getGradxf,PBC-method getGradxdyf,PBC-method
>   > ###   getBINMAT,PBC-method getModel,PBC-method setDensity,PBC-method
>   > ###   setGradient,PBC-method pbcPlot,PBC-method pbcPlot getDxdyf getD=
> xf
>   > ###   getF getGradxdyf getGradxf getGraf setGradient setDensity
>   > ###   phi.student1 phi.student phi.norm margin compute gradxf2.studen=
> t
>   > ###   gradxf.norm gradxdyphi2.student gradxdyphi.norm getModel getRoo=
> t
>   > ###   getNIteration getGraph dxf.student dxf.norm dxdyphi.student
>   > ###   dxdyphi.norm getBINMAT draw getBinMat pbc igraph-class PBC-clas=
> s
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## PBC class information
>   > showClass("PBC")
>   Class "PBC" [package "PBC"]
>   =
> 
>   Slots:
>                                                                          =
>  =
> 
>   Name:        root      graph          f        dxf      dxdyf       gra=
> f
>   Class:  character     igraph expression expression expression expressio=
> n
>                                                                          =
>  =
> 
>   Name:      gradxf   gradxdyf     BINMAT      model    density   gradien=
> t
>   Class: expression expression     matrix  character    numeric     vecto=
> r
>                    =
> 
>   Name:  nIteration
>   Class:    numeric
>   > ## Create a PBC object with linking family "Gumbel"
>   > g <- graph.formula(X1-X3,X2-X3,X3-X4,X4-X5,simplify =3D FALSE)
>   > pbcObj <- pbc(g, model=3D"gumbel")
>   Error in matrix(res, ncol =3D 2, byrow =3D TRUE) : =
> 
>     unimplemented type 'expression' in 'copyMatrix'
>   Calls: pbc ... as.igraph.es -> inherits -> na.omit -> E -> ends -> matr=
> ix
>   Execution halted
> 
> Package: PBC
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   Loading required package: igraph
>   =
> 
>   Attaching package: =E2=80=98igraph=E2=80=99
>   =
> 
>   The following objects are masked from =E2=80=98package:stats=E2=80=99:
>   =
> 
>       decompose, spectrum
>   =
> 
>   The following object is masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       union
>   =
> 
>   =
> 
>   Error: processing vignette =E2=80=98PBC.Rnw=E2=80=99 failed with diagno=
> stics:
>    chunk 3 =
> 
>   Error in matrix(res, ncol =3D 2, byrow =3D TRUE) : =
> 
>     unimplemented type =E2=80=98expression=E2=80=99 in =E2=80=98copyMatri=
> x=E2=80=99
>   =
> 
>   Execution halted
> 
> Package: PBC
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98PBC.Rnw=E2=80=99
>     ...
>   =
> 
>   =
> 
>   > g <- graph.formula(X1 - X2, X2 - X3, X3 - X4, X4 - =
> 
>   +     X5, simplify =3D FALSE)
>   =
> 
>   > myPBC <- pbcGumbel(g)
>   =
> 
>     When sourcing =E2=80=98PBC.R=E2=80=99:
>   Error: unimplemented type =E2=80=98expression=E2=80=99 in =E2=80=98copy=
> Matrix=E2=80=99
>   Execution halted
> 
> Package: PBC
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/optim.R=E2=80=99 failed.
>   Last 13 lines of output:
>     > ## Parameters ##
>     > ################
>     > theta <- runif(4)
>     > g <- graph.formula(X1-X4,X4-X2,X2-X3,X4-X5,simplify =3D FALSE)
>     > =
> 
>     > ##########################
>     > ## PBC objects Creation ##
>     > ##########################
>     > myPBCGumbel <- pbcGumbel(g)
>     Error in matrix(res, ncol =3D 2, byrow =3D TRUE) : =
> 
>       unimplemented type 'expression' in 'copyMatrix'
>     Calls: pbcGumbel ... as.igraph.es -> inherits -> na.omit -> E -> ends=
>  -> matrix
>     Execution halted
> 
> Package: PROFANCY
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   Loading required package: Matrix
>   Loading required package: lattice
>   Loading required package: igraph
>   =
> 
>   Attaching package: =E2=80=98igraph=E2=80=99
>   =
> 
>   The following objects are masked from =E2=80=98package:stats=E2=80=99:
>   =
> 
>       decompose, spectrum
>   =
> 
>   The following object is masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       union
>   =
> 
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>   Error: processing vignette =E2=80=98PROFANCY.Rnw=E2=80=99 failed with d=
> iagnostics:
>    chunk 3 =
> 
>   Error in assign("me", graph, envir =3D env) : =
> 
>     use of NULL environment is defunct
>   Execution halted
> 
> Package: PROFANCY
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98PROFANCY.Rnw=E2=80=99
>     ...
>   10: source(output, echo =3D TRUE)
>   11: doTryCatch(return(expr), name, parentenv, handler)
>   12: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   13: tryCatchList(expr, classes, parentenv, handlers)
>   14: tryCatch({    source(output, echo =3D TRUE)}, error =3D function(e)=
>  {    cat("\n  When sourcing ", sQuote(output), ":\n", sep =3D "")    sto=
> p(conditionMessage(e), call. =3D FALSE, domain =3D NA)})
>   15: tools:::.run_one_vignette("PROFANCY.Rnw", "/home/hornik/tmp/CRAN/PR=
> OFANCY.Rcheck/00_pkg_src/PROFANCY/vignettes",     pkgdir =3D "/home/horni=
> k/tmp/CRAN/PROFANCY.Rcheck/00_pkg_src/PROFANCY")
>   aborting ...
>   Segmentation fault
>   =
> 
>   ... incomplete output.  Crash?
> 
> Package: QuACN
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98QuACN-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: minBalabanID
>   > ### Title: Balaban ID number considering shortest paths only
>   > ### Aliases: minBalabanID
>   > ### Keywords: descriptors
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > set.seed(987)
>   > g <- randomEGraph(LETTERS[1:10], 0.3)
>   > =
> 
>   > minBalabanID(g)
>   Error in eval(expr, envir, enclos) : object 'X' not found
>   Calls: minBalabanID ... [[.igraph.vs -> [ -> [.igraph.vs -> lazy_eval -=
> > eval -> eval
>   Execution halted
> 
> Package: QuACN
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   =
> 
>   The following objects are masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       %*%, apply, crossprod, matrix, tcrossprod
>   =
> 
>   C code of R package 'Rmpfr': GMP using 64 bits per limb
>   =
> 
>   =
> 
>   Attaching package: =E2=80=98Rmpfr=E2=80=99
>   =
> 
>   The following objects are masked from =E2=80=98package:stats=E2=80=99:
>   =
> 
>       dbinom, dnorm, dpois, pnorm
>   =
> 
>   The following objects are masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       cbind, pmax, pmin, rbind
>   =
> 
>   Warning in names(fvi) <- nodes(g) :
>     class =E2=80=98mpfr=E2=80=99 has no =E2=80=98names=E2=80=99 slot; ass=
> igning a names attribute will create an invalid object
>   =
> 
>   Error: processing vignette =E2=80=98QuACN.Rnw=E2=80=99 failed with diag=
> nostics:
>    chunk 83 =
> 
>   Error in eval(expr, envir, enclos) : object =E2=80=98X=E2=80=99 not fou=
> nd
>   Execution halted
> 
> Package: QuACN
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98QuACN.Rnw=E2=80=99
>     ...
>   [1] 17.53585
>   =
> 
>   > connectivityID(g, deg =3D vec.degree)
>   [1] 17.53585
>   =
> 
>   > minConnectivityID(g)
>   =
> 
>     When sourcing =E2=80=98QuACN.R=E2=80=99:
>   Error: object =E2=80=98X=E2=80=99 not found
>   Execution halted
> 
> Package: RCA
> Check: whether package can be installed
> Old result: WARNING
>   Found the following significant warnings:
>     glpenv01.c:130:48: warning: incompatible integer to pointer conversio=
> n returning 'int' from a function with result type 'ENV *' (aka 'struct E=
> NV *') [-Wint-conversion]
>     glpenv01.c:138:43: warning: incompatible integer to pointer conversio=
> n returning 'int' from a function with result type 'ENV *' (aka 'struct E=
> NV *') [-Wint-conversion]
>   See =E2=80=98/home/hornik/tmp/R.check/r-devel-clang/Work/PKGS/RCA.Rchec=
> k/00install.out=E2=80=99 for details.
> New result: WARNING
>   Found the following significant warnings:
>     glpenv01.c:130:48: warning: incompatible integer to pointer conversio=
> n returning 'int' from a function with result type 'ENV *' (aka 'struct E=
> NV *') [-Wint-conversion]
>     glpenv01.c:138:43: warning: incompatible integer to pointer conversio=
> n returning 'int' from a function with result type 'ENV *' (aka 'struct E=
> NV *') [-Wint-conversion]
>   See =E2=80=98/home/hornik/tmp/CRAN/RCA.Rcheck/00install.out=E2=80=99 fo=
> r details.
> 
> Package: ReliabilityTheory
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98ReliabilityTheory-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: systemGraphToGenerator
>   > ### Title: Construct a Continuous-time Markov Chain Generator
>   > ### Aliases: systemGraphToGenerator
>   > ### Keywords: generator matrix system signature
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # Get the generator representing a repairable 5 component 'bridge' sy=
> stem with
>   > # failure rate 1 and repair rate 365.
>   > data(sccsO5)
>   > G <- systemGraphToGenerator(sccsO5[[18]]$graph, 1, 365)
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>    *** caught segfault ***
>   address (nil), cause 'unknown'
>   =
> 
>   Traceback:
>    1: base::.Call("R_igraph_mybracket", graph, 10L, PACKAGE =3D "igraph")=
> 
>    2: get_vs_ref(graph)
>    3: update_vs_ref(graph)
>    4: V(g)
>    5: systemGraphToGenerator(sccsO5[[18]]$graph, 1, 365)
>   aborting ...
>   Segmentation fault
> 
> Package: SDDE
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98SDDE-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: complete_network
>   > ### Title: compare two given networks (original and augmented, presen=
> ted as
>   > ###   undirected graphs) using a path analysis
>   > ### Aliases: complete_network
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## Searching the sample data (containing 11 original nodes and 3 augm=
> ented nodes)
>   > data(Sample_1)
>   > result <- complete_network(g1, g2)
>   Error in assign("me", graph, envir =3D env) : invalid 'envir' argument
>   Calls: complete_network -> V -> update_vs_ref -> assign
>   Execution halted
> 
> 
> Package: SOMbrero
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98SOMbrero-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: projectIGraph
>   > ### Title: Compute the projection of a graph on a grid
>   > ### Aliases: projectIGraph.somRes projectIGraph
>   > ### Keywords: methods
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > data(lesmis)
>   > set.seed(7383)
>   > mis.som <- trainSOM(x.data=3Ddissim.lesmis, type=3D"relational", nb.s=
> ave=3D10)
>   > proj.lesmis <- projectIGraph(mis.som, lesmis)
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>    *** caught segfault ***
>   address 0x1400000013, cause 'memory not mapped'
>   =
> 
>   Traceback:
>    1: base::.Call("R_igraph_mybracket", graph, 10L, PACKAGE =3D "igraph")=
> 
>    2: get_vs_ref(graph)
>    3: update_vs_ref(graph)
>    4: V(the.graph)
>    5: projectGraph(init.graph, object$clustering, object$parameters$the.g=
> rid$coord)
>    6: projectIGraph.somRes(mis.som, lesmis)
>    7: projectIGraph(mis.som, lesmis)
>   aborting ...
>   Segmentation fault
> 
> Package: SOMbrero
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>    9: knit_print.default(x, options =3D options)
>   10: fun(x, options =3D options)
>   11: value_fun(ev$value, ev$visible)
>   12: withVisible(value_fun(ev$value, ev$visible))
>   13: withCallingHandlers(withVisible(value_fun(ev$value, ev$visible)),  =
>    warning =3D wHandler, error =3D eHandler, message =3D mHandler)
>   14: handle(pv <- withCallingHandlers(withVisible(value_fun(ev$value,   =
>   ev$visible)), warning =3D wHandler, error =3D eHandler, message =3D mHa=
> ndler))
>   15: evaluate_call(expr, parsed$src[[i]], envir =3D envir, enclos =3D en=
> clos,     debug =3D debug, last =3D i =3D=3D length(out), use_try =3D sto=
> p_on_error !=3D         2L, keep_warning =3D keep_warning, keep_message =3D=
>  keep_message,     output_handler =3D output_handler)
>   16: evaluate::evaluate(code, envir =3D env, new_device =3D FALSE, keep_=
> warning =3D !isFALSE(options$warning),     keep_message =3D !isFALSE(opti=
> ons$message), stop_on_error =3D if (options$error &&         options$incl=
> ude) 0L else 2L, output_handler =3D knit_handlers(options$render,        =
>  options))
>   17: in_dir(opts_knit$get("root.dir") %n% input_dir(), evaluate::evaluat=
> e(code,     envir =3D env, new_device =3D FALSE, keep_warning =3D !isFALS=
> E(options$warning),     keep_message =3D !isFALSE(options$message), stop_=
> on_error =3D if (options$error &&         options$include) 0L else 2L, ou=
> tput_handler =3D knit_handlers(options$render,         options)))
>   18: block_exec(params)
>   19: call_block(x)
>   20: process_group.block(group)
>   21: process_group(group)
>   22: withCallingHandlers(if (tangle) process_tangle(group) else process_=
> group(group),     error =3D function(e) {        setwd(wd)        cat(res=
> , sep =3D "\n", file =3D output %n% "")        message("Quitting from lin=
> es ", paste(current_lines(i),             collapse =3D "-"), " (", knit_c=
> oncord$get("infile"),             ") ")    })
>   23: process_file(text, output)
>   24: knit(input, text =3D text, envir =3D envir, encoding =3D encoding, =
>     quiet =3D quiet)
>   25: (if (grepl("\\.[Rr]md$", file)) knit2html else if (grepl("\\.[Rr]rs=
> t$",     file)) knit2pdf else knit)(file, encoding =3D encoding, quiet =3D=
>  quiet,     envir =3D globalenv())
>   26: engine$weave(file, quiet =3D quiet, encoding =3D enc)
>   27: doTryCatch(return(expr), name, parentenv, handler)
>   28: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   29: tryCatchList(expr, classes, parentenv, handlers)
>   30: tryCatch({    engine$weave(file, quiet =3D quiet, encoding =3D enc)=
>     setwd(startdir)    find_vignette_product(name, by =3D "weave", engine=
>  =3D engine)}, error =3D function(e) {    stop(gettextf("processing vigne=
> tte '%s' failed with diagnostics:\n%s",         file, conditionMessage(e)=
> ), domain =3D NA, call. =3D FALSE)})
>   31: buildVignettes(dir =3D "/home/hornik/tmp/CRAN/SOMbrero.Rcheck/vign_=
> test/SOMbrero")
>   aborting ...
>   Segmentation fault
> 
> Package: SSN
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98SSN-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: SimulateOnSSN
>   > ### Title: Simulating Data on Spatial Stream Networks
>   > ### Aliases: SimulateOnSSN
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > #######################################
>   > ## example 1: Gaussian data, 2 networks
>   > #######################################
>   > =
> 
>   > library(SSN)
>   > set.seed(101)
>   > ## simulate a SpatialStreamNetwork object
>   > raw1.ssn <- createSSN(n =3D c(10,10),
>   +     obsDesign =3D binomialDesign(c(50,50)), predDesign =3D binomialDe=
> sign(c(100,100)),
>   + 	importToR =3D TRUE, path =3D paste(tempdir(),"/sim1", sep =3D ""))
>   > plot(raw1.ssn)
>   > =
> 
>   > ## create distance matrices, including between predicted and observed=
> 
>   > createDistMat(raw1.ssn, "preds", o.write=3DTRUE, amongpred =3D TRUE)
>   > =
> 
>   > ## look at the column names of each of the data frames
>   > names(raw1.ssn)
>   $Obs
>    [1] "locID"      "upDist"     "pid"        "netID"      "rid"       =
> 
>    [6] "ratio"      "shreve"     "addfunccol" "NEAR_X"     "NEAR_Y"    =
> 
>   =
> 
>   $preds
>    [1] "locID"      "upDist"     "pid"        "netID"      "rid"       =
> 
>    [6] "ratio"      "shreve"     "addfunccol" "NEAR_X"     "NEAR_Y"    =
> 
>   =
> 
>   > =
> 
>   > ## extract the observed and predicted data frames
>   > raw1DFobs <- getSSNdata.frame(raw1.ssn, "Obs")
>   > raw1DFpred <- getSSNdata.frame(raw1.ssn, "preds")
>   > =
> 
>   > ## add a continuous covariate randomly
>   > raw1DFobs[,"X1"] <- rnorm(length(raw1DFobs[,1]))
>   > raw1DFpred[,"X1"] <- rnorm(length(raw1DFpred[,1]))
>   > =
> 
>   > ## add a categorical covariate randomly
>   > raw1DFobs[,"F1"] <- as.factor(sample.int(3,length(raw1DFobs[,1]), rep=
> lace =3D TRUE))
>   > raw1DFpred[,"F1"] <- as.factor(sample.int(3,length(raw1DFpred[,1]), r=
> eplace =3D TRUE))
>   > =
> 
>   > ## simulate Gaussian data
>   > sim1.out <- SimulateOnSSN(raw1.ssn,
>   + 	ObsSimDF =3D raw1DFobs,
>   + 	PredSimDF =3D raw1DFpred,
>   + 	PredID =3D "preds",
>   + 	formula =3D ~ X1 + F1,
>   + 	coefficients =3D c(1, .5, -1, 1),
>   + 	CorModels =3D c("Exponential.tailup", "Exponential.taildown"),
>   + 	use.nugget =3D TRUE,
>   + 	use.anisotropy =3D FALSE,
>   + 	CorParms =3D c(2, 5, 2, 5, 0.1),
>   + 	addfunccol =3D "addfunccol")
>   > =
> 
>   > ## Columns of design matrix, coefficients argument applied to these
>   > sim1.out$FixedEffects
>          Xnames Coefficient
>   1 (Intercept)         1.0
>   2          X1         0.5
>   3         F12        -1.0
>   4         F13         1.0
>   > =
> 
>   > ## extract the ssn.object
>   > sim1.ssn <- sim1.out$ssn.object
>   > =
> 
>   > ## extract the observed and predicted data frames, now with simulated=
>  values
>   > sim1DFobs <- getSSNdata.frame(sim1.ssn, "Obs")
>   > sim1DFobs[,"Sim_Values"]
>     [1] -1.22221603  4.63912013  2.61728318  2.08787430  2.79048827  1.64=
> 033148
>     [7]  3.49540946  1.99945533  5.72195878  1.20537606  2.99037210  1.67=
> 877369
>    [13] -0.51200212  1.35291928  3.99476133  0.70740751  1.01256425  5.38=
> 907795
>    [19]  2.76542504  3.36835225  1.51621684  1.96676706  1.81892768 -0.80=
> 520080
>    [25]  0.05693503  0.69611890  0.07005844  2.86270046  1.93813656  1.66=
> 973468
>    [31]  3.95391369  1.16850219  0.36026058 -1.10791594  0.12566414 -1.43=
> 834661
>    [37]  0.69236606  2.59446507  1.69784809  3.52564693  1.06980961 -0.30=
> 536485
>    [43] -0.09252584  1.58185562  1.97110922  2.39896065  2.70699895  2.89=
> 575511
>    [49]  2.82499131  2.98420754 -0.22938636  1.20469100  1.94339172  1.50=
> 021304
>    [55]  2.30724767  1.63846283  0.65354338 -0.36399753  2.19599708 -0.55=
> 693252
>    [61] -2.45291734  3.19421460 -2.26737820  0.99835279  0.37491736 -0.88=
> 000103
>    [67]  1.34138560  3.01037830  0.96254576  0.23918404  3.32474447  2.23=
> 326315
>    [73]  1.87103880  2.48801876  0.23901987 -1.20189523  1.45746703 -1.45=
> 504862
>    [79] -2.47756017  0.81722022  0.98496416 -2.40688920  1.09409146 -1.14=
> 140862
>    [85]  2.80984996 -0.15283142  2.76631989 -1.49042589  2.55362768 -1.07=
> 074101
>    [91]  0.53528971  2.61915527 -2.89275396  0.09577112  0.46590269  1.39=
> 517740
>    [97]  1.42268596  0.59728284 -2.95525195  4.57564676
>   > sim1DFpred <- getSSNdata.frame(sim1.ssn, "preds")
>   > sim1DFpred[,"Sim_Values"]
>     [1]  0.90022179 -0.41282611  4.04054785  3.29128707  3.33055418  2.84=
> 417972
>     [7] -2.78260315  2.07483716  3.17869484 -0.60004571  2.90952775 -0.64=
> 288100
>    [13] -0.03491546  4.67513772  4.76810022  3.68529578  1.13991597  1.70=
> 658724
>    [19]  1.12762684  1.41887483  0.45311675  0.88622539  5.46857129  1.32=
> 914323
>    [25]  0.64484278  3.34303984  0.15421007  2.18519934  1.36442289  4.87=
> 824147
>    [31]  1.65248755  2.43422956  0.71373275  1.94060359  1.92271221  3.53=
> 886042
>    [37]  3.16735849  1.68087713  1.91498299  0.42178747  0.57373418  2.73=
> 271917
>    [43] -0.32626370  0.77176114  1.01788214  2.41854045  6.32744102  1.37=
> 179285
>    [49] -0.70787537 -1.40514483  0.63303383 -0.48877376 -0.52145761  3.05=
> 408689
>    [55] -0.28282582  2.71714904  3.86713443  4.76398834  0.21383758  2.16=
> 347844
>    [61]  4.25314770  3.84701713  3.50128009  3.77780398  0.43647427  1.31=
> 199011
>    [67] -1.22953430  2.74217901  0.26494851  2.49376613  0.91615371  2.35=
> 073005
>    [73]  1.77085946  0.46187341  1.37541422  0.08820810  4.51074452 -0.44=
> 896499
>    [79]  1.72817983 -1.13197006  3.10548018  4.49461712  2.10152842  4.69=
> 690834
>    [85]  3.39922575  3.16603618 -1.12129236  3.75663566  1.58317379  4.26=
> 059766
>    [91]  0.91838379  1.91024851  4.09803929  2.14609306  0.98833217  2.75=
> 162381
>    [97]  1.81045836  0.87533777  0.63199948  0.18344066 -1.54025210  0.23=
> 425787
>   [103]  0.80153991  0.94887259  0.06943306  2.39996953 -1.41065690  1.00=
> 739854
>   [109] -3.83899461 -0.53752253 -0.28800064 -0.25210009  0.31297603  1.78=
> 450093
>   [115]  5.05302283  2.48839069 -1.30079354 -0.62959345  0.62667206  4.95=
> 014964
>   [121]  1.95043133  0.14525495  3.01857698  0.35436941  0.78416368  0.22=
> 548448
>   [127]  2.04326741  0.06874216 -2.07524148 -0.88005153  2.30160356 -2.36=
> 412541
>   [133]  2.19116972 -0.41121250  5.00110689  1.68382117  1.45023533  0.81=
> 779967
>   [139] -0.84480430 -1.73482270  2.62198854 -2.61896318  3.42261897  4.26=
> 309575
>   [145]  3.26525695  3.17263882  2.65645933  1.71130230  3.44862809  0.20=
> 268776
>   [151]  1.15200580  0.44839442  1.36702546  0.11790512 -0.24375402  1.57=
> 702866
>   [157]  1.77033570 -2.99595711  2.37607936  3.65182474  2.18867494  3.45=
> 299200
>   [163]  0.26978345  4.53104868  1.87604903 -1.65134014  2.07875823  1.88=
> 976928
>   [169]  1.20580964 -1.05023794  0.47757510  3.27415777  3.02438409 -0.16=
> 796632
>   [175]  2.59291582  1.34009753  1.63429809 -1.09995260 -0.25282263  1.93=
> 945274
>   [181]  2.84386817  3.66277324 -0.86760097  0.31237487  2.48537729  0.37=
> 393541
>   [187] -1.54643205  5.08228036 -3.37771315 -0.08407991 -2.35993735  1.37=
> 779282
>   [193]  1.79250206 -0.18933285 -0.37120536  1.14680133 -0.90535391 -0.76=
> 086874
>   [199] -0.37739976  6.00019593
>   > =
> 
>   > ## plot the simulated observed values
>   > plot(sim1.ssn, "Sim_Values")
>   > =
> 
>   > ## store simulated prediction values, and then create NAs in their pl=
> ace
>   > sim1preds <- sim1DFpred[,"Sim_Values"]
>   > sim1DFpred[,"Sim_Values"] <- NA
>   > sim1.ssn <- putSSNdata.frame(sim1DFpred, sim1.ssn, "preds")
>   > =
> 
>   > # NOT RUN, IT TAKES A MINUTE OR SO
>   > ## fit a model to see how well we estimate simulation parameters
>   > #fitSimGau <- glmssn(Sim_Values ~ X1 + F1, ssn.object =3D sim1.ssn,
>   > #	 CorModels =3D c("Exponential.tailup", "Exponential.taildown"),
>   > #	 addfunccol =3D "addfunccol")
>   > # LOAD A STORED VERSION INSTEAD
>   > data(modelFits)
>   > #make sure fitSimGau has the correct path, will vary for each users i=
> nstallation
>   > #predictions depend on distance matrix created earlier with createDis=
> tMat function
>   > #path of this lsn directory was created with createSSN
>   > fitSimGau$ssn.object@path <- paste(tempdir(),"/sim1", sep =3D "")
>   > =
> 
>   > summary(fitSimGau)
>   =
> 
>   Call:
>   glmssn(formula =3D Sim_Values ~ X1 + F1, ssn.object =3D sim1.ssn, =
> 
>       CorModels =3D c("Exponential.tailup", "Exponential.taildown"), =
> 
>       addfunccol =3D "addfunccol")
>   =
> 
>   Residuals:
>       Min      1Q  Median      3Q     Max =
> 
>   -3.4017 -1.1714  0.4401  1.1060  4.6293 =
> 
>   =
> 
>   Coefficients:
>               Estimate Std. Error t value Pr(>|t|)    =
> 
>   (Intercept) -0.65419    0.45644  -1.433    0.155    =
> 
>   X1           0.41216    0.06982   5.903   <2e-16 ***
>   F11          0.00000         NA      NA       NA    =
> 
>   F12         -1.09780    0.14820  -7.408   <2e-16 ***
>   F13          1.27425    0.14291   8.917   <2e-16 ***
>   ---
>   Signif. codes:  0 =E2=80=98***=E2=80=99 0.001 =E2=80=98**=E2=80=99 0.01=
>  =E2=80=98*=E2=80=99 0.05 =E2=80=98.=E2=80=99 0.1 =E2=80=98 =E2=80=99 1
>   =
> 
>   Covariance Parameters:
>        Covariance.Model Parameter Estimate
>      Exponential.tailup   parsill  3.22828
>      Exponential.tailup     range  4.24424
>    Exponential.taildown   parsill  0.00140
>    Exponential.taildown     range  9.09635
>                  Nugget   parsill  0.08062
>   =
> 
>   Residual standard error: 1.81942
>   Generalized R-squared: 0.7705965
>   > =
> 
>   > ## make predictions
>   > pred1.ssn <- predict(fitSimGau,"preds")
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   Warning in sqrt(vec[n + p + 1] - tlam %*% vec[1:n] + t(m) %*% vec[(n + =
> 1):(n +  :
>     NaNs produced
>   > par(bg =3D "grey60")
>   > plot(pred1.ssn, color.palette =3D terrain.colors(10))
>   Error in quantile.default(cexVals, seq(0, 1, by =3D 0.2)) : =
> 
>     missing values and NaN's not allowed if 'na.rm' is FALSE
>   Calls: plot ... plot.glmssn.predict -> quantile -> quantile.default
>   Execution halted
> 
> Package: SubpathwayGMir
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>    2: get_vs_ref(graph)
>    3: update_vs_ref(graph)
>    4: V(graphList[[t]])
>    5: getInteGraphList(DirectGraphList, relations)
>    6: eval(expr, envir, enclos)
>    7: eval(expr, .GlobalEnv)
>    8: withVisible(eval(expr, .GlobalEnv))
>    9: doTryCatch(return(expr), name, parentenv, handler)
>   10: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   11: tryCatchList(expr, classes, parentenv, handlers)
>   12: tryCatch(expr, error =3D function(e) {    call <- conditionCall(e) =
>    if (!is.null(call)) {        if (identical(call[[1L]], quote(doTryCatc=
> h)))             call <- sys.call(-4L)        dcall <- deparse(call)[1L] =
>        prefix <- paste("Error in", dcall, ": ")        LONG <- 75L       =
>  msg <- conditionMessage(e)        sm <- strsplit(msg, "\n")[[1L]]       =
>  w <- 14L + nchar(dcall, type =3D "w") + nchar(sm[1L], type =3D "w")     =
>    if (is.na(w))             w <- 14L + nchar(dcall, type =3D "b") + ncha=
> r(sm[1L],                 type =3D "b")        if (w > LONG)             =
> prefix <- paste0(prefix, "\n  ")    }    else prefix <- "Error : "    msg=
>  <- paste0(prefix, conditionMessage(e), "\n")    .Internal(seterrmessage(=
> msg[1L]))    if (!silent && identical(getOption("show.error.messages"),  =
>        TRUE)) {        cat(msg, file =3D stderr())        .Internal(print=
> DeferredWarnings())    }    invisible(structure(msg, class =3D "try-error=
> ", condition =3D e))})
>   13: try(withVisible(eval(expr, .GlobalEnv)), silent =3D TRUE)
>   14: evalFunc(ce, options)
>   15: tryCatchList(expr, classes, parentenv, handlers)
>   16: tryCatch(evalFunc(ce, options), finally =3D {    cat("\n")    sink(=
> )})
>   17: driver$runcode(drobj, chunk, chunkopts)
>   18: utils::Sweave(...)
>   19: engine$weave(file, quiet =3D quiet, encoding =3D enc)
>   20: doTryCatch(return(expr), name, parentenv, handler)
>   21: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   22: tryCatchList(expr, classes, parentenv, handlers)
>   23: tryCatch({    engine$weave(file, quiet =3D quiet, encoding =3D enc)=
>     setwd(startdir)    find_vignette_product(name, by =3D "weave", engine=
>  =3D engine)}, error =3D function(e) {    stop(gettextf("processing vigne=
> tte '%s' failed with diagnostics:\n%s",         file, conditionMessage(e)=
> ), domain =3D NA, call. =3D FALSE)})
>   24: buildVignettes(dir =3D "/home/hornik/tmp/CRAN/SubpathwayGMir.Rcheck=
> /vign_test/SubpathwayGMir")
>   aborting ...
>   Segmentation fault
> 
> Package: SubpathwayGMir
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98SubpathwayGMir.Rnw=E2=80=99
>     ...
>    9: source(output, echo =3D TRUE)
>   10: doTryCatch(return(expr), name, parentenv, handler)
>   11: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   12: tryCatchList(expr, classes, parentenv, handlers)
>   13: tryCatch({    source(output, echo =3D TRUE)}, error =3D function(e)=
>  {    cat("\n  When sourcing ", sQuote(output), ":\n", sep =3D "")    sto=
> p(conditionMessage(e), call. =3D FALSE, domain =3D NA)})
>   14: tools:::.run_one_vignette("SubpathwayGMir.Rnw", "/home/hornik/tmp/C=
> RAN/SubpathwayGMir.Rcheck/00_pkg_src/SubpathwayGMir/vignettes",     pkgdi=
> r =3D "/home/hornik/tmp/CRAN/SubpathwayGMir.Rcheck/00_pkg_src/SubpathwayG=
> Mir")
>   aborting ...
>   Segmentation fault
>   =
> 
>   ... incomplete output.  Crash?
> 
> Package: VineCopula
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98VineCopula-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: RVinePIT
>   > ### Title: Probability Integral Transformation for R-Vine Copula Mode=
> ls
>   > ### Aliases: RVinePIT
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # load data set
>   > data(daxreturns)
>   > =
> 
>   > # select the R-vine structure, families and parameters
>   > RVM <- RVineStructureSelect(daxreturns[,1:3], c(1:6))
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Error in RVineMatrix(M, family =3D Type, par =3D Param, par2 =3D Params=
> 2, names =3D nam) : =
> 
>     Error in the structure matrix.
>   Calls: RVineStructureSelect -> as.RVM -> RVineMatrix
>   Execution halted
> 
> Package: adegenet
> Check: examples
> Old result: ERROR
>   Running examples in =E2=80=98adegenet-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > ### Name: df2genind
>   > ### Title: Convert a data.frame of genotypes to a genind object, and
>   > ###   conversely.
>   > ### Aliases: df2genind genind2df
>   > ### Keywords: manip
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## simple example
>   > df <- data.frame(locusA=3Dc("11","11","12","32"),
>   + locusB=3Dc(NA,"34","55","15"),locusC=3Dc("22","22","21","22"))
>   > row.names(df) <- .genlab("genotype",4)
>   > df
>             locusA locusB locusC
>   genotype1     11   <NA>     22
>   genotype2     11     34     22
>   genotype3     12     55     21
>   genotype4     32     15     22
>   > =
> 
>   > obj <- df2genind(df, ploidy=3D2)
>   Error in while (keepCheck) { : missing value where TRUE/FALSE needed
>   Calls: df2genind -> fillWithZero
>   Execution halted
> New result: ERROR
>   Running examples in =E2=80=98adegenet-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: df2genind
>   > ### Title: Convert a data.frame of genotypes to a genind object, and
>   > ###   conversely.
>   > ### Aliases: df2genind genind2df
>   > ### Keywords: manip
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## simple example
>   > df <- data.frame(locusA=3Dc("11","11","12","32"),
>   + locusB=3Dc(NA,"34","55","15"),locusC=3Dc("22","22","21","22"))
>   > row.names(df) <- .genlab("genotype",4)
>   > df
>             locusA locusB locusC
>   genotype1     11   <NA>     22
>   genotype2     11     34     22
>   genotype3     12     55     21
>   genotype4     32     15     22
>   > =
> 
>   > obj <- df2genind(df, ploidy=3D2)
>   Error in while (keepCheck) { : missing value where TRUE/FALSE needed
>   Calls: df2genind -> fillWithZero
>   Execution halted
> 
> Package: adegenet
> Check: R code for possible problems
> Old result: NOTE
>   HWE.test.genind : ftest: no visible global function definition for
>     =E2=80=98HWE.chisq=E2=80=99
>   HWE.test.genind : ftest: no visible global function definition for
>     =E2=80=98genotype=E2=80=99
>   alignment2genind: no visible binding for global variable =E2=80=98s2c=E2=
> =80=99
>   chooseCN: no visible global function definition for =E2=80=98tri2nb=E2=80=
> =99
>   chooseCN: no visible global function definition for =E2=80=98gabrielnei=
> gh=E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98graph2nb=E2=
> =80=99
>   chooseCN: no visible global function definition for =E2=80=98relativene=
> igh=E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98dnearneigh=
> =E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98knearneigh=
> =E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98knn2nb=E2=80=
> =99
>   chooseCN: no visible global function definition for =E2=80=98nb2listw=E2=
> =80=99
>   chooseCN: no visible global function definition for =E2=80=98mat2listw=E2=
> =80=99
>   fasta2DNAbin: no visible global function definition for =E2=80=98seg.si=
> tes=E2=80=99
>   fasta2genlight: no visible global function definition for =E2=80=98mcla=
> pply=E2=80=99
>   fstat: no visible global function definition for =E2=80=98varcomp.glob=E2=
> =80=99
>   genind2genotype : f2: no visible global function definition for
>     =E2=80=98as.genotype=E2=80=99
>   genind2genotype: no visible global function definition for
>     =E2=80=98makeGenotypes=E2=80=99
>   glPca: no visible global function definition for =E2=80=98mclapply=E2=80=
> =99
>   global.rtest: no visible global function definition for
>     =E2=80=98orthobasis.listw=E2=80=99
>   gstat.randtest: no visible global function definition for
>     =E2=80=98g.stats.glob=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98g.stats.glob=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98samp.within=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98samp.between=E2=80=99
>   local.rtest: no visible global function definition for
>     =E2=80=98orthobasis.listw=E2=80=99
>   plot.spca: no visible global function definition for =E2=80=98card=E2=80=
> =99
>   read.PLINK: no visible global function definition for =E2=80=98mclapply=
> =E2=80=99
>   read.snp: no visible global function definition for =E2=80=98mclapply=E2=
> =80=99
>   snpposi.plot.DNAbin: no visible global function definition for
>     =E2=80=98seg.sites=E2=80=99
>   snpposi.test.DNAbin: no visible global function definition for
>     =E2=80=98seg.sites=E2=80=99
>   spca: no visible global function definition for =E2=80=98mat2listw=E2=80=
> =99
>   spca: no visible global function definition for =E2=80=98nb2listw=E2=80=
> =99
>   summary.spca: no visible global function definition for =E2=80=98listw2=
> mat=E2=80=99
>   summary.spca: no visible binding for global variable =E2=80=98lag.listw=
> =E2=80=99
> New result: NOTE
>   HWE.test.genind : ftest: no visible global function definition for
>     =E2=80=98HWE.chisq=E2=80=99
>   HWE.test.genind : ftest: no visible global function definition for
>     =E2=80=98genotype=E2=80=99
>   alignment2genind: no visible binding for global variable =E2=80=98s2c=E2=
> =80=99
>   as.igraph.haploGen: possible error in layout.fruchterman.reingold(out,
>     params =3D list(miny =3D ypos, maxy =3D ypos)): unused argument (para=
> ms =3D
>     list(miny =3D ypos, maxy =3D ypos))
>   as.igraph.seqTrack: possible error in layout.fruchterman.reingold(out,
>     params =3D list(miny =3D ypos, maxy =3D ypos)): unused argument (para=
> ms =3D
>     list(miny =3D ypos, maxy =3D ypos))
>   chooseCN: no visible global function definition for =E2=80=98tri2nb=E2=80=
> =99
>   chooseCN: no visible global function definition for =E2=80=98gabrielnei=
> gh=E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98graph2nb=E2=
> =80=99
>   chooseCN: no visible global function definition for =E2=80=98relativene=
> igh=E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98dnearneigh=
> =E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98knearneigh=
> =E2=80=99
>   chooseCN: no visible global function definition for =E2=80=98knn2nb=E2=80=
> =99
>   chooseCN: no visible global function definition for =E2=80=98nb2listw=E2=
> =80=99
>   chooseCN: no visible global function definition for =E2=80=98mat2listw=E2=
> =80=99
>   fasta2DNAbin: no visible global function definition for =E2=80=98seg.si=
> tes=E2=80=99
>   fasta2genlight: no visible global function definition for =E2=80=98mcla=
> pply=E2=80=99
>   fstat: no visible global function definition for =E2=80=98varcomp.glob=E2=
> =80=99
>   genind2genotype : f2: no visible global function definition for
>     =E2=80=98as.genotype=E2=80=99
>   genind2genotype: no visible global function definition for
>     =E2=80=98makeGenotypes=E2=80=99
>   glPca: no visible global function definition for =E2=80=98mclapply=E2=80=
> =99
>   global.rtest: no visible global function definition for
>     =E2=80=98orthobasis.listw=E2=80=99
>   gstat.randtest: no visible global function definition for
>     =E2=80=98g.stats.glob=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98g.stats.glob=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98samp.within=E2=80=99
>   gstat.randtest : <anonymous>: no visible global function definition for=
> 
>     =E2=80=98samp.between=E2=80=99
>   local.rtest: no visible global function definition for
>     =E2=80=98orthobasis.listw=E2=80=99
>   plot.spca: no visible global function definition for =E2=80=98card=E2=80=
> =99
>   read.PLINK: no visible global function definition for =E2=80=98mclapply=
> =E2=80=99
>   read.snp: no visible global function definition for =E2=80=98mclapply=E2=
> =80=99
>   snpposi.plot.DNAbin: no visible global function definition for
>     =E2=80=98seg.sites=E2=80=99
>   snpposi.test.DNAbin: no visible global function definition for
>     =E2=80=98seg.sites=E2=80=99
>   spca: no visible global function definition for =E2=80=98mat2listw=E2=80=
> =99
>   spca: no visible global function definition for =E2=80=98nb2listw=E2=80=
> =99
>   summary.spca: no visible global function definition for =E2=80=98listw2=
> mat=E2=80=99
>   summary.spca: no visible binding for global variable =E2=80=98lag.listw=
> =E2=80=99
> 
> Package: arulesViz
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98arulesViz-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: plot
>   > ### Title: Plot method to visualize association rules and itemsets
>   > ### Aliases: plot plot.itemsets plot.rules plot.grouped_matrix
>   > ### Keywords: hplot
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > data(Groceries)
>   > rules <- apriori(Groceries, parameter=3Dlist(support=3D0.005, confide=
> nce=3D0.5))
>   =
> 
>   Parameter specification:
>    confidence minval smax arem  aval originalSupport support minlen maxle=
> n target
>           0.5    0.1    1 none FALSE            TRUE   0.005      1     1=
> 0  rules
>      ext
>    FALSE
>   =
> 
>   Algorithmic control:
>    filter tree heap memopt load sort verbose
>       0.1 TRUE TRUE  FALSE TRUE    2    TRUE
>   =
> 
>   apriori - find association rules with the apriori algorithm
>   version 4.21 (2004.05.09)        (c) 1996-2004   Christian Borgelt
>   set item appearances ...[0 item(s)] done [0.00s].
>   set transactions ...[169 item(s), 9835 transaction(s)] done [0.01s].
>   sorting and recoding items ... [120 item(s)] done [0.00s].
>   creating transaction tree ... done [0.01s].
>   checking subsets of size 1 2 3 4 done [0.01s].
>   writing ... [120 rule(s)] done [0.00s].
>   creating S4 object  ... done [0.00s].
>   > rules
>   set of 120 rules =
> 
>   > =
> 
>   > ## Scatterplot
>   > plot(rules)
>   > ## try: sel <- plot(rules, interactive=3DTRUE)
>   > =
> 
>   > ## Scatterplot with custom colors
>   > library(colorspace) # for sequential_hcl
>   > plot(rules, control=3Dlist(col=3Dsequential_hcl(100)))
>   >     =
> 
>   > ## Two-key plot is a scatterplot with shading =3D "order"
>   > plot(rules, shading=3D"order", control=3Dlist(main =3D "Two-key plot"=
> , =
> 
>   +   col=3Drainbow(5)))
>   > =
> 
>   > ## The following techniques work better with fewer rules
>   > subrules <- subset(rules, lift>2.5)
>   > subrules
>   set of 41 rules =
> 
>   >   =
> 
>   > ## 2D matrix with shading
>   > plot(subrules, method=3D"matrix", measure=3D"lift")
>   Itemsets in Antecedent (LHS)
>    [1] "{root vegetables,onions}"                       =
> 
>    [2] "{onions,whole milk}"                            =
> 
>    [3] "{chicken,root vegetables}"                      =
> 
>    [4] "{root vegetables,frozen vegetables}"            =
> 
>    [5] "{tropical fruit,curd}"                          =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{pork,root vegetables}"                         =
> 
>    [8] "{root vegetables,margarine}"                    =
> 
>    [9] "{butter,whipped/sour cream}"                    =
> 
>   [10] "{tropical fruit,butter}"                        =
> 
>   [11] "{root vegetables,butter}"                       =
> 
>   [12] "{butter,yogurt}"                                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{whipped/sour cream,domestic eggs}"             =
> 
>   [15] "{root vegetables,domestic eggs}"                =
> 
>   [16] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [17] "{pip fruit,whipped/sour cream}"                 =
> 
>   [18] "{citrus fruit,whipped/sour cream}"              =
> 
>   [19] "{tropical fruit,whipped/sour cream}"            =
> 
>   [20] "{root vegetables,whipped/sour cream}"           =
> 
>   [21] "{pip fruit,root vegetables}"                    =
> 
>   [22] "{root vegetables,pastry}"                       =
> 
>   [23] "{citrus fruit,root vegetables}"                 =
> 
>   [24] "{root vegetables,shopping bags}"                =
> 
>   [25] "{tropical fruit,root vegetables}"               =
> 
>   [26] "{root vegetables,yogurt}"                       =
> 
>   [27] "{root vegetables,rolls/buns}"                   =
> 
>   [28] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [29] "{root vegetables,whole milk,whipped/sour cream}"
>   [30] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [31] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [34] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [35] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   [36] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [37] "{tropical fruit,whole milk,yogurt}"             =
> 
>   [38] "{root vegetables,whole milk,yogurt}"            =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > plot(subrules, method=3D"matrix", measure=3D"lift", control=3Dlist(re=
> order=3DTRUE))
>   Itemsets in Antecedent (LHS)
>    [1] "{tropical fruit,curd}"                          =
> 
>    [2] "{root vegetables,yogurt}"                       =
> 
>    [3] "{root vegetables,whipped/sour cream}"           =
> 
>    [4] "{root vegetables,rolls/buns}"                   =
> 
>    [5] "{tropical fruit,whole milk,yogurt}"             =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{whipped/sour cream,domestic eggs}"             =
> 
>    [8] "{root vegetables,domestic eggs}"                =
> 
>    [9] "{root vegetables,butter}"                       =
> 
>   [10] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [11] "{pork,root vegetables}"                         =
> 
>   [12] "{root vegetables,shopping bags}"                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{pip fruit,root vegetables}"                    =
> 
>   [15] "{citrus fruit,whipped/sour cream}"              =
> 
>   [16] "{chicken,root vegetables}"                      =
> 
>   [17] "{root vegetables,frozen vegetables}"            =
> 
>   [18] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [19] "{root vegetables,margarine}"                    =
> 
>   [20] "{root vegetables,pastry}"                       =
> 
>   [21] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [22] "{root vegetables,whole milk,yogurt}"            =
> 
>   [23] "{onions,whole milk}"                            =
> 
>   [24] "{root vegetables,whole milk,whipped/sour cream}"
>   [25] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [26] "{tropical fruit,butter}"                        =
> 
>   [27] "{tropical fruit,whipped/sour cream}"            =
> 
>   [28] "{tropical fruit,root vegetables}"               =
> 
>   [29] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [30] "{citrus fruit,root vegetables}"                 =
> 
>   [31] "{root vegetables,onions}"                       =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [34] "{pip fruit,whipped/sour cream}"                 =
> 
>   [35] "{butter,whipped/sour cream}"                    =
> 
>   [36] "{butter,yogurt}"                                =
> 
>   [37] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [38] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > =
> 
>   > ## 3D matrix
>   > plot(subrules, method=3D"matrix3D", measure=3D"lift")
>   Itemsets in Antecedent (LHS)
>    [1] "{root vegetables,onions}"                       =
> 
>    [2] "{onions,whole milk}"                            =
> 
>    [3] "{chicken,root vegetables}"                      =
> 
>    [4] "{root vegetables,frozen vegetables}"            =
> 
>    [5] "{tropical fruit,curd}"                          =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{pork,root vegetables}"                         =
> 
>    [8] "{root vegetables,margarine}"                    =
> 
>    [9] "{butter,whipped/sour cream}"                    =
> 
>   [10] "{tropical fruit,butter}"                        =
> 
>   [11] "{root vegetables,butter}"                       =
> 
>   [12] "{butter,yogurt}"                                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{whipped/sour cream,domestic eggs}"             =
> 
>   [15] "{root vegetables,domestic eggs}"                =
> 
>   [16] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [17] "{pip fruit,whipped/sour cream}"                 =
> 
>   [18] "{citrus fruit,whipped/sour cream}"              =
> 
>   [19] "{tropical fruit,whipped/sour cream}"            =
> 
>   [20] "{root vegetables,whipped/sour cream}"           =
> 
>   [21] "{pip fruit,root vegetables}"                    =
> 
>   [22] "{root vegetables,pastry}"                       =
> 
>   [23] "{citrus fruit,root vegetables}"                 =
> 
>   [24] "{root vegetables,shopping bags}"                =
> 
>   [25] "{tropical fruit,root vegetables}"               =
> 
>   [26] "{root vegetables,yogurt}"                       =
> 
>   [27] "{root vegetables,rolls/buns}"                   =
> 
>   [28] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [29] "{root vegetables,whole milk,whipped/sour cream}"
>   [30] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [31] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [34] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [35] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   [36] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [37] "{tropical fruit,whole milk,yogurt}"             =
> 
>   [38] "{root vegetables,whole milk,yogurt}"            =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > plot(subrules, method=3D"matrix3D", measure=3D"lift", control=3Dlist(=
> reorder=3DTRUE))
>   Itemsets in Antecedent (LHS)
>    [1] "{tropical fruit,curd}"                          =
> 
>    [2] "{root vegetables,yogurt}"                       =
> 
>    [3] "{root vegetables,whipped/sour cream}"           =
> 
>    [4] "{root vegetables,rolls/buns}"                   =
> 
>    [5] "{tropical fruit,whole milk,yogurt}"             =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{whipped/sour cream,domestic eggs}"             =
> 
>    [8] "{root vegetables,domestic eggs}"                =
> 
>    [9] "{root vegetables,butter}"                       =
> 
>   [10] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [11] "{pork,root vegetables}"                         =
> 
>   [12] "{root vegetables,shopping bags}"                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{pip fruit,root vegetables}"                    =
> 
>   [15] "{citrus fruit,whipped/sour cream}"              =
> 
>   [16] "{chicken,root vegetables}"                      =
> 
>   [17] "{root vegetables,frozen vegetables}"            =
> 
>   [18] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [19] "{root vegetables,margarine}"                    =
> 
>   [20] "{root vegetables,pastry}"                       =
> 
>   [21] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [22] "{root vegetables,whole milk,yogurt}"            =
> 
>   [23] "{onions,whole milk}"                            =
> 
>   [24] "{root vegetables,whole milk,whipped/sour cream}"
>   [25] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [26] "{tropical fruit,butter}"                        =
> 
>   [27] "{tropical fruit,whipped/sour cream}"            =
> 
>   [28] "{tropical fruit,root vegetables}"               =
> 
>   [29] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [30] "{citrus fruit,root vegetables}"                 =
> 
>   [31] "{root vegetables,onions}"                       =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [34] "{pip fruit,whipped/sour cream}"                 =
> 
>   [35] "{butter,whipped/sour cream}"                    =
> 
>   [36] "{butter,yogurt}"                                =
> 
>   [37] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [38] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > =
> 
>   > ## matrix with two measures
>   > plot(subrules, method=3D"matrix", measure=3Dc("lift", "confidence"))
>   Itemsets in Antecedent (LHS)
>    [1] "{root vegetables,onions}"                       =
> 
>    [2] "{onions,whole milk}"                            =
> 
>    [3] "{chicken,root vegetables}"                      =
> 
>    [4] "{root vegetables,frozen vegetables}"            =
> 
>    [5] "{tropical fruit,curd}"                          =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{pork,root vegetables}"                         =
> 
>    [8] "{root vegetables,margarine}"                    =
> 
>    [9] "{butter,whipped/sour cream}"                    =
> 
>   [10] "{tropical fruit,butter}"                        =
> 
>   [11] "{root vegetables,butter}"                       =
> 
>   [12] "{butter,yogurt}"                                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{whipped/sour cream,domestic eggs}"             =
> 
>   [15] "{root vegetables,domestic eggs}"                =
> 
>   [16] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [17] "{pip fruit,whipped/sour cream}"                 =
> 
>   [18] "{citrus fruit,whipped/sour cream}"              =
> 
>   [19] "{tropical fruit,whipped/sour cream}"            =
> 
>   [20] "{root vegetables,whipped/sour cream}"           =
> 
>   [21] "{pip fruit,root vegetables}"                    =
> 
>   [22] "{root vegetables,pastry}"                       =
> 
>   [23] "{citrus fruit,root vegetables}"                 =
> 
>   [24] "{root vegetables,shopping bags}"                =
> 
>   [25] "{tropical fruit,root vegetables}"               =
> 
>   [26] "{root vegetables,yogurt}"                       =
> 
>   [27] "{root vegetables,rolls/buns}"                   =
> 
>   [28] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [29] "{root vegetables,whole milk,whipped/sour cream}"
>   [30] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [31] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [34] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [35] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   [36] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [37] "{tropical fruit,whole milk,yogurt}"             =
> 
>   [38] "{root vegetables,whole milk,yogurt}"            =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > plot(subrules, method=3D"matrix", measure=3Dc("lift", "confidence"), =
> 
>   + 	control=3Dlist(reorder=3DTRUE))
>   Itemsets in Antecedent (LHS)
>    [1] "{tropical fruit,curd}"                          =
> 
>    [2] "{root vegetables,whipped/sour cream}"           =
> 
>    [3] "{root vegetables,yogurt}"                       =
> 
>    [4] "{root vegetables,rolls/buns}"                   =
> 
>    [5] "{tropical fruit,whole milk,yogurt}"             =
> 
>    [6] "{root vegetables,curd}"                         =
> 
>    [7] "{whipped/sour cream,domestic eggs}"             =
> 
>    [8] "{root vegetables,domestic eggs}"                =
> 
>    [9] "{root vegetables,butter}"                       =
> 
>   [10] "{whole milk,yogurt,whipped/sour cream}"         =
> 
>   [11] "{pork,root vegetables}"                         =
> 
>   [12] "{root vegetables,shopping bags}"                =
> 
>   [13] "{root vegetables,newspapers}"                   =
> 
>   [14] "{pip fruit,root vegetables}"                    =
> 
>   [15] "{citrus fruit,whipped/sour cream}"              =
> 
>   [16] "{chicken,root vegetables}"                      =
> 
>   [17] "{root vegetables,frozen vegetables}"            =
> 
>   [18] "{pip fruit,whole milk,yogurt}"                  =
> 
>   [19] "{root vegetables,margarine}"                    =
> 
>   [20] "{root vegetables,pastry}"                       =
> 
>   [21] "{whole milk,yogurt,fruit/vegetable juice}"      =
> 
>   [22] "{root vegetables,whole milk,yogurt}"            =
> 
>   [23] "{onions,whole milk}"                            =
> 
>   [24] "{root vegetables,whole milk,whipped/sour cream}"
>   [25] "{root vegetables,fruit/vegetable juice}"        =
> 
>   [26] "{tropical fruit,butter}"                        =
> 
>   [27] "{tropical fruit,whipped/sour cream}"            =
> 
>   [28] "{tropical fruit,root vegetables}"               =
> 
>   [29] "{tropical fruit,root vegetables,whole milk}"    =
> 
>   [30] "{citrus fruit,root vegetables}"                 =
> 
>   [31] "{root vegetables,onions}"                       =
> 
>   [32] "{pip fruit,root vegetables,whole milk}"         =
> 
>   [33] "{citrus fruit,root vegetables,whole milk}"      =
> 
>   [34] "{pip fruit,whipped/sour cream}"                 =
> 
>   [35] "{butter,whipped/sour cream}"                    =
> 
>   [36] "{butter,yogurt}"                                =
> 
>   [37] "{pip fruit,root vegetables,other vegetables}"   =
> 
>   [38] "{tropical fruit,root vegetables,yogurt}"        =
> 
>   Itemsets in Consequent (RHS)
>   [1] "{other vegetables}" "{yogurt}"           "{whole milk}"      =
> 
>   > =
> 
>   > ## try: plot(subrules, method=3D"matrix", measure=3D"lift", interacti=
> ve=3DTRUE, =
> 
>   > ##		control=3Dlist(reorder=3DTRUE))
>   > =
> 
>   > ## grouped matrix plot
>   > plot(rules, method=3D"grouped")
>   > ## try: sel <- plot(rules, method=3D"grouped", interactive=3DTRUE)
>   > =
> 
>   > ## graphs only work with very few rules
>   > subrules2 <- sample(rules, 10)
>   > plot(subrules2, method=3D"graph")
>   Error in control$layout(g, params =3D control$layoutParams) : =
> 
>     unused argument (params =3D control$layoutParams)
>   Calls: plot ... plot -> plot.igraph -> i.parse.plot.params -> <Anonymou=
> s>
>   Execution halted
> 
> Package: arulesViz
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   Loading required package: arules
>   Loading required package: Matrix
>   =
> 
>   Attaching package: =E2=80=98arules=E2=80=99
>   =
> 
>   The following objects are masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       %in%, write
>   =
> 
>   Loading required package: grid
>   Warning: replacing previous import by =E2=80=98igraph::union=E2=80=99 w=
> hen loading =E2=80=98arulesViz=E2=80=99
>   Warning: replacing previous import by =E2=80=98seriation::permute=E2=80=
> =99 when loading =E2=80=98arulesViz=E2=80=99
>   =
> 
>   Attaching package: =E2=80=98arulesViz=E2=80=99
>   =
> 
>   The following object is masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       abbreviate
>   =
> 
>   =
> 
>   Error: processing vignette =E2=80=98arulesViz.Rnw=E2=80=99 failed with =
> diagnostics:
>    chunk 23 (label =3D graph1) =
> 
>   Error in control$layout(g, params =3D control$layoutParams) : =
> 
>     unused argument (params =3D control$layoutParams)
>   Execution halted
> 
> Package: arulesViz
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98arulesViz.Rnw=E2=80=99
>     ...
>   =
> 
>   > plot(rules, method =3D "grouped", control =3D list(k =3D 50))
>   =
> 
>   > subrules2 <- head(sort(rules, by =3D "lift"), 10)
>   =
> 
>   > plot(subrules2, method =3D "graph", control =3D list(type =3D "items"=
> ))
>   =
> 
>     When sourcing =E2=80=98arulesViz.R=E2=80=99:
>   Error: unused argument (params =3D control$layoutParams)
>   Execution halted
> 
> Package: arulesViz
> Check: whether package can be installed
> New result: WARNING
>   Found the following significant warnings:
>     Warning: replacing previous import by =E2=80=98igraph::union=E2=80=99=
>  when loading =E2=80=98arulesViz=E2=80=99
>     Warning: replacing previous import by =E2=80=98seriation::permute=E2=80=
> =99 when loading =E2=80=98arulesViz=E2=80=99
>   See =E2=80=98/home/hornik/tmp/CRAN/arulesViz.Rcheck/00install.out=E2=80=
> =99 for details.
> 
> 
> Package: causaleffect
> Check: whether package can be installed
> New result: WARNING
>   Found the following significant warnings:
>     Warning: replacing previous import by =E2=80=98igraph::pa=E2=80=99 wh=
> en loading =E2=80=98causaleffect=E2=80=99
>   See =E2=80=98/home/hornik/tmp/CRAN/causaleffect.Rcheck/00install.out=E2=
> =80=99 for details.
> 
> Package: cccd
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98cccd-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: cccd
>   > ### Title: Class Cover Catch Digraph
>   > ### Aliases: cccd cccd.rw cccd.classify cccd.classifier cccd.classifi=
> er.rw
>   > ###   cccd.multiclass.classifier cccd.multiclass.classify plot.cccd
>   > ###   plot.cccdClassifier
>   > ### Keywords: graphs
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > set.seed(456330)
>   > z <- matrix(runif(1000),ncol=3D2)
>   > ind <- which(z[,1]<.5 & z[,2]<.5)
>   > x <- z[ind,]
>   > y <- z[-ind,]
>   > g <- cccd(x,y)
>   > C <- cccd.classifier(x,y)
>   Error in graph(n =3D vc, edges, directed =3D (mode =3D=3D "directed")) =
> : =
> 
>     'edges' must be numeric of character
>   Calls: cccd.classifier ... dominate.greedy -> graph.adjacency -> graph.=
> adjacency.sparse -> graph
>   Execution halted
> 
> Package: dnet
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98dnet-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: dCommSignif
>   > ### Title: Function to test the significance of communities within a =
> graph
>   > ### Aliases: dCommSignif
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # 1) generate an vector consisting of random values from beta distrib=
> ution
>   > x <- rbeta(1000, shape1=3D0.5, shape2=3D1)
>   > =
> 
>   > # 2) fit a p-value distribution under beta-uniform mixture model
>   > fit <- dBUMfit(x, ntry=3D1, hist.bum=3DFALSE, contour.bum=3DFALSE)
>   	A total of p-values: 1000
>   	Maximum Log-Likelihood: 342.1
>   	Mixture parameter (lambda): 0.087
>   	Shape parameter (a): 0.461
>   > =
> 
>   > # 3) calculate the scores according to the fitted BUM and fdr=3D0.01
>   > # using "pdf" method
>   > scores <- dBUMscore(fit, method=3D"pdf", fdr=3D0.05, scatter.bum=3DFA=
> LSE)
>   > names(scores) <- as.character(1:length(scores))
>   > =
> 
>   > # 4) generate a random graph according to the ER model
>   > g <- erdos.renyi.game(1000, 1/100)
>   > =
> 
>   > # 5) produce the induced subgraph only based on the nodes in query
>   > subg <- dNetInduce(g, V(g), knn=3D0)
>   > =
> 
>   > # 6) find the module with the maximum score
>   > module <- dNetFind(subg, scores)
>   Error in eval(expr, envir, enclos) : object 'X' not found
>   Calls: dNetFind ... FUN -> [ -> [.igraph.vs -> lazy_eval -> eval -> eva=
> l
>   Execution halted
> 
> Package: fanovaGraph
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/run-all.R=E2=80=99 failed.
>   Last 13 lines of output:
>     F =3D -9.97537
>     final  value -9.975373 =
> 
>     converged
>          threshold      RMSE
>     [1,]       0.0 0.3281777
>     [2,]       0.4 0.2187619
>     [3,]       1.0 0.9907953
>     testthat results =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D
>     OK: 31 SKIPPED: 0 FAILED: 1
>     1. Failure (at test_fullexample.R#78): the full example works as befo=
> re =
> 
>     =
> 
>     Error: testthat unit tests failed
>     Execution halted
> 
> Package: gRapfa
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98gRapfa-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: KL
>   > ### Title: Kullback-Leibler divergence for APFA models
>   > ### Aliases: KL
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > library(gRapfa)
>   > data(Wheeze)
>   > samp <- sample(1:537, 250)
>   > G <- select.IC(Wheeze[samp,])
>   > G.fit  <- fit.APFA(G, Wheeze[-samp,])
>   Warning in Ops.factor(a$from, 1) : =E2=80=98-=E2=80=99 not meaningful f=
> or factors
>   Warning in Ops.factor(from, 1) : =E2=80=98-=E2=80=99 not meaningful for=
>  factors
>   Warning in Ops.factor(from, 1) : =E2=80=98-=E2=80=99 not meaningful for=
>  factors
>   Warning in Ops.factor(from, 1) : =E2=80=98-=E2=80=99 not meaningful for=
>  factors
>   Error in eattrs[[name]][index] <- value : replacement has length zero
>   Calls: fit.APFA -> E<- -> i_set_edge_attr
>   Execution halted
> 
> Package: gemtc
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98gemtc-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: gemtc-package
>   > ### Title: GeMTC: Network meta-analysis in R
>   > ### Aliases: mtc gemtc gemtc-package
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # Load the example network and generate a consistency model:
>   > file <- system.file("extdata/luades-smoking.gemtc", package=3D"gemtc"=
> )
>   > network <- read.mtc.network(file) =
> 
>   > model <- mtc.model(network, type=3D"consistency")
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Warning: 'get.edge' is deperecated, please use 'ends' instead.
>   Error in eval(expr, envir, enclos) : object 'newX' not found
>   Calls: mtc.model ... FUN -> [ -> [.igraph.vs -> lazy_eval -> eval -> ev=
> al
>   Execution halted
> 
> Package: gemtc
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/test.R=E2=80=99 failed.
>   Last 13 lines of output:
>     9. Error: tree.relative.effect handles a simple tree =
> 
>     1. Error: tree.relative.effect handles a more complex tree =
> 
>     2. Error: tree.relative.effect handles two-treatment case =
> 
>     3. Error: relative.effect can be applied recursively =
> 
>     4. Error: rank.probability returns the right results =
> 
>     5. Error: rank.probability can be applied to a subset of parameters =
> 
>     6. Error: spanning.tree.mtc.result handles two-treatment case =
> 
>     7. Error: relative.effect is robust to missing sd.d =
> 
>     8. Error: relative.effect is robust to leading columns =
> 
>     9. ...
>     =
> 
>     Error: testthat unit tests failed
>     Execution halted
> 
> Package: intergraph
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98intergraph-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: asDF
>   > ### Title: Convert network to data frame(s)
>   > ### Aliases: asDF asDF.igraph asDF.network
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # using method for 'network' objects
>   > d1 <- asDF(exNetwork)
>   > str(d1)
>   List of 2
>    $ edges   :'data.frame':	11 obs. of  4 variables:
>     ..$ V1   : int [1:11] 2 3 4 5 6 8 10 11 14 12 ...
>     ..$ V2   : int [1:11] 1 1 1 1 7 9 11 12 12 13 ...
>     ..$ label: chr [1:11] "ba" "ca" "da" "ea" ...
>     ..$ na   : logi [1:11] FALSE FALSE FALSE FALSE FALSE FALSE ...
>    $ vertexes:'data.frame':	15 obs. of  4 variables:
>     ..$ intergraph_id: int [1:15] 1 2 3 4 5 6 7 8 9 10 ...
>     ..$ label        : chr [1:15] "a" "b" "c" "d" ...
>     ..$ na           : logi [1:15] FALSE FALSE FALSE FALSE FALSE FALSE ..=
> =2E
>     ..$ vertex.names : chr [1:15] "a" "b" "c" "d" ...
>   > =
> 
>   > # using method for 'igraph' objects
>   > d2 <- asDF(exIgraph)
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>    *** caught segfault ***
>   address 0x100000008, cause 'memory not mapped'
>   =
> 
>   Traceback:
>    1: base::.Call("R_igraph_mybracket", graph, 10L, PACKAGE =3D "igraph")=
> 
>    2: get_vs_ref(graph)
>    3: update_es_ref(graph)
>    4: E(graph)
>    5: inherits(e, "igraph.es")
>    6: as.igraph.es(graph, index)
>    7: igraph::get.edge.attribute(x, a)
>    8: FUN(X[[i]], ...)
>    9: lapply(nams, function(a) igraph::get.edge.attribute(x, a))
>   10: dumpAttr.igraph(object, "edge")
>   11: dumpAttr(object, "edge")
>   12: asDF.igraph(exIgraph)
>   13: asDF(exIgraph)
>   aborting ...
>   Segmentation fault
> 
> Package: intergraph
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   15: asNetwork(exIgraph)
>   16: eval(expr, envir, enclos)
>   17: eval(expr, envir, enclos)
>   18: withVisible(eval(expr, envir, enclos))
>   19: withCallingHandlers(withVisible(eval(expr, envir, enclos)), warning=
>  =3D wHandler,     error =3D eHandler, message =3D mHandler)
>   20: handle(ev <- withCallingHandlers(withVisible(eval(expr, envir,     =
> enclos)), warning =3D wHandler, error =3D eHandler, message =3D mHandler)=
> )
>   21: evaluate_call(expr, parsed$src[[i]], envir =3D envir, enclos =3D en=
> clos,     debug =3D debug, last =3D i =3D=3D length(out), use_try =3D sto=
> p_on_error !=3D         2L, keep_warning =3D keep_warning, keep_message =3D=
>  keep_message,     output_handler =3D output_handler)
>   22: evaluate::evaluate(code, envir =3D env, new_device =3D FALSE, keep_=
> warning =3D !isFALSE(options$warning),     keep_message =3D !isFALSE(opti=
> ons$message), stop_on_error =3D if (options$error &&         options$incl=
> ude) 0L else 2L, output_handler =3D knit_handlers(options$render,        =
>  options))
>   23: in_dir(opts_knit$get("root.dir") %n% input_dir(), evaluate::evaluat=
> e(code,     envir =3D env, new_device =3D FALSE, keep_warning =3D !isFALS=
> E(options$warning),     keep_message =3D !isFALSE(options$message), stop_=
> on_error =3D if (options$error &&         options$include) 0L else 2L, ou=
> tput_handler =3D knit_handlers(options$render,         options)))
>   24: block_exec(params)
>   25: call_block(x)
>   26: process_group.block(group)
>   27: process_group(group)
>   28: withCallingHandlers(if (tangle) process_tangle(group) else process_=
> group(group),     error =3D function(e) {        setwd(wd)        cat(res=
> , sep =3D "\n", file =3D output %n% "")        message("Quitting from lin=
> es ", paste(current_lines(i),             collapse =3D "-"), " (", knit_c=
> oncord$get("infile"),             ") ")    })
>   29: process_file(text, output)
>   30: knit(input, text =3D text, envir =3D envir, encoding =3D encoding, =
>     quiet =3D quiet)
>   31: (if (grepl("\\.[Rr]md$", file)) knit2html else if (grepl("\\.[Rr]rs=
> t$",     file)) knit2pdf else knit)(file, encoding =3D encoding, quiet =3D=
>  quiet,     envir =3D globalenv())
>   32: engine$weave(file, quiet =3D quiet, encoding =3D enc)
>   33: doTryCatch(return(expr), name, parentenv, handler)
>   34: tryCatchOne(expr, names, parentenv, handlers[[1L]])
>   35: tryCatchList(expr, classes, parentenv, handlers)
>   36: tryCatch({    engine$weave(file, quiet =3D quiet, encoding =3D enc)=
>     setwd(startdir)    find_vignette_product(name, by =3D "weave", engine=
>  =3D engine)}, error =3D function(e) {    stop(gettextf("processing vigne=
> tte '%s' failed with diagnostics:\n%s",         file, conditionMessage(e)=
> ), domain =3D NA, call. =3D FALSE)})
>   37: buildVignettes(dir =3D "/home/hornik/tmp/CRAN/intergraph.Rcheck/vig=
> n_test/intergraph")
>   aborting ...
>   Segmentation fault
> 
> Package: intergraph
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/testall.R=E2=80=99 failed.
>   Last 13 lines of output:
>     24: test_code(desc, substitute(code), env =3D parent.frame())
>     25: test_that("Vertex names are properly set via 'vnames' argument fo=
> r undirected network",     {        l <- asDF(exIgraph2)        g <- asIg=
> raph(l$edges, vertices =3D l$vertexes, directed =3D FALSE)        expect_=
> identical(g, exIgraph2)    })
>     26: eval(expr, envir, enclos)
>     27: eval(exprs, envir)
>     28: sys.source2(fname, new.env(parent =3D env))
>     29: FUN(X[[i]], ...)
>     30: lapply(paths, test_file, env =3D env, reporter =3D current_report=
> er,     start_end_reporter =3D FALSE)
>     31: test_dir(test_path, reporter =3D reporter, env =3D env, filter =3D=
>  filter,     ...)
>     32: with_top_env(env, {    test_dir(test_path, reporter =3D reporter,=
>  env =3D env, filter =3D filter,         ...)})
>     33: run_tests(package, test_path, filter, reporter, ...)
>     34: test_package("intergraph")
>     aborting ...
>     Segmentation fault
> 
> Package: modMax
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98modMax-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: extremalOptimization
>   > ### Title: Extremal optimization (EO) algorithms
>   > ### Aliases: extremalOptimization pcseoss
>   > ### Keywords: Extremal Optimization Community Modularity Random Local=
> 
>   > ###   Search Agent Social Networks PCSEO-SS algorithm Community struc=
> ture
>   > ###   Conflict pairwise constraints large-scale network
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > =
> 
>   > #weighted network
>   > randomgraph <- erdos.renyi.game(10, 0.3, type=3D"gnp",directed =3D FA=
> LSE, loops =3D FALSE)
>   > =
> 
>   > #to ensure that the graph is connected
>   > vertices <- which(clusters(randomgraph)$membership=3D=3D1)  =
> 
>   > graph <- induced.subgraph(randomgraph,vertices)
>   > graph <- set.edge.attribute(graph, "weight", value=3Drunif(ecount(gra=
> ph),0,1))
>   > =
> 
>   > adj <- get.adjacency(graph, attr=3D"weight")
>   > result <- extremalOptimization(adj)
>   Error in A[i, neighbors[j]] : =
> 
>     invalid or not-yet-implemented 'Matrix' subsetting
>   Calls: extremalOptimization -> callExtremalOptimization -> calculateQ -=
> > [ -> [
>   Execution halted
> 
> Package: modMax
> Check: whether package can be installed
> New result: WARNING
>   Found the following significant warnings:
>     Warning: replacing previous import by =E2=80=98gtools::permute=E2=80=99=
>  when loading =E2=80=98modMax=E2=80=99
>   See =E2=80=98/home/hornik/tmp/CRAN/modMax.Rcheck/00install.out=E2=80=99=
>  for details.
> 
> Package: nat
> Check: Rd cross-references
> New result: WARNING
>   Missing link or links in documentation object 'ngraph.Rd':
>     =E2=80=98[igraph]{attributes}=E2=80=99
>   =
> 
>   See section 'Cross-references' in the 'Writing R Extensions' manual.
> 
> Package: nat
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/test-all.R=E2=80=99 failed.
>   Last 13 lines of output:
>     4: graph(NULL, n =3D 1) at test-seglist.R:50
>     5: stop("'edges' must be numeric of character")
>     =
> 
>     testthat results =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D
>     OK: 627 SKIPPED: 0 FAILED: 5
>     1. Failure (at test-neuroml-io.R#36): parse neuroml files =
> 
>     2. Failure (at test-ngraph.R#63): equivalence of seglist and swc meth=
> ods for as.ngraph.neuron =
> 
>     3. Failure (at test-ngraph.R#64): equivalence of seglist and swc meth=
> ods for as.ngraph.neuron =
> 
>     4. Failure (at test-ngraph.R#65): equivalence of seglist and swc meth=
> ods for as.ngraph.neuron =
> 
>     5. Error: convert graph to seglist =
> 
>     =
> 
>     Error: testthat unit tests failed
>     Execution halted
> 
> Package: nat
> Check: whether package can be installed
> New result: WARNING
>   Found the following significant warnings:
>     Warning: replacing previous import by =E2=80=98nabor::knn=E2=80=99 wh=
> en loading =E2=80=98nat=E2=80=99
>   See =E2=80=98/home/hornik/tmp/CRAN/nat.Rcheck/00install.out=E2=80=99 fo=
> r details.
> 
> Package: netassoc
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98netassoc-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: makenetwork
>   > ### Title: Infer species-association network
>   > ### Aliases: makenetwork
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # generate random data
>   > set.seed(1)
>   > nsp <- 10
>   > nsi <- 5
>   > m_obs <- floor(matrix(rgamma(nsp*nsi,shape=3D5),ncol=3Dnsi,nrow=3Dnsp=
> ))
>   > m_nul <- floor(matrix(rexp(nsp*nsi,rate=3D0.05),ncol=3Dnsi,nrow=3Dnsp=
> ))
>   > =
> 
>   > n <- makenetwork(m_obs, m_nul, numnulls=3D50, plot=3DTRUE)
>   Generating null replicates.............................................=
> =2E..........done.
>   Calculating co-occurrence scores...1 2 0.022 obs. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   1 3 0.044 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 4 0.067 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 5 0.089 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 6 0.111 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   1 7 0.133 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 8 0.156 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 9 0.178 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   1 10 0.200 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   2 3 0.222 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 4 0.244 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 5 0.267 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 6 0.289 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   2 7 0.311 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 8 0.333 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 9 0.356 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   2 10 0.378 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   3 4 0.400 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   3 5 0.422 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   3 6 0.444 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   3 7 0.467 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   3 8 0.489 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   3 9 0.511 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   3 10 0.533 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   4 5 0.556 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   4 6 0.578 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   4 7 0.600 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   4 8 0.622 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   4 9 0.644 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   4 10 0.667 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   5 6 0.689 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   5 7 0.711 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   5 8 0.733 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   5 9 0.756 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   5 10 0.778 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   6 7 0.800 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   6 8 0.822 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   6 9 0.844 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, me=
> thod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   6 10 0.867 obs. .. .. .Warning in cor(x =3D veci_nul, y =3D vecj_nul, m=
> ethod =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .Warning in cor(x =3D veci_nul, y =3D v=
> ecj_nul, method =3D whichmethod) :
>     the standard deviation is zero
>   . .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. .. .. .. .. .. =
> 
>   7 8 0.889 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   7 9 0.911 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   7 10 0.933 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   8 9 0.956 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. ..=
>  .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. =
> 
>   8 10 0.978 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   9 10 1.000 obs. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .=
> =2E .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. .. =
> =2E. .. .. .. .. .. .. .. =
> 
>   ...done.
>   Calculating standardized effect sizes......done.
>   Applying kappa threshold......done.
>   Building network......done.
>   Error in .Call("R_igraph_layout_kamada_kawai", graph, coords, maxiter, =
>  : =
> 
>     At structural_properties.c:5235 : cannot run Bellman-Ford algorithm, =
> Negative loop detected while calculating shortest paths
>   Calls: makenetwork ... layout.auto -> layout_with_kk -> .Call -> <Anony=
> mous>
>   Execution halted
> 
> Package: netgsa
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98netgsa-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: NetGSA
>   > ### Title: Network-based Gene Set Analysis
>   > ### Aliases: NetGSA
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > set.seed(1)
>   > library(igraph)
>   > data(netgsaex)
>   > =
> 
>   > A1 =3D netgsaex$A1
>   > A2 =3D netgsaex$A2
>   > B =3D netgsaex$B
>   > x =3D netgsaex$x
>   > y =3D netgsaex$y
>   > =
> 
>   > ##Visualize the networks
>   > par(mar =3D c(0.5, 0.5, 3, 0.5))
>   > plot(netgsaex$g.alt, vertex.size =3D 5, vertex.label =3D NA, main=3D"=
> Network - alt")
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   Error in assign("me", graph, envir =3D env) : invalid 'envir' argument
>   Calls: plot ... as.igraph.es -> inherits -> E -> update_es_ref -> assig=
> n
>   Execution halted
> 
> Package: optrees
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98optrees-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: getShortestPathTree
>   > ### Title: Computes a shortest path tree
>   > ### Aliases: getShortestPathTree
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > # Graph
>   > nodes <- 1:5
>   > arcs <- matrix(c(1,2,2, 1,3,2, 1,4,3, 2,5,5, 3,2,4, 3,5,3, 4,3,1, 4,5=
> ,0),
>   +                ncol =3D 3, byrow =3D TRUE)
>   > # Shortest path tree
>   > getShortestPathTree(nodes, arcs, algorithm =3D "Dijkstra", directed=3D=
> FALSE)
>   =
> 
>    Shortest path tree =
> 
>    Algorithm: Dijkstra =
> 
>    Stages:  4 | Time:  0.001 =
> 
>    ------------------------------
>         ept1     ept2    weight =
> 
>            1        2         2
>            1        3         2
>            1        4         3
>            4        5         0
>    ------------------------------
>                      Total =3D 7 =
> 
>   =
> 
>    Distances from source: =
> 
>    ------------------------------
>       source     node  distance =
> 
>            1        2         2
>            1        3         2
>            1        4         3
>            1        5         3
>    ------------------------------
>   =
> 
>   Error in if (vr[1] =3D=3D vr[2]) { : missing value where TRUE/FALSE nee=
> ded
>   Calls: getShortestPathTree ... repGraph -> plot.igraph -> norm_coords -=
> > .layout.norm.col
>   Execution halted
> 
> Package: outbreaker
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98outbreaker-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: simulated outbreak dataset
>   > ### Title: Toy outbreak dataset used to illustrate outbreaker
>   > ### Aliases: fakeOutbreak
>   > ### Keywords: datasets
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## Not run: =
> 
>   > ##D ## COMMAND LINES TO GENERATE SIMILAR DATA ##
>   > ##D w <- c(0, 0.5, 1, 0.75)
>   > ##D ## note: this works only if outbreak has at least 30 case
>   > ##D dat <- simOutbreak(R0 =3D 2, infec.curve =3D w, n.hosts =3D 100)[=
> 1:30]
>   > ##D collecDates <- dat$onset + sample(0:3, size=3D30, replace=3DTRUE,=
>  prob=3Dw)
>   > ## End(Not run)
>   > =
> 
>   > ## EXAMPLE USING TOYOUTBREAK ##
>   > ## LOAD DATA, SET RANDOM SEED
>   > data(fakeOutbreak)
>   > attach(fakeOutbreak)
>   > =
> 
>   > ## VISUALIZE DYNAMICS
>   > matplot(dat$dynam, type=3D"o", pch=3D20, lty=3D1,
>   +    main=3D"Outbreak dynamics", xlim=3Dc(0,28))
>   > legend("topright", legend=3Dc("S","I","R"), lty=3D1, col=3D1:3)
>   > =
> 
>   > ## VISUALIZE TRANSMISSION TREE
>   > plot(dat, annot=3D"dist", main=3D"Data - transmission tree")
>   Error in layout.fruchterman.reingold(out, params =3D list(minx =3D V(ou=
> t)$date,  : =
> 
>     unused argument (params =3D list(minx =3D V(out)$date, maxx =3D V(out=
> )$date))
>   Calls: plot ... as.igraph.simOutbreak -> layout.fruchterman.reingold
>   Execution halted
> 
> Package: outbreaker
> Check: R code for possible problems
> New result: NOTE
>   as.igraph.simOutbreak: possible error in
>     layout.fruchterman.reingold(out, params =3D list(minx =3D V(out)$date=
> ,
>     maxx =3D V(out)$date)): unused argument (params =3D list(minx =3D
>     V(out)$date, maxx =3D V(out)$date))
>   as.igraph.tTree: possible error in layout.fruchterman.reingold(out,
>     params =3D list(minx =3D x$inf.dates, maxx =3D x$inf.dates)): unused
>     argument (params =3D list(minx =3D x$inf.dates, maxx =3D x$inf.dates)=
> )
>   transGraph: possible error in layout.fruchterman.reingold(out, params =3D=
> 
>     list(minx =3D V(out)$onset, maxx =3D V(out)$onset), rescale =3D FALSE=
> ):
>     unused arguments (params =3D list(minx =3D V(out)$onset, maxx =3D
>     V(out)$onset), rescale =3D FALSE)
> 
> Package: pcalg
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98pcalg-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: jointIda
>   > ### Title: Estimate Multiset of Possible Total Joint Effects
>   > ### Aliases: jointIda
>   > ### Keywords: multivariate models graphs
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > ## Create a weighted DAG
>   > p <- 6
>   > V<-as.character(1:p)
>   > edL <- vector("list",length=3D6)
>   > names(edL)<-V
>   > edL[[1]] <- list(edges=3Dc(3,4),weights=3Dc(1.1,0.3))
>   > edL[[2]] <- list(edges=3Dc(6),weights=3Dc(0.4))
>   > edL[[3]] <- list(edges=3Dc(2,4,6),weights=3Dc(0.6,0.8,0.9))
>   > edL[[4]] <- list(edges=3Dc(2),weights=3Dc(0.5))
>   > edL[[5]] <- list(edges=3Dc(1,4),weights=3Dc(0.2,0.7))
>   > myDAG <- new("graphNEL",nodes=3DV,edgeL=3DedL,edgemode=3D"directed") =
> ## true DAG
>   > myCPDAG <- dag2cpdag(myDAG) ## true CPDAG
>   > covTrue <- trueCov(myDAG) ## true covariance matrix
>   > =
> 
>   > ## simulate Gaussian data from the true DAG
>   > set.seed(123)
>   > if (require(mvtnorm)) {
>   +   n <- 1000
>   +   dat <- rmvnorm(n,mean=3Drep(0,p),sigma=3DcovTrue)
>   + }
>   Loading required package: mvtnorm
>   > =
> 
>   > ## estimate CPDAG -- see  help(pc)
>   > suffStat <- list(C =3D cor(dat), n =3D n)
>   > pc.fit <- pc(suffStat, indepTest =3D gaussCItest, p =3D p, alpha =3D =
> 0.01 ,u2pd=3D"relaxed")
>   > =
> 
>   > if (require(Rgraphviz)) {
>   +   ## plot the true and estimated graphs
>   +   par(mfrow =3D c(1,2))
>   +   plot(myDAG, main =3D "True DAG")
>   +   plot(pc.fit, main =3D "Estimated CPDAG")
>   + }
>   Loading required package: Rgraphviz
>   Loading required package: graph
>   Loading required package: grid
>   > =
> 
>   > ## Suppose that we know the true CPDAG and covariance matrix
>   > jointIda(x.pos=3Dc(1,2),y.pos=3D6,covTrue,graphEst=3DmyCPDAG,techniqu=
> e=3D"RRC")
>   Error in simple_vs_index(x, ii, na_ok) : Unknown vertex selected
>   Calls: jointIda ... extract.parent.sets -> [ -> [.igraph.vs -> simple_v=
> s_index
>   Execution halted
> 
> Package: pcalg
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/test_jointIda.R=E2=80=99 failed.
>   Last 13 lines of output:
>     Loading required package: mvtnorm
>     > =
> 
>     > ## estimate CPDAG -- see  help(pc)
>     > suffStat <- list(C =3D cor(dat), n =3D n)
>     > pc.fit <- pc(suffStat, indepTest =3D gaussCItest, p =3D p, alpha =3D=
>  0.01 ,u2pd=3D"relaxed")
>     > =
> 
>     > Rnd <- 7
>     > ## Suppose that we know the true CPDAG and covariance matrix
>     > mTrue <- matrix(c(0.99, 0.4, 0.99, 0.4, 0, 0.4), 2,3)
>     > m1 <- round(jointIda(x.pos=3Dc(1,2),y.pos=3D6,covTrue,graphEst=3Dmy=
> CPDAG,technique=3D"RRC"), Rnd)
>     Error in simple_vs_index(x, ii, na_ok) : Unknown vertex selected
>     Calls: jointIda ... extract.parent.sets -> [ -> [.igraph.vs -> simple=
> _vs_index
>     Execution halted
> 
> Package: popgraph
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98popgraph-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: theme_empty
>   > ### Title: A blank theme for plotting networks
>   > ### Aliases: theme_empty
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > data(lopho)
>   > require(ggplot2)
>   > require(igraph)
>   > layout <- layout.fruchterman.reingold( lopho )
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   Error in assign("me", graph, envir =3D env) : invalid 'envir' argument
>   Calls: layout.fruchterman.reingold -> E -> update_es_ref -> assign
>   Execution halted
> 
> Package: poplite
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98poplite-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: External methods
>   > ### Title: Specific methods for generics defined in external packages=
> =2E
>   > ### Aliases: filter select
>   > ### Keywords: utilities
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   >   if (require(Lahman))
>   +   {
>   +       baseball.teams <- makeSchemaFromData(TeamsFranchises, name=3D"t=
> eam_franch")
>   +       baseball.teams <- append(baseball.teams, makeSchemaFromData(Tea=
> ms, name=3D"teams"))
>   +       =
> 
>   +       relationship(baseball.teams, from=3D"team_franch", to=3D"teams"=
> ) <- franchID ~ franchID
>   +       =
> 
>   +       baseball.db <- Database(baseball.teams, tempfile())
>   +       =
> 
>   +       populate(baseball.db, teams=3DTeams, team_franch=3DTeamsFranchi=
> ses)
>   +       =
> 
>   +       select(baseball.db, .tables=3D"teams")
>   +       =
> 
>   +       select(baseball.db, .tables=3Dc("teams", "team_franch"))
>   +       =
> 
>   +       select(baseball.db, yearID:WCWin, franchName)
>   +       =
> 
>   +       filter(baseball.db, active =3D=3D "Y")
>   +       =
> 
>   +       select(filter(baseball.db, active =3D=3D "Y" & W > 50 & teamID =
> =3D=3D "CAL"), active, W, teamID)
>   +   }
>   Loading required package: Lahman
>   Starting team_franch
>   Starting teams
>   Error in eval(expr, envir, enclos) : object 'X' not found
>   Calls: select ... FUN -> [ -> [.igraph.vs -> lazy_eval -> eval -> eval
>   Execution halted
> 
> Package: poplite
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   The following objects are masked from =E2=80=98package:base=E2=80=99:
>   =
> 
>       intersect, setdiff, setequal, union
>   =
> 
>   =
> 
>   Attaching package: =E2=80=98poplite=E2=80=99
>   =
> 
>   The following object is masked from =E2=80=98package:dplyr=E2=80=99:
>   =
> 
>       select
>   =
> 
>   The following object is masked from =E2=80=98package:stats=E2=80=99:
>   =
> 
>       filter
>   =
> 
>   Error in makeSchemaFromData(dna, "dna") : =
> 
>     ERROR: The names of the supplied data.frame need to be modified for t=
> he database see correct.df.names
>   Starting clinical
>   Starting samples
>   Starting dna
>   =
> 
>   Error: processing vignette =E2=80=98poplite.Rnw=E2=80=99 failed with di=
> agnostics:
>    chunk 9 =
> 
>   Error in eval(expr, envir, enclos) : object =E2=80=98X=E2=80=99 not fou=
> nd
>   Execution halted
> 
> Package: poplite
> Check: running R code from vignettes
> New result: ERROR
>   Errors in running code in vignettes:
>   when running code in =E2=80=98poplite.Rnw=E2=80=99
>     ...
>   9         10    1 dna_10_1
>   10        15    1 dna_15_1
>   ..       ...  ...      ...
>   =
> 
>   > select(sample.tracking.db, .tables =3D c("clinical", =
> 
>   +     "dna"))
>   =
> 
>     When sourcing =E2=80=98poplite.R=E2=80=99:
>   Error: object =E2=80=98X=E2=80=99 not found
>   Execution halted
> 
> Package: poplite
> Check: tests
> New result: ERROR
>   Running the tests in =E2=80=98tests/testthat.R=E2=80=99 failed.
>   Last 13 lines of output:
>     16: lazy_eval(args[[idx]], data =3D c(attrs, nei =3D nei, innei =3D i=
> nnei, outnei =3D outnei, =
> 
>            adj =3D adj, inc =3D inc, from =3D from, to =3D to))
>     17: eval(x$expr, data, x$env)
>     18: eval(expr, envir, enclos)
>     =
> 
>     testthat results =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=
> =3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D=3D
>     OK: 129 SKIPPED: 0 FAILED: 3
>     1. Error: Querying with Database objects =
> 
>     2. Error: sample tracking example but with direct keys between dna an=
> d samples =
> 
>     3. Error: oligoMask queries that break poplite =
> 
>     =
> 
>     Error: testthat unit tests failed
>     Execution halted
> 
> Package: ppiPre
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98ppiPre-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: AASim
>   > ### Title: Compute Adamic-Adar Index Between Two Nodes in PPI Network=
> 
>   > ### Aliases: AASim
>   > ### Keywords: manip
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   >   edges <- data.frame(node1=3Dc("1132", "1133", "1134", "1134", "1145=
> ", "1147", "1147", "1147"),
>   +                       node2=3Dc("1134", "1134", "1145", "1147", "1147=
> ", "1148", "1149", "1150"))
>   >   graph<-igraph::graph.data.frame(edges,directed=3DFALSE)
>   >   AASim("1134","1147",graph)
>   Error in `[<-.igraph.vs`(`*tmp*`, 1, value =3D 9) : invalid indexing
>   Calls: AASim -> [<- -> [<-.igraph.vs
>   Execution halted
> 
> Package: qdap
> Check: Rd cross-references
> New result: WARNING
>   Missing link or links in documentation object 'plot.cm_distance.Rd':
>     =E2=80=98[igraph]{layout}=E2=80=99
>   =
> 
>   Missing link or links in documentation object 'word_associate.Rd':
>     =E2=80=98[igraph]{layout}=E2=80=99
>   =
> 
>   Missing link or links in documentation object 'word_network_plot.Rd':
>     =E2=80=98[igraph]{igraph.vertex.shapes}=E2=80=99 =E2=80=98[igraph]{la=
> yout}=E2=80=99
>   =
> 
>   See section 'Cross-references' in the 'Writing R Extensions' manual.
> 
> Package: secrlinear
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98secrlinear-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: Arvicola
>   > ### Title: Water Vole Capture Dataset
>   > ### Aliases: arvicola
>   > ### Keywords: datasets
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > =
> 
>   > summary(arvicola)
>   Object class      capthist =
> 
>   Detector type     multi =
> 
>   Detector number   88 =
> 
>   Average spacing   19.80165 m =
> 
>   x-range           163.85 835.61 m =
> 
>   y-range           457.67 684.59 m =
> 
>   Counts by occasion =
> 
>                      1  2  3  4  5  6 Total
>   n                 16 11 18 12 16 11    84
>   u                 16  2  6  1  1  0    26
>   f                  7  3  4  5  3  4    26
>   M(t+1)            16 18 24 25 26 26    26
>   losses             0  0  0  0  0  0     0
>   detections        16 11 18 12 16 11    84
>   detectors visited 16 11 18 12 16 11    84
>   detectors used    88 88 88 88 88 88   528
>   =
> 
>   > head(traps(arvicola))
>             x      y
>   0.A  164.86 609.69
>   0.B  164.86 609.69
>   20.A 163.85 629.66
>   20.B 163.85 629.66
>   40.A 164.88 649.19
>   40.B 164.88 649.19
>   > =
> 
>   > ## for speed, pre-compute distance matrix
>   > userd <- networkdistance (traps(arvicola), glymemask, glymemask)
>   Warning in warn_version(graph) :
>     This graph was created by an old(er) igraph version.
>     Call upgrade_graph() on it to use with the current igraph version
>     For now we convert it on the fly...
>   =
> 
>    *** caught segfault ***
>   address 0x9400000093, cause 'memory not mapped'
>   =
> 
>   Traceback:
>    1: base::.Call("R_igraph_mybracket", graph, 10L, PACKAGE =3D "igraph")=
> 
>    2: get_vs_ref(graph)
>    3: update_vs_ref(graph)
>    4: V(gr)
>    5: cbind(V(gr)$x, V(gr)$y)
>    6: networkdistance(traps(arvicola), glymemask, glymemask)
>   aborting ...
>   Segmentation fault
> 
> Package: secrlinear
> Check: re-building of vignette outputs
> New result: NOTE
>   Error in re-building vignettes:
>     ...
>   Warning in in_dir(opts_knit$get("root.dir") %n% input_dir(), evaluate::=
> evaluate(code,  :
>     You changed the working directory to /home/hornik/tmp/CRAN/secrlinear=
> =2ERcheck/secrlinear/extdata (probably via setwd()). It will be restored =
> to /home/hornik/tmp/CRAN/secrlinear.Rcheck/vign_test/secrlinear/vignettes=
> =2E See the Note section in ?knitr::knit
>   Quitting from lines 72-74 (secrlinear-vignette.Rmd) =
> 
>   Error: processing vignette =E2=80=98secrlinear-vignette.Rmd=E2=80=99 fa=
> iled with diagnostics:
>   non-numeric argument to binary operator
>   Execution halted
> 
> Package: timeordered
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98timeordered-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: shortesttimepath
>   > ### Title: Determines a path (shortest by the least time) between a v=
> ertex
>   > ###   at a start time and another vertex at any later time.
>   > ### Aliases: shortesttimepath
>   > ### Keywords: ~kwd1 ~kwd2
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > data(ants)
>   > allindivs <- c(union(ants$VertexFrom, ants$VertexTo), "NULL1", "NULL2=
> ")
>   > g <- generatetonetwork(ants, allindivs)
>   > stp <- shortesttimepath(g, "WBGG", 927, "Q")
>   Warning in .Call("R_igraph_get_shortest_paths", graph, as.igraph.vs(gra=
> ph,  :
>     At structural_properties.c:4517 :Couldn't reach some vertices
>   Error in eval(expr, envir, enclos) : object 'X' not found
>   Calls: shortesttimepath ... tail -> [ -> [.igraph.vs -> lazy_eval -> ev=
> al -> eval
>   Execution halted
> 
> Package: treemap
> Check: examples
> New result: ERROR
>   Running examples in =E2=80=98treemap-Ex.R=E2=80=99 failed
>   The error most likely occurred in:
>   =
> 
>   > base::assign(".ptime", proc.time(), pos =3D "CheckExEnv")
>   > ### Name: treegraph
>   > ### Title: Create a tree graph
>   > ### Aliases: treegraph
>   > =
> 
>   > ### ** Examples
>   > =
> 
>   > data(business)
>   > treegraph(business, index=3Dc("NACE1", "NACE2", "NACE3", "NACE4"), sh=
> ow.labels=3DFALSE)
>   > treegraph(business[business$NACE1=3D=3D"F - Construction",],
>   +     index=3Dc("NACE2", "NACE3", "NACE4"), show.labels=3DTRUE, truncat=
> e.labels=3Dc(2,4,6))
>   > treegraph(business[business$NACE1=3D=3D"F - Construction",],
>   +     index=3Dc("NACE2", "NACE3", "NACE4"), show.labels=3DTRUE, truncat=
> e.labels=3Dc(2,4,6),
>   +     vertex.layout=3Digraph::layout.fruchterman.reingold)
>   Error in (function (graph, coords =3D NULL, dim =3D 2, niter =3D 500, s=
> tart.temp =3D sqrt(vcount(graph)),  : =
> 
>     unused arguments (circular =3D TRUE, root =3D 1)
>   Calls: treegraph -> do.call -> <Anonymous>
>   Execution halted
