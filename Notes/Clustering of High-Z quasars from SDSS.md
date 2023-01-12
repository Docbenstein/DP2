- Sample contains 4,426 luminous optical quasars
- Redshift $2.9 \leq z \leq 5.4$
- Power law fit $\xi(r) = (r/r_0)^{-\gamma}$: 
	- $r_0 = 15.2 \pm 2.7 h^{-1}Mpc$.
	- $\gamma = 2.0 \pm 0.3$
	- Scale range $4 \leq r_p \leq 150 h^{-1}Mpc$
- For $z \approx 1.5$, $r_0 \approx 6.5 h^{-1}Mpc$
- Sample is devided into two redshift bins assuming $\gamma = 2.0$:-
- $2.9 \leq z \leq 3.5$:
	- $r_0 = 16.9\pm 1.7h^{-1}Mpc$
	- $Duty = 0.004 \sim 0.05$ 
	- $t_Q = 4 \sim 50 Myr$
	- $M_{min} = 2-3 \times 10^{12} h^{-1}M_0$
	- $b_{eff}\sim8$ at $z=3.0$
- $z \geq 3.5$:
	- $r_0 = 24.3\pm 2.4 h^{-1}Mpc$
	- $Duty = 0.03 \sim 0.6$
	- $t_Q = 30 \sim 600 Myr$
	- $M_{min} = 4-6\times10^{12}h^{-1}M_0$
	- $b_{eff} \sim 16$ at $z = 4.5$


### Questions

- Why data is devided into two bins?
- What does it mean to say, quasar locus crosses the stellar locus in color space at $z \approx 2.7$ [Fan 1999]?
- What is the quasar selection algorithm in SDSS?
- Overlapping plates?
- 
### Sample selection

- 2.5 wide-field telescope, drift scan camera with 30 CCDs, images sky in 5 boad bands ($ugriz$)
- Candiates for followup spectroscopy are selected using their colors, and arranged in spectro plates for [[double spectroscopy]]
- Spectroscopy is carried out over 5740 $deg^2$.
- Selection algorithm:
	- $z\leq 3.5$ are outliers from the stellar locus in the ugri color cube.
	- $z>3.5$ are outliers from the griz color cube.
- Quasar candidate sample is flux limited to $i = 19.1$ and at $z > 3$ to $i = 20.2$.

### Redshift space correlation function

- Redshift space is where distances are obtained from redshift without any corrections for peculiar velocity of redshift errors.
- Redshift space correlation function[Landy & Szalay(1993)]$$\xi(s) = \frac{\langle DD\rangle - 2\langle DR \rangle + \langle RR \rangle}{\langle RR\rangle}$$
- **Jackknife**:  10 spatially contiguous subsambles are made from the data sets and jackknife samples are created by omitting each of these samples in turn and mean of the number of data points in bin $s$ for each jackknife samble is taken as $DD_{mean}$, used in place of $\langle DD \rangle$. Covaraince matrix is calculated as,$$Cov(\xi_i,\xi_j) = \frac{N-1}{N}\sum^N_{l=1} (\xi_i^l - \bar\xi_i)(\xi_j^l - \bar\xi_j)$$
- **Poisson error estimator**: 

### Real Space correlation function

- Redshift space distortion due to peculiar motion of quasars in the cluster, called **Fingers of God**.![Alt test](https://ned.ipac.caltech.edu/level5/March12/Coil/Figures/figure4.jpg "Fingers of God")
- Projected correlation function $w_p(r_p)$: $$w_p(r_p) = 2 \int_0^\infty d\pi \xi_s(r_p, \pi)$$
- where, $$\pi = \frac{s\cdot l}{|l|} \hspace{1cm} r_p = \sqrt{s\cdot s - \pi^2}$$
- In practice integration is only upto $\pi_{cutoff} = 100h^{-1}Mpc$. 
- Now relation between projected correlation function and real space correlation function:$$w_p(r_p) = 2\int_0^\infty dy\xi(\sqrt{r_p^2 + y^2})$$$$w_p(r_p) = 2\int_0^\infty \frac{rdr}{\sqrt{r^2 - r_p^2}}\xi(r)$$$$w_p(r_p) = r_p\left(\frac{r_o}{r_p}\right)^\gamma \frac{\Gamma(1/2)\Gamma[(\gamma -1)/2]}{\Gamma(\gamma/2)}$$
- Now angular correlation function can be fitted with this function to obtain $\gamma$ and $r_0$.
- The predicted correlation function of the underlying dark matter at $r = 15h^{-1}Mpc$ is $\sim 0.014$ at $z = 3.5$, far below that of the current high redshift quasar sample $\sim 22.92$.
- The clustering of quasars increases strongly with redshift over the range probed by our sample.

### Appendix A. Quasar redshift determination

- Mg II line has a small and known offset from the systemic redshift. 