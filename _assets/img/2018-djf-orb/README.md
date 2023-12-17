# Pictures from Farnham et al 2018

This folder contains figures from our paper on regional extreme precipitation events in the Ohio River Basin. ake sure that your `.bib` file includes

```bibtex
@article{Farnham:2018gs,
  title = {Regional Extreme Precipitation Events: Robust Inference from Credibly Simulated {{GCM}} Variables},
  author = {Farnham, David J and {Doss-Gollin}, James and Lall, Upmanu},
  year = {2018},
  volume = {54},
  doi = {10.1002/2017wr021318},
  journal = {Water Resources Research},
  language = {English},
  number = {6},
}
```

Cite each figure as something like `\citet[fig.~3]{Farnham:2018gs}`.

## List of pictures with captions

For each figure you can find a caption, in LaTeX.
Assumes the use of the `sinuitx` packages and `glossaries` with the glossaries defined in `../my-papers/glossaries.tex`.
Note that you can, and probably should, write a shorter caption to use in Beamer.

**Figure 1**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_1.pdf}
	\caption[Map of the \acs{orb} study area]{
		Map of study area.
		Blue grid shows resolution of \gls{gfdl} \gls{cm3} coupled model cells.
		Red grid shows native resolution of \gls{cpc} precipitation data cells.
		The shaded area indicates the \gls{orb} ($\sim$ 530 000 km$^2$) as defined by the \gls{usgs}.
	}\label{fig:orb-area-map}
\end{figure}
```

**Figure 2**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{{Figure_2}.pdf}
	\caption[Relationship between streamflow and \acs{rep} days]{
		Relationship between streamflow and \acs{rep} days.
		(Left) Locations and drainage areas of the six long record streamflow stations.
		(Top, right) The seasonality of extreme streamflow ($>\approx$ 99.7th percentile) for each site in colors as expressed through the probability of extreme streamflow occurrence during each season.
		(Bottom, right) The log odds ratio of \cref{eqn:log_odds} and confidence interval associated with \gls{mam} days when one of more \gls{rep} days have occurred in the previous fifteen days vs. those when no \gls{rep} days have occurred in the previous 15 days and streamflow being above or below the $\approx$ 99.7th percentile.
		The odds ratio confidence interval was calculated via the unconditional maximum likelihood estimation (or the Wald method) via the \texttt{epitools} package of the R statistical programming language.
	}\label{fig:orb-RIP-streamflow}
\end{figure}
```
**Figure 3**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.75\textwidth]{{Figure_3}.pdf}
	\caption[
		Frequency distribution of \acs{rep} days in observations and \acs{gcm} output
	]{
		Frequency distribution of \gls{rep} days in observations and \gls{gcm} output.
		(a): The frequency distribution of the number of \gls{mam} \gls{rep} days by year for the observed record (red solid line) and the two \gls{gfdl} \gls{cm3} ensemble members (black solid lines).
		(b): The probability of a \gls{rep} event on a day given that a \gls{rep} event occurred the day prior divided by the marginal probability of a \gls{rep} event for the \gls{mam} season for the observed record and the two ensemble members.
		(c,d): as (a,b) but with the observed \nth{99} percentile precipitation thresholds used to derive the
		model \gls{rep} records.
		The bottom panels show that the discrepancy between the \gls{gcm} runs and the observed \gls{rep} records is even more stark when the observed precipitation data is used to calculate the \nth{99} percentile thresholds for the model and \gls{rep} records, an indication of a significant positive bias with respect to the \gls{gcm}'s \nth{99} percentile precipitation.
		In fact, the median of the study region's \nth{99} percentiles is 31 mm/day in the \gls{gfdl} \gls{cm3} model, and only \SI{25}{\milli\meter\per day} in the \gls{cpc} data.
	}\label{fig:orb-RIP-historic}
\end{figure}
```

**Figure 4**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_4.pdf}
	\caption[
		Daily $Z_{700}$ and $Q_{700}$ composite anomalies  and $Q_{700}$ from four days before each \acs{mam} \acs{rep} event to one day following the event
	]{
		Daily composites of $Z_{700}$ anomalies (shades) and $Q_{700}$ (contours at \SI{4e-4}{\kilo\gram\per\kilo\gram}) from four days before each \gls{mam} \gls{rep} event to one day following the event for the observed-reanalysis record.
		Solid contours represent positive anomalies and dashed contours represent negative anomalies.
		An ``X'' indicates that at least 80\% of composite members (\ie at least 37 of the 46 \gls{rep} events) had $Z_{700}$ anomalies of the same sign in that location.
	}\label{fig:orb-MAM-Z-Q}
\end{figure}
```

