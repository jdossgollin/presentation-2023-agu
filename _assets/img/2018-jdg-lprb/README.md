# Pictures from Doss-Gollin et al 2018

This folder contains figures from our paper on flooding in Paraguay. Make sure that your `.bib` file includes

```bibtex
@article{DossGollin:2018bn,
  title = {Heavy Rainfall in {{Paraguay}} during the 2015-2016 Austral Summer: Causes and Sub-Seasonal-to-Seasonal Predictive Skill},
  author = {{Doss-Gollin}, James and Mu{\~n}oz, {\'A}ngel G and Mason, Simon J and Past{\'e}n, Max},
  year = {2018},
  volume = {31},
  pages = {6669--6685},
  doi = {10.1175/JCLI-D-17-0805.1},
  journal = {Journal of Climate},
  language = {English},
  number = {17},
  open = {true},
  preprint = {https://eartharxiv.org/gzj8n/},
  repo = {https://github.com/jdossgollin/2018-paraguay-floods}
}
```

and then cite figures as something like \citep[fig.~5]{DossGollin:2018bn}.

## List of pictures with captions

For each figure you can find a caption, in LaTeX.
Assumes the use of the `sinuitx` packages and `glossaries` with the glossaries defined in `../my-papers/glossaries.tex`.
Note that you can, and probably should, write a shorter caption to use in Beamer.

