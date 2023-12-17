# Pictures from Doss-Gollin et al 2019

This folder contains figures from our paper on flooding in Paraguay. Make sure that your `.bib` file includes

```bibtex
@article{DossGollin:2019,
  title = {Robust Adaptation to Multiscale Climate Variability},
  author = {{Doss-Gollin}, James and Farnham, David J. and Steinschneider, Scott and Lall, Upmanu},
  year = {2019},
  volume = {7},
  issn = {2328-4277},
  doi = {10.1029/2019EF001154},
  journal = {Earth's Future},
  language = {en},
  number = {7},
}
```

and then cite figures as something like \citep[fig.~5]{DossGollin:2019}.

## List of pictures with captions

For each ### Figure you can find a caption, in LaTeX.
Assumes the use of the `sinuitx` packages and `glossaries` with the glossaries defined in `../my-papers/glossaries.tex`.
Note that you can, and probably should, write a shorter caption to use in Beamer.

### Figure 1

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{observed-lfv.pdf}
	\caption[
		Time series and wavelet global spectra of some representative hydroclimate time series
	]{
		Hydroclimate time series vary on many time scales.
		(a) A \SI{500}{year} reconstruction of summer rainfall over Arizona from the \acrfull{lbda}.
		Lower values indicate more severe drought.
		A 20-year running mean is also shown in blue.
		(b) A \SI{100}{year} record of annual-maximum streamflow for the American River at Folsom.
		Daily streamflow values were divided by the catchment area to yield a normalized flow in units of \si{\milli\meter\per\day}.
		(c) The global wavelet power spectrum of the \gls{lbda} time series (a).
		Blue (red) dots indicate frequencies which are significant at $\alpha=0.10(0.05)$ compared to white noise.
		(d) Global wavelet power spectrum, like (c), for the American River data.
		}\label{fig:robust-observed-lfv}
\end{figure}
```

### Figure 2

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.7\textwidth]{conceptual-sketch.pdf}
	\caption[
		A stylized illustration of irreducible and estimation uncertainty.
	]{
		A stylized illustration of (a) irreducible and (b) estimation uncertainty.
		(a): Irreducible uncertainty cannot be resolved with better models or data and is dominated in the short term by chaotic behavior of the climate, and in the long term by the uncertainty in future \acrlong{acc}.
		(b): Informational uncertainty limits the potential to identify different climate signals.
		The blue line shows an idealized climate signal and the black line shows observations, which are scattered stochastically around the signal line.
		The green shading shows the true range within which observations will occur 95\% of the time, while the gray shading the 95\% confidence interval as estimated with a linear trend model.
		}\label{fig:robust-conceptual-sketch}
\end{figure}
```

### Figure 3

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{flowchart.pdf}
	\caption[
		Flow chart describing experiment design
	]{
		Flow chart describing experiment design.
		Parameters are shown in red.
		$N$ denotes the informational uncertainty (length of historical record) and $M$ the amount of extrapolation (project design life).
		Calculated quantities are shown in white.
		Quantities used for analysis are shown in blue.
		}\label{fig:robust-flowchart}
\end{figure}
```

### Figure 4

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{Example-NINO3-M100-N50.pdf}
	\caption[
		Illustration of the estimation procedure for a single time series
	]{
		An illustration of the estimation procedure.
		A single streamflow sequence with $N=50$ and $M=100$ is shown for each of the three cases (secular only, \gls{lfv} only, and secular plus \gls{lfv}) considered.
		The blue line shows the observed sequence.
		The gray shading indicates the 50\% and 95\% confidence intervals using each of the three fitting methods discussed (rows).
		The horizontal black line indicates the flood threshold.
		}\label{fig:robust-example-fit}
\end{figure}
```

### Figure 5

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{secular-only-nino3-bias-variance.pdf}
	\caption[
		Expected estimation bias and variance for sequences generated with secular change only (no \acs{lfv}).
	]{
		Expected estimation bias and variance for sequences generated with secular change only (no \gls{lfv}).
		Sequences were fit to each of three statistical models (columns) for different $N$ and $M$ ($x$ and $y$ axis, respectively).
		Top row shows estimation bias and bottom row shows log standard deviation of estimates.
		Note the uneven spacing of the $x$ and $y$ axes.
		}\label{fig:robust-secular-nino3-bias-variance}
\end{figure}
```

### Figure 6

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{secular-only-markov-bias-variance.pdf}
	\caption{
		As \cref{fig:robust-secular-nino3-bias-variance} for sequences generated with the two-state Markov chain model.
		}\label{fig:robust-secular-only-markov-bias-variance}
\end{figure}
```

### Figure 7

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{lfv-secular-nino3-bias-variance.pdf}
	\caption{
		As \cref{fig:robust-secular-nino3-bias-variance} but for sequences generated with both \gls{lfv} and secular change.
		}\label{fig:robust-lfv-secular-nino3-bias-variance}
\end{figure}
```

### Figure 8

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.75\textwidth]{M-N-Sketch.pdf}
	\caption{
		The importance of predicting different signals, and the identifiability and predictability of the signals, depends on the degree of informational uncertainty ($N$) and the project planning period ($M$).
		}\label{fig:robust-m-n-sketch}
\end{figure}
```

### Figure S1

```latex
\begin{figure}
  \centering
  \includegraphics[width=0.5\textwidth]{Bias-Variance-Sketch.pdf}
  \caption{
    Consequences of model bias or incorrect model representation of uncertainty.
    If an estimate has a positive bias and overestimates uncertainty, the instrument may be too expensive.
    If an estimate has negative bias and underestimates uncertainty, it will be likely to fail.
  }\label{fig:conceptual-bias-variance}
\end{figure}
```

### Figure S2

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{enso_wavelet.png}
	\caption{
	Wavelet analysis of the synthetic annual NINO3 time series described in Section 2.1.
	(L): wavelet power spectrum.
	Note that the color bar uses a quantile scale and is thus nonlinear.
	(R): global (average) power spectrum.
	Blue dots indicate frequencies which are significant at $\alpha=0.10$ and red dots frequencies which are significant at $\alpha=0.05$ compared to white noise.
	}\label{fig:enso-ts}
\end{figure}
```

### Figure S3

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{secular-only-markov-bias-variance.pdf}
	\caption{
	Secular change: as ### Figure 5 for sequences generated with the two-state Markov chain model.
	}\label{fig:secular-only-markov-bias-variance}
\end{figure}
```

### Figure S4

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{lfv-only-markov-bias-variance.pdf}
	\caption{
	LFV only: as ### Figure 6 for sequences generated with the two-state Markov chain model.
	}\label{fig:lfv-markov-bias-variance}
\end{figure}
```

### Figure S5

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.8\textwidth]{lfv-secular-markov-bias-variance.pdf}
	\caption{
	LFV plus secular change: as ### Figure 7 for sequences generated with the two-state Markov chain model.
	}\label{fig:lfv-secular-markov-bias-variance}
\end{figure}
```