**Figure 5**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_5.pdf}
	\caption[
		Daily $Z_{700}$ and $Q_{700}$ composite anomalies on the day of \acs{rep} events in each of the \acs{gfdl} \acs{cm3} \acs{gcm} ensemble members and the observed-reanalysis record.
	]{
		Same as \cref{fig:orb-MAM-Z-Q} but for the day of the \gls{rep} event (lag = 0) and each of the \gls{gfdl} \gls{cm3} \gls{gcm} ensemble members and the observed-reanalysis record (panels).
		As in \cref{fig:orb-MAM-Z-Q}, an ``X'' indicates that at least 80\% of composite members had $Z_{700}$ anomalies of the same sign in that location.
		This 80\% criteria translates to at least 83 out of 103 \gls{rep} events, 92 out of 115 \gls{rep} events, and 37 out of 46 \gls{rep} events, for the two \gls{cm3} ensemble members and the observed-reanalysis record, respectively.
	}\label{fig:orb-MAM-mod-obs-gph}
\end{figure}
```

**Figure 6**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_6.pdf}
	\caption[
		Regions used to define the atmospheric indices used for statistical modeling and the distribution of these indices before and after \acs{rep} days.
	]{
		(Top) the regions that define each of the atmospheric indices.
		The index names are shown in red.
		The Ohio River basin, shown in more detail in \cref{fig:orb-area-map} is shaded in dark gray.
		The $\text{Z}_\text{P}$ index is defined by the average $Z_{700}$ within the area between \SIlist{130;155}{\degree W} and \SIlist{30;55}{\degree N} (leftmost dashed box), the $\text{Z}_\text{L}$  index is defined by the average $Z_{700}$ within the area between \SIlist{87.5;102.5}{\degree W} and \SIlist{30;45}{\degree N} (middle dashed box), and the $\text{Z}_\text{H}$ index is defined by the average $Z_{700}$ within the area between \SIlist{62.5;77.5}{\degree W} and \SIlist{30;45}{\degree N} (rightmost dashed box).
		The OMG and HUM indices are defined using the average atmospheric vertical velocity and specific humidity within the area between \SIlist{77.5;90}{\degree W} and \SIlist{36;42}{\degree N} (solid box).
		(Middle and bottom) The index values prior to and after the \gls{rep} events.
		The black line shows the median index value.
		The dark shaded area shows the range capturing the middle 50\% of days, while the light shaded area shows the range capturing the middle 90\% of days.
		All panels use the observed \gls{rep} record and the corresponding reanalysis-based atmospheric indices.
	}\label{fig:orb-index-location-time}
\end{figure}
```

**Figure 7**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_7.pdf}
	\caption[
		Cumulative distribution functions, serial correlation functions, and serial tail persistence functions for each of the climate-derived statistical indices.
	]{
		(Top) Cumulative distribution function for the \gls{mam} indices.
		(Middle) The serial correlation function for the \gls{mam} indices.
		(Bottom) The serial tail persistence of the \gls{mam} indices when in high states as shown by the probability of the index being above the 90th percentile on day t, given that the index was above that percentile on day t-lag, where lag values of 1 through 10 are shown along the x-axis.
		In all panels the solid line is the reanalysis-based indices and the dashed lines are the \gls{gcm} ensemble member-based indices.
		Negative OMG and $\text{Z}_\text{L}$ are shown for easier interpretation since low values of these two indices are associated with \gls{rep} days.
	}\label{fig:orb-cdf-persist-comp}
\end{figure}
```

**Figure 8**

```latex
\begin{figure}[ht]
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_8.pdf}
	\caption[
		Comparison of \acs{rep} day representation in observation and \acs{gcm} simulation.
	]{
		Comparison of \acs{rep} day representation in observation and \acs{gcm} simulation.
		(a) The number of \gls{mam} \gls{rep} days by year based on the two \gls{gfdl} \gls{cm3} ensemble member's precipitation fields (black solid lines), the mean of the simulated \gls{rep} counts obtained via the regression on the indices derived from the two \gls{gfdl} \gls{cm3} ensemble member's $Z_{700}$, $Q_{700}$, and $\omega_{700}$ fields (black dashed lines), and the 50th and 95th percentile prediction intervals based on the 1000 simulations (dark and light shaded regions, respectively).
		All data has been Gaussian kernel smoothed (bandwidth = 10 years) before the mean and prediction intervals are computed.
		The first and last 5 years of the smooths have been truncated from the figure to avoid edge effects.
		(b) The counts for the number of \gls{mam} \gls{rep} days by year for the observed record (solid red line), the record derived from the \gls{gfdl} \gls{gcm} \gls{cm3} precipitation fields (solid black lines), and the mean of the simulations for each ensemble member (dashed black lines).
		(c) Probability of a \gls{mam} \gls{rep} day on a day given that a \gls{rep} day occurred the day prior divided by the marginal probability of a \gls{rep} day for the observed record and the \gls{rep} simulated records for the two ensemble members and the observed record.
		The boxplot whiskers extend to points within 1.5 times the interquartile range above the 75th percentile, and any observation outside of this range is shown as a point.
	}
	\label{fig:orb-historical-simulations}