**Figure 1**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{study_area.jpg}
	\caption[Topographical map of the \acs{lprb}]{
		Topographical map of the study area.
		Colors indicate $\log_{10}$ of elevation, in \si{\meter}, from the Global Land One-Km Base Elevation project available at \texttt{http://iridl.ldeo.columbia.edu/SOURCES/.NOAA/.NGDC/.GLOBE/.topo/}.
		(a): all of South America.
		The domains of the \acrlong{lprb} and the domain used for weather typing are indicated in red and blue, respectively.
		(b): The \acrfull{lprb}.
		As for (a), the \gls{lprb} is marked with a red box.
		Streamflow time series shown in \cref{fig:lprb-streamflow} were taken from the fours stations indicated.
		The Paraguay River and its tributaries, from the Natural Earth database (\url{www.naturalearthdata.com}), are also shown.
		Full station names are: Bahía Negra (Bne); Concepción (Conc); Asunción (Asu); Pilar (Pil).
		}\label{fig:lprb-study-area}
\end{figure}
```

**Figure 2**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{anomalies_ndjf1516.pdf}
	\caption[Monthly composite anomalies observed during \acs{ndjf} 2015-16]{
		Monthly composite anomalies observed during \gls{ndjf} 2015-16.
		Top row (a-d) shows streamfunction anomalies at \SI{850}{\hecto\pascal}, in units of \si{\meter\squared\per\second}.
		Bottom row (e-h) shows rainfall anomalies, in units of \si{\milli\meter\per\day}.
		}\label{fig:lprb-anomalies}
\end{figure}
```

**Figure 3**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{Streamflow.pdf}
	\caption[River stage time series for four gauges on the Paraguay River]{
		River stage (height; in \si{\meter}) for the Paraguay River at four gauges along the Paraguay River.
		The station names are shortened versions of those shown in \cref{fig:lprb-study-area}.
		(a): Seasonality (orange) and time series of 2015-16 observations (black) at each stream gauge.
		Seasonality was fit using local polynomial regression as implemented in the \texttt{locfit} package in the \textbf{R} statistical programming environment \citep{Loader:1999vo}.
		(b): Time series of daily stage measurements from 1929 to 2016 at each station.
		}\label{fig:lprb-streamflow}
\end{figure}
```

**Figure 4**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{lagged_rain.pdf}
	\caption[Composite anomalies associated with heavy rainfall in the \acs{lprb}]{
		Composite anomalies associated with heavy rainfall (\nth{90} percentile exceedance of area-averaged rainfall in the \acrlong{lprb}).
		Lagged composites are shown, by column, for $t = $ \SIlist{-2;-1;0;1}{\day} relative to the date of heavy rainfall.
		Top row (a-d) shows composite streamfunction and wind anomalies at \SIlist{850}{\hecto\pascal}.
		Strongest 5\% of wind anomaly vectors between \SI{60}{\degree S} and \SI{10}{\degree N} (all longitudes) are also shown.
		Bottom row (e-h) shows composite rainfall anomalies, in units of \si{\milli\meter\per\day}.
		}\label{fig:lprb-lagged-rain}
\end{figure}
```

**Figure 5**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{eof_loadings.pdf}
	\caption[Loadings of the four leading \acs{eof}s of daily \acs{ndjf} \SI{850}{\hecto\pascal} streamfunction]{
		Loadings of the four leading \glspl{eof} of daily \gls{ndjf} \SI{850}{\hecto\pascal} streamfunction over the weather typing region shown in \cref{fig:lprb-study-area}.
		Parentheses in sub-plot titles indicate the percentage of total variance explained by each \gls{eof}.
		}\label{fig:lprb-eof-loading}
\end{figure}
```

**Figure 6**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth,height=8in,keepaspectratio=true]{wt_composite.pdf}
	\caption[Composite anomalies associated with each weather type]{
		Composite anomalies associated with each weather type.
		Top row (a-f) shows streamfunction anomalies at \SIlist{850}{\hecto\pascal}.
		Strongest 20\% of wind anomaly vectors over the plot area are also shown.
		Bottom row (g-l) shows rainfall anomalies, in units of \si{\milli\meter\per\day}.
		The relative frequency of occurrence of each weather type (in days) is presented on the top of each column.
		}\label{fig:lprb-wt-composite}
\end{figure}
```

**Figure 7**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{rain_wt_201516.pdf}
	\caption[Time series of area-averaged rainfall in the \acs{lprb} for \acs{ndjf}  2015-16]{
		Time series of area-averaged rainfall in the \acrlong{lprb} (\cref{fig:lprb-study-area}) for each day of \gls{ndjf}  2015-16.
		Lines indicate the rainfall value, in units of \si{\milli\meter\per\day}.
		The weather type corresponding to each day is indicated in an adjacent text label.
		Dashed lines blue indicate (from bottom to top) the climatological 50th, \nth{90}, and 99th percentiles of \gls{ndjf} area-averaged rain over the \acrlong{lprb}.
		}\label{fig:lprb-rain-wt}
\end{figure}
```

**Figure 8**

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.5\textwidth]{seasonal_forecast.pdf}
	\caption[Seasonal model forecast for probability of exceedance of \nth{90} percentile of \acs{djf} rainfall, as issued in November 2015]{
		Seasonal model forecast for probability of exceedance of \nth{90} percentile of DJF rainfall, as issued in November 2015.
		Color indicates the forecast probability of exceeding the \nth{90} percentile of climatological rainfall during DJF 2015-16 -- this is presented as the odds ratio as defined in \cref{eq:odds-ratio}.
		A value greater than 1 indicates that the model forecast greater-than-average odds of rainfall exceeding the \nth{90} percentile.
		Grid cells which observed an exceedance of the \nth{90} percentile of DJF rainfall are outlined in black.
		}\label{fig:lprb-seas-prob-fcst}
\end{figure}
```

**Figure 9**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{chiclet.pdf}
	\caption[Chiclet diagram of ensemble-mean precipitation anomaly forecasts over the \acs{lprb} for \acs{ndjf} 2015-16]{
		Chiclet diagram \citep[see][]{Carbin:2016fx} of ensemble-mean precipitation anomaly forecasts over the \acrlong{lprb} (see \cref{fig:lprb-study-area}) from uncorrected \gls{ecmwf} \gls{s2s} model forecast data, as a function of the forecast target date (horizontal axis) and lead time (vertical axis).
		Time series of CPC daily mean precipitation over the same area is plotted with $y$-axis inverted; horizontal black line denotes \gls{ndjf} climatology.
		}\label{fig:lprb-chiclet}
\end{figure}
```

**Figure 10**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{mos_forecasts.pdf}
	\caption[Raw and \acs{mos}-adjusted \acs{s2s} model forecasts and spatial skill scores]{
		Raw and \gls{mos}-adjusted \gls{s2s} model forecasts and skill scores for the methods indicated in \cref{tab:lprb-mos-methods}.
		Top row (a-e) shows the heavy rainfall forecast for 1-7 December 2015 as the odds ratio defined in \cref{eq:odds-ratio} over the target domain.
		A value greater than 1 indicates that the model forecast greater-than-average odds of rainfall exceeding the \nth{90} percentile.
		Second row (f-j) shows the Ignorance Score defined in \cref{eq:ignorance}, with zero indicating a perfect forecast.
		Bottom row (k-o) shows the 2AFC skill score for each grid cell; a value greater than 50 indicates that the model outperforms climatology.
		Columns separate different \gls{mos} models except for ``Raw'' (a,f,k), which indicates the uncorrected \gls{s2s} model output.
		For all rows the grid cells which observed a \nth{90} percentile exceedance for 1-7 December 2015 are outlined in black.
		}\label{fig:lprb-subs-prob-fcst}
\end{figure}
```

**Figure 11**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{wt_mjo_enso.pdf}
	\caption[Anomalous probability of occurrence of each weather type concurrent with observance of each \acs{mjo} and \acs{enso} phase]{
		Anomalous probability of occurrence of each weather type concurrent with observance of each \gls{mjo} phase.
		When \gls{mjo} amplitude is less than 1, it is defined as neutral phase (0).
		Plots are shown separately for El Niño (NINO 3.4 $>1$), La Niña (NINO 3.4 $< -1$), and Neutral \gls{enso} phases.
		Only values which are significant at $\alpha=0.10$, calculated with a bootstrap of 5000 samples, are shown.
		}\label{fig:lprb-wt-mjo-enso}
\end{figure}
```

**Figure 12**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{ChacoNoChacojet.pdf}
	\caption[Schematics of low-level jet events (red arrows) during austral summer and El Niño years]{
		Schematics of low-level jet events (red arrows) during austral summer and El Niño years.
		Most jet events are of the ``Chaco'' type, particularly when \gls{sst} anomalies in the central southern Atlantic Ocean (a, see green box) are weak.
		When a dipole \gls{sst} anomaly occurs in the central southern Atlantic with the warmer pole equatorward, the meridional temperature gradient and sea-land temperature contrasts establish an anticyclonic circulation (dot-dashed line) conducive to increased occurrence of No-Chaco jet events (b).
		Other \gls{sst} anomaly configurations tend to be present outside the green box (not shown).
		Winds in panels are typical for each case (at \SI{850}{\hecto\pascal}).
		Reference wind vector in \si{\meter\per\second}.
		Green box shows location of \gls{scad}.
		}\label{fig:lprb-chaco-nochaco}
\end{figure}
```

**Figure S1**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth,height=0.4\textheight,keepaspectratio=true]{gpw-v4-2015.png}
	\caption[Gridded estimate of population density]{
		Gridded estimate of population density (color; in units of persons per square kilometer) \citep[image from][]{CenterforInternationalEarthScienceInformationNetwork:2016tv}.
		}\label{fig:lprb-population-density}
