# Acoustic scattering and forces on an arbitrarily sized fluid sphere by a general acoustic field
## Authors: M. Pessôa, A.A.R. Neves 

In the .nb files we describe how we obtained results presented in the paper Acoustic scattering and forces on an arbitrarily sized fluid sphere by a general acoustic field.

Simulations include the scattering of a plane wave emitted on a spherical surface, and the reconstructed beam for an arbitrarily localized Bessel Beam. Also, we calculate the profiles for acoustic radiation force for a plane wave and a Bessel Beam. We also present the convergence for the different expansion coefficients. 

In this repository: 
 - Bessel_PressureField_v1.nb corresponds to the reconstruction of an arbitrarily located Bessel Beam reconstructed by the multipole expansion coefficients. The function was written in spherical coordinates, and using Bessel's addition theorem, yielding, 
 
 <a href="https://www.codecogs.com/eqnedit.php?latex=J_q(k&space;\rho&space;\sin&space;\beta)&space;\mathrm{e}^{\mathrm{i}q&space;\varphi}=&space;\mathrm{e}^{\mathrm{i}q\phi}\sum_{p=-\infty}^{\infty}&space;J_p&space;(k&space;\rho_0&space;\sin&space;\beta)&space;J_{p&plus;q}&space;(k&space;r&space;\sin&space;\theta&space;\sin&space;\beta)&space;\mathrm{e}^{\mathrm{i}p(\phi-\phi_0)}." target="_blank"><img src="https://latex.codecogs.com/gif.latex?J_q(k&space;\rho&space;\sin&space;\beta)&space;\mathrm{e}^{\mathrm{i}q&space;\varphi}=&space;\mathrm{e}^{\mathrm{i}q\phi}\sum_{p=-\infty}^{\infty}&space;J_p&space;(k&space;\rho_0&space;\sin&space;\beta)&space;J_{p&plus;q}&space;(k&space;r&space;\sin&space;\theta&space;\sin&space;\beta)&space;\mathrm{e}^{\mathrm{i}p(\phi-\phi_0)}." title="J_q(k \rho \sin \beta) \mathrm{e}^{\mathrm{i}q \varphi}= \mathrm{e}^{\mathrm{i}q\phi}\sum_{p=-\infty}^{\infty} J_p (k \rho_0 \sin \beta) J_{p+q} (k r \sin \theta \sin \beta) \mathrm{e}^{\mathrm{i}p(\phi-\phi_0)}." /></a>
 
 - Convergence_V1.nb describes the convergence methods used for the scattered field coefficient <a href="https://www.codecogs.com/eqnedit.php?latex=C_{lm}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?C_{lm}" title="C_{lm}" /></a>
 
 - Acoustic radiation force was calculated by solving, 
  <a href="https://www.codecogs.com/eqnedit.php?latex=\mathbf{F}^{\bold{rad}}=-\frac{|p_0|^2}{4\rho\omega^2}&space;\operatorname{Re}\left[&space;\sum_{lmpq}(i)^{p-l}\left(&space;2C_{lm}C_{pq}^{*}&plus;C_{lm}G_{pq}^{*}&plus;G_{lm}C_{pq}^*\right)&space;\int_{\mathrm{d}\Omega}&space;Y_{lm}(\theta,\phi)Y_{pq}^{*}(\theta,\phi)&space;\hat{\mathbf{r}}\,\mathrm{d}\Omega\right]" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\mathbf{F}^{\bold{rad}}=-\frac{|p_0|^2}{4\rho\omega^2}&space;\operatorname{Re}\left[&space;\sum_{lmpq}(i)^{p-l}\left(&space;2C_{lm}C_{pq}^{*}&plus;C_{lm}G_{pq}^{*}&plus;G_{lm}C_{pq}^*\right)&space;\int_{\mathrm{d}\Omega}&space;Y_{lm}(\theta,\phi)Y_{pq}^{*}(\theta,\phi)&space;\hat{\mathbf{r}}\,\mathrm{d}\Omega\right]" title="\mathbf{F}^{\bold{rad}}=-\frac{|p_0|^2}{4\rho\omega^2} \operatorname{Re}\left[ \sum_{lmpq}(i)^{p-l}\left( 2C_{lm}C_{pq}^{*}+C_{lm}G_{pq}^{*}+G_{lm}C_{pq}^*\right) \int_{\mathrm{d}\Omega} Y_{lm}(\theta,\phi)Y_{pq}^{*}(\theta,\phi) \hat{\mathbf{r}}\,\mathrm{d}\Omega\right]" /></a>
  
 and obtaining the (x,y,z) components for scattering <a href="https://www.codecogs.com/eqnedit.php?latex=C_{lm}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?C_{lm}" title="C_{lm}" /></a> and incident <a href="https://www.codecogs.com/eqnedit.php?latex=G_{lm}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?G_{lm}" title="G_{lm}" /></a> coefficients.

- The resulting acoustic radiation force was calculated for both Bessel Beam and Plane Wave cases, of incident forms: 
<a href="https://www.codecogs.com/eqnedit.php?latex=P_{\mathrm{inc}}(r,\theta,\phi)=p_0&space;\mathrm{e}^{\mathrm{i}kr&space;\cos&space;\theta&space;\cos&space;\beta}J_q(kr&space;\sin&space;\theta\sin&space;\beta&space;)\mathrm{e}^{\mathrm{i}q\phi}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?P_{\mathrm{inc}}(r,\theta,\phi)=p_0&space;\mathrm{e}^{\mathrm{i}kr&space;\cos&space;\theta&space;\cos&space;\beta}J_q(kr&space;\sin&space;\theta\sin&space;\beta&space;)\mathrm{e}^{\mathrm{i}q\phi}" title="P_{\mathrm{inc}}(r,\theta,\phi)=p_0 \mathrm{e}^{\mathrm{i}kr \cos \theta \cos \beta}J_q(kr \sin \theta\sin \beta )\mathrm{e}^{\mathrm{i}q\phi}" /></a>

<a href="https://www.codecogs.com/eqnedit.php?latex=\dpi{100}&space;P_{\mathrm{inc}}(r,\theta,\phi)=p_0\mathrm{e}^{\mathrm{i}k^{E}r\cos\theta}\mathrm{e}^{-\mathrm{i}k^Ez0}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\dpi{100}&space;P_{\mathrm{inc}}(r,\theta,\phi)=p_0\mathrm{e}^{\mathrm{i}k^{E}r\cos\theta}\mathrm{e}^{-\mathrm{i}k^Ez0}" title="P_{\mathrm{inc}}(r,\theta,\phi)=p_0\mathrm{e}^{\mathrm{i}k^{E}r\cos\theta}\mathrm{e}^{-\mathrm{i}k^Ez0}" /></a>

respectively.