\end{figure}
```

**Figure 9**

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_9.pdf}
	\caption[
		Projected number of \acs{mam} \acs{rep} days using raw \acs{gcm} output, a naive bias correction, and the Bayesian logistic regression model.
	]{
		Projected number of \acs{mam} \acs{rep} days using raw \acs{gcm} output, a naive bias correction, and the Bayesian logistic regression model.
		(a) The projected number of \gls{mam} \gls{rep} days by year based on the \gls{gfdl} \gls{cm3} RCP 8.5 ensemble member precipitation field (black solid line), the mean of the simulated \gls{rep} counts obtained via the regression on the \gls{gcm}-based indices (black dashed lines), and the 50th and 95th percentile prediction intervals based on the 1000 simulations (dark and light shaded regions, respectively).
		The blue dashed line is the projected \gls{mam} \gls{rep} record when we assume that the historical bias between the \gls{gcm} and observed \gls{rep} frequency is multiplicative and stationary and we rescale the projection based on the \gls{gcm} precipitation field.
		In this case, this amounts to dividing the solid black line by about 2.2.
		All data has been Gaussian kernel smoothed (bandwidth = 10 years) before the mean and prediction intervals are computed.
		The first and last 5 years of the smooths have been truncated from the figure to avoid edge effects.
		(b) The counts for the number of \gls{mam} \gls{rep} days by year with corresponding line colors and types as in (a).
	}
	\label{fig:orb-future-simulations}
\end{figure}
```

**Figure 10**

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.95\textwidth]{Figure_10.pdf}
	\caption[
		\Acrshortpl{pdf} for the number of \acs{rep}s per year over three different time periods based on simulations from the Bayesian logistic regression model.
	]{
		Kernel density smoothed \glspl{pdf} showing the mean number of simulated \gls{mam} \gls{rep} days over the 30 year periods of 1970-1999 (red line) and 2070-2099 (short-dashed green line) and 2070-2099 after the trend in the HUM index has been removed (long-dashed blue line).
		Each curve is composed from 1000 points that represent the mean \# of \glspl{rep} per year in a 30 year simulation.
		}\label{fig:orb-HUM-effects}
\end{figure}
```

**Figure S1**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S1.pdf}
	\caption[Frequency distribution of local extreme precipitation days in \acs{gcm} simulations and observations]{
		The difference of frequency distributions (between the observed and two \gls{gcm} ensemble members) of local (one cell) extreme precipitation days by season (columns) over the historic record for all days with at least 1 local extreme precipitation event in the study region.
	}
	\label{fig:orb-IP-distribution}
\end{figure}
```

**Figure S2**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S2.pdf}
	\caption[The distribution of the regional extreme precipitation days by month for the observed record and \acs{gcm} ensemble members]{
		The distribution of the regional extreme precipitation days by month for the observed record and each of the two \gls{gcm} ensemble members.
		Note that the \gls{gcm} ensemble members are very similar and averaging across them does not significantly reduce the bias with respect to spring (\acs{mam}, or months 3, 4, and 5) and summer (\acs{jja}, or months 6, 7, and 8) \gls{rep} frequency.
	}
	\label{fig:orb-REP-seasonality}
\end{figure}
```

**Figure S3**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S3.pdf}
	\caption[Average precipitation percentiles when at least one of the 15 study area grid cells experienced a local \nth{99} percentile exceedance]{
		The precipitation percentiles (shading) averaged over all days when at least one of the 15 study area cells received rainfall greater than the 99th percentile for the observed and two \gls{gcm} ensemble members.
		All cells with mean percentile less than the 75th are shaded white.
	}
	\label{fig:orb-IP-percentile}
\end{figure}
```

**Figure S4**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S4.pdf}
	\caption[Difference between each \gls{gcm} ensemble member and the observed record of precipitation percentiles averaged over all \acs{rep} days.]{
		The difference between each \gls{gcm} ensemble member and the observed record of precipitation percentiles (shading) averaged over all \gls{rep} days.
	}
	\label{fig:orb-REP-lag-diff}
\end{figure}
```

**Figure S5**

```
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S5.pdf}
	\caption[
		Composites of $Z_{700}$ anomalies and absolute $Z_{700}$ during \acs{rep} days for observations and \acs{gcm} ensemble members.
	]{
		\Gls{mam} \gls{rep} day composites of $Z_{700}$ anomalies (shading) and absolute $Z_{700}$ (contours in \SI{50}{\meter} increments with 3000 m marked with a thicker contour) for both the observed/reanalysis (\ie reanalysis $Z_{700}$ during observed REPs) and each of the two \gls{gcm} ensemble members.
		Solid contours represent positive anomalies and dashed contours represent negative anomalies.
		An ``X'' indicates that at least 80\% of composite members had $Z_{700}$ anomalies of the same sign in that location.
		This 80\% criteria translates to at least 83 out of 103 \gls{rep} events, 92 out of 115 \gls{rep} events, and 37 out of 46 \gls{rep} events, for the two \gls{cm3} ensemble members and the observed-reanalysis record, respectively.
	}
	\label{fig:orb-MAM-mod-obs-Z}
