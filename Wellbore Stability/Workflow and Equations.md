# Workflow
This workflow is for extensional tectonic settings where $S_{V}$ = $\sigma_{1}$, $S_{Hmax}$ = $\sigma_{2}$, and $S_{hmin}$ = $\sigma_{3}$. To calculate $S_{V}$ we integrate the density log ($\rho_{b}$) by the accel multiplied by from TVDSS (h) = 0 to a given depth (h):
$S_{V}=\int_{0}^{h} \rho_{b} g h$
#### 1. Sonic analysis - Assess Vp and Vs logs. If no Vs log is available, a correlation can be made using: ${V_{s}}= 0.77 \times  {V_{p}} - 0.86$
#### 2. Then calculate the elastic properties. First, start with the elastic Young's modulus using Vp and Vs logs: ${E_{d} (PSI)}= 1.34 \times 10^{10} \times \frac{\rho_{b}}{{\Delta t_{s}^{2}}} \times \frac{(3 \Delta t_{s}^{2} - 4 \Delta t_{p}^{2})}{(\Delta t_{s}^{2} - \Delta t_{p}^{2})}$
#### 2a. $Shear Modulus (G: PSI) = 1.34 \times 10^{10} \times \frac{\rho}{{\Delta t_{s}^{2}}}$
 $\Delta t$ is in us/ft and $\rho_{b}$ is in g/cc.
#### 3. Then calculate the dynamic Poisson's ratio: $v_{d} = \frac{(\frac{\Delta t_{s}}{\Delta t_{p}})^{2}-2}{2 (\frac{\Delta t_{s}}{\Delta t_{p}})^{2}-1}$
##### 3a. An alternative equation to determine the Young's Modulus is: $E_{d} = 2G(1+v)$
#### 4. Remember that the static Young's Modulus is up to 8x smaller than the dynamic, so use correlation equation: $E_{s} = 0.414E_{d} -1.059$
#### 5. This can be calibrated with real measurements from tri-axial tests if you have them.

# Poro-elastic equations:
In poro-elastic equations we usually assume that the Biot's coefficient ($\alpha$) = 1. More so, $S_{hmin}$ can also be deduced from Leak-off Tests (LOTs), but Extended Leak-off tests (XLOTs) are preferable as the second cycle gives a much more reliable estimate whilst also disregarding the tensile strength of a rock because it has already been fractured.
### $S_{hmin}$:
##### $$\sigma_{h} = \frac{v}{(1-v)}(\sigma_{V} - \alpha P_{P}) + \alpha P_{P} + \frac{E_{sta}}{(1-v^{2})}(\varepsilon_{x} + v\varepsilon_{y})$$
### $S_{Hmax}$:
##### $$\sigma_{H} = \frac{v}{(1-v)}(\sigma_{V} - \alpha P_{P}) + \alpha P_{P} + \frac{E_{sta}}{(1-v^{2})}(\varepsilon_{y} + v\varepsilon_{x})$$

####  We can also calculate the horizontal stresses where if $\rho_{b} = 3\sigma_{h} - \sigma_{H} - P_{P} + T_{0}$:
where $\rho_{b}$ is bulk density, $\sigma_{h}$ is *S~hmin~*, $\sigma_{H}$ is *S~Hmax~*, $P_{P}$ is pore pressure (hydrostatic), and $T_{0}$ is tensile strencth

Re-arranging this formula we can thus deduce that $\sigma_{H} = 3\sigma_{h} - \rho_{b} - P_{P} + T_{0}$. However, as stated above, if we already has $S_{hmin}$ from $2^{nd}$ cycle XLOTs, then we can disregard the tensile strength (
$\sigma

### 6. UCS can be calculated using the equations in this table:
| UCS (MPa)| Fm. Type| Ref.
| -------- | ------- |------------------|
| $$0.03V_{P}-31.5$$  | Any| Freyburg (1972) |
| $$1200 \times \exp{(-0.036\Delta t)}$$ | Sandstone | McNally (1987) |
| $$2.28 + 4.1089E$$  | Any | Bradford et al. (1998) |
| $$254(1-2.7\Phi^{2})$$ | Any | Vernik et al. (1993) |
| $$(0.77304.8/\Delta t)^{2.93}$$ | Shale | Horsrud (2001) |
| $$7.97E^{0.91}$$ | Shale | Lal (1999) |
| $$2.922\Phi^{-0.96}$$ | Shale | Horsrud (2001) |
| $$13.8E^{0.34}$$ | Limestone | Golubev and Rabinovich (1976) |
###### Where E is the static Young's Modulus, $$\Phi$$ is porosity, $$\Delta t$$ is sonic is us/ft, and $$V_{P}$$ is P-wave velocity.
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjc1ODc0MzAyLC02NTkxMTA2MDYsLTEzOT
IxMzA3MTJdfQ==
-->