# Simcenter Nastran - Cotter Joint Design - Transverse Shear
What seemed to be a straightforward analysis problem resulted in an in-depth deep-dive into **Stress Result Components**, study of the theory behind *Principal*, *Octahedral* and *Maximum Shear* stresses. And suitability of **2D Shell** elements for representing structures exposed predominantly to transverse shear based on their Degrees of Freedom and transferred loads.
Fantastic! This is precisely why I'm doing these micro-projects 😀

*Also, we can use anchor links on github* 😂
- [The Problem and Manual Analysis](#The-Problem-and-Manual-Analysis)
- [Full 3D Assembly](#Full-3D-Assembly)
- [2D Cotter Assembly ](#2D-Cotter-Assembly)
- [Cotter Only Attempts](#Cotter-Only-Attempts)

# The Problem and Manual Analysis
<img width="1043" height="729" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/hand_calc.jpg" />

# Full 3D Assembly
This is the version of the analysis that yielded results conforming to the manual analysis as It allowed me to replicate the specific boundary conditions presented in the theoretical problem
<img width="856" height="694" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/3d.jpg" />
<img width="1280" height="720" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/full3D_displacement.gif" />
<img width="1369" height="759" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/3d_stress.jpg" />

# 2D Cotter Assembly 
This is the case that prompted me to research exactly how 2D shell elements handle transverse loading and resultant pure transverse shear. TLDR: unless we're dealing with **Composites** we should use HEX elements instead
<img width="626" height="819" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/2d_cotter_assy.jpg" />

# Cotter Only Attempts
Try as I might I was unable to achieve satisfactory results through analyzing just the cotter. The requirement to remove all degrees of freedom to achieve convergence resulted in me over stiffening the component and reporting spurious results ☹
<img width="1500" height="780" alt="image" src="https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/blob/main/assets/cotter_only.jpg" />

[Back to Top](https://github.com/mgrzb451/Simcenter_Nastran-Cotter_Joint_design-Transverse_Shear/new/main?filename=README.md#simcenter-nastran---cotter-joint-design---transverse-shear)