\end{figure}
```

**Figure S6**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S6.pdf}
	\caption[
		The difference in standard deviation of daily \acs{mam} geopotential height at \SI{700}{\hecto\pascal} for between reanalysis and each \acs{gcm} ensemble member.
	]{
		The difference in standard deviation of daily \gls{mam} geopotential height at \SI{700}{\hecto\pascal} for the reanalysis and each of the two \gls{gcm} ensemble members.
		Note that the pattern associated with each ensemble member looks very similar, \ie averaging across ensemble members does not meaningfully reduce the bias with respect to the reanalysis record.
	}
	\label{fig:orb-zg-sd}
\end{figure}
```

**Figure S7**

```latex
\begin{figure}
	\centering
	\includegraphics[width=1\textwidth]{Figure_S7.pdf}
	\caption[
		Climatological zonal \SI{200}{\hecto\pascal} wind for reanalysis and each \acs{gcm} ensemble member.
	]{
		The climatological zonal wind \SI{200}{\hecto\pascal} (shading and contours) in \si{\meter\per\second} for the reanalysis and each of the two \gls{gcm} ensemble members.
		The contours show \SIlist{15;25;35}{\meter\per\second}.
		Note that the pattern associated with each ensemble member looks very similar, \ie averaging across ensemble members does not meaningfully reduce the bias with respect to the reanalysis record.
		}\label{fig:orb-u-200-mean}
\end{figure}
```

**Figure S8**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth,height=0.6\textheight,keepaspectratio=true]{Figure_S8.pdf}
	\caption[
		Qualitative diagnostics and checks for the Bayesian logistic regression model.
	]{
		(Top) Yearly record of the number of \gls{rep} days per year for the observed record (solid black points and line), the mean of the regression predicted record during the calibration period (solid blue points and line) and testing period (solid red points and line). 
		The 50th percentile prediction intervals are also shown for each year with blue and red vertical lines for calibration and testing periods, respectively. 
		(Second from top) The probability that the model simulates the observed number of \glspl{rep} in a year divided by the calibration sample probability of observing that same number of \glspl{rep} in a year for the calibration and testing samples (blue and red points and lines, respectively). 
		A ratio greater than one indicates skill. 
		The training and testing sample median ratios are shown with blue and red dashed lines. 
		(Third from top) The probability that the simulated number of \glspl{rep} in a year were less than the observed number of \glspl{rep} in a year. 
		Random noise with mean zero and standard deviation of 0.001 is added to the simulation derived yearly time-series to avoid the ties that result from the discrete nature of the data. 
		(Bottom) The discrete probability distribution of simulated number of \gls{rep} days for years where 0, 1, 2, or 3 \gls{rep} days were observed. That is, each column of tiles sums to 1. 
		A 1:1 line is shown via dashed lines.
	}
	\label{fig:orb-mod_check_2}
\end{figure}
```

**Figure S9**

```latex
\begin{figure}
	\centering
	\includegraphics[width=0.7\textwidth]{Figure_S9.pdf}
	\caption[
		The probability of a \acs{rep} event given a \acs{rep} event the day prior, divided by the marginal probability of a \acs{rep} event, for the observed record and 1000 simulated records from the Bayesian logistic regression model.
	]{
		The probability of a \gls{rep} event on a day given that a \gls{rep} event occurred the day prior divided by the marginal probability of a \gls{rep} event for the \gls{mam} season for the observed record (obs) and 1000 simulated records from the Bayesian regression model (sims) for the calibration (left) and testing (right) periods.
		The boxplot whiskers extend to points within 1.5 of the interquartile range, and any observation outside of this range is shown as a point.
	}
	\label{fig:orb-mod_check_3}
\end{figure}
```

**Figure S10**

```latex
\begin{figure}
	\centering
	\includegraphics[width=\textwidth]{Figure_S10.pdf}
	\caption[
		Wavelet power spectrum for the number of \acs{rep} events per year in observations and in simulations from the Bayesian logistic regression model.
	]{
		(Top) Wavelet power spectrum for the observed \# of \gls{rep} events by year. 
		Color indicates power and regions inside of the white borders are significant at the 90\% level as determined by shuffling the given time-series (\ie bootstrapping).
		(Bottom) Same as (Top) but for the mean model predicted \# \gls{rep} by year.
	}
	\label{fig:orb-mod_check_wave}
\end{figure}
```