\end{figure}
```

**Figure S2**

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{wt_classifiability.pdf}
	\caption{
		Classifiability index as a function of of $K$ (the number of weather types created).
		}\label{fig:lprb-s2}
\end{figure}
```

**Figure S3**

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{nino_34_ts.pdf}
	\caption[Monthly NINO 3.4 time series during the study period]{
		Monthly NINO 3.4 time series during the study period.
		Each month from November 2015 through February 2016 is specifically marked with a blue dot.
		Data from \citet{Kaplan:1998df}.
		}\label{fig:lprb-s3}
\end{figure}
```

**Figure S4**

```latex
\begin{figure}
	\includegraphics[width=\textwidth, height=\textheight, keepaspectratio=true]{nino_sst_anomalies.pdf}
	\caption[Monthly \acrshort{sst} anomalies during December of three major El Niño events.]{
		Monthly \gls{sst} anomalies during December of three major El Niño events.
		Months shown are \gls{ndjf} of (a,d,g,j): 1982-83, (b,e,h,k): 1997-98, and (c,f,i,l): 2015-16.
		Units are in \si{\celsius}.
		\Gls{sst} data from \citet{reynolds_insitu:2002}.
		Also shown are rainfall anomalies over South America, from \citet{Chen:2008gd}.
		Rainfall contour intervals are \SI{1}{\milli\meter\per\day}.
		}\label{fig:lprb-s4}
\end{figure}
```

**Figure S5**

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{mjo_ts.pdf}
	\caption[Evolution of the \acrshort{mjo} during NDJF 2015-16]{
		Evolution of the \gls{mjo} during NDJF 2015-16.
		Points are plotted on RMM1 ($x$-axis) and RMM2 ($y$-axis), derived from leading \glspl{eof} of \gls{olr} fields \citep{Wheeler:2004ea}.
		Gray lines divide the plot into the eight phases used in the text.
		Colors show the time evolution of the system from 01 November 2015 (blue) to 29 February 2016 (yellow).
		Gray circle indicates the area of neutral \gls{mjo} activity with amplitude $<0$.
		}\label{fig:lprb-s5}
\end{figure}
```

**Figure S6**

```latex
\begin{figure}
    \includegraphics{sst_anomalies.pdf}
    \caption{
        Pearson correlation, at monthly time step, of \gls{sst} anomalies \citep{reynolds_insitu:2002} with four leading \glspl{eof} of \SI{850}{\hecto\pascal} streamfunction over the weather typing region, shown with a black box.
        \gls{scad} is shown with a blue box.
        (a): \acrshort{eof}41; (b): \acrshort{eof}2; (c): \acrshort{eof}3; (d): \acrshort{eof}4.
    }\label{fig:sst-anomalies}
\end{figure}
```

**Figure S7**

```latex
\begin{figure}
	\includegraphics[width=\textwidth]{predictors_eofs.pdf}
	\caption{
		Spearman (rank) correlation coefficient between several S2S climate indices and weather type occurrence at monthly time step.
		These correlations are computed between the proportion of occurrence of each weather type and the monthly-mean time series of the climate index.
		For the MJO phases the monthly-mean time series is the proportion of occurrence of that phase for the given month.
		The NINO 3.4 time series was up-sampled from monthly to daily values by persisting the most recent monthly value (no interpolation).
		The SCAD predictor, labeled Dipole, is the mean meridional gradient of SST anomalies over the region \SIrange{30}{10}{\degree W} and \SIrange{40}{15}{\degree S}, up-sampled to daily values using the same method as the NINO 3.4 time series.
	}\label{fig:predictor-eof}
\end{figure}

```
