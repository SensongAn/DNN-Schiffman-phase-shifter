# Schiffman phase shifter dataset (single section)
The input parameters, simulation environment and results are defined below:  

<img src="https://github.com/SensongAn/DNN-Schiffman-phase-shifter/blob/main/pics/1.jpg" width="50%">

-   **Substrate:** The phase shfiters are constructed based on the **Rogers R4003C** dielectric substrate, with the thickness of **1.524mm**, permittivity of **3.55** and loss tangent of **0.0027**. 

-   **Conductor:** **Copper (lossy, annealed)** for both microstrip circuits above the substrate and GND beneath.

-   **Substrate dimensions:** Width of all phase shifters are fixed to be 50 mm. Length are variables, determined by the length of the coupling lines.

-   **Parameters:** The four design parameters, including **w1, w2, l1 and l2** showing in the figure below are listed in the **1st-4th** column in the **"parameter"** matrix. **w_50** indicates the width of the 50 Ohms transmission line, which equals to **3.4 mm** in this case.

-   **Excitation:** Wave ports for both port 1 and port 2.

-   **Boundary conditions:** Open and add space boundaries in all directions.

-   **Solver:** Frequency Domain Solver in CST.                              

-   **Frequency:** 1 to 5 GHz, with a frequency spacing of 0.1GHz. 401 frequency points in total.

-   **Simulation tool:** All data are derived with the frequency domain solver
    in commercial simulation package CST MICROWAVE STUDIO.

-   **Result:** Real parts and imaginary parts of the S11, S21 responses of
    each phase shifter structure are included in the **“real_S11”, “imag_S11”** matrix and **“real_S21”, “imag_S21”** matrix, respectively.
    

<br/>
<br/>
<br/>
<br/>
<br/>

# Schiffman phase shifter dataset (dual section)
The input parameters, simulation environment and results are defined below:  

<img src="https://github.com/SensongAn/DNN-Schiffman-phase-shifter/blob/main/pics/2.jpg" width="50%">

-   **Substrate:** The phase shfiters are constructed based on the **Rogers R4003C** dielectric substrate, with the thickness of **1.524mm**, permittivity of **3.55** and loss tangent of **0.0027**. 

-   **Conductor:** **Copper (lossy, annealed)** for both microstrip circuits above the substrate and GND beneath.

-   **Substrate dimensions:** Width of all phase shifters are fixed to be 50 mm. Length are variables, determined by the length of the coupling lines.

-   **Parameters:** The four design parameters, including **w1, l1, w2, l2, l3, d1 and d2** showing in the figure below are listed in the **1st-7th** column in the **"parameter"** matrix. **w_50** indicates the width of the 50 Ohms transmission line, which equals to **3.4 mm** in this case.

-   **Excitation:** Wave ports for both port 1 and port 2.

-   **Boundary conditions:** Open and add space boundaries in all directions.

-   **Solver:** Frequency Domain Solver in CST.                              

-   **Frequency:** 1 to 5 GHz, with a frequency spacing of 0.1GHz. 401 frequency points in total.

-   **Simulation tool:** All data are derived with the frequency domain solver
    in commercial simulation package CST MICROWAVE STUDIO.

-   **Result:** Real parts and imaginary parts of the S11, S21 responses of
    each phase shifter structure are included in the **“real_S11”, “imag_S11”** matrix and **“real_S21”, “imag_S21”** matrix, respectively.
    

<br/>
<br/>
<br/>
<br/>
<br/>
    
    
    
# Schiffman phase shifter inverse design tool
A fast Schiffman phase shifter design tool enabled by DNN

Deploymentation of the well-trained Schiffman inverse design network model.
Environment prerequisites are as follows:
**1. Prerequisites for Deployment**

Verify that version 9.5 (R2018b) of the MATLAB Runtime is installed.   
If not, you can run the MATLAB Runtime installer.
To find its location, enter
  
    >>mcrinstaller
      
at the MATLAB prompt.
NOTE: You will need administrator rights to run the MATLAB Runtime installer. 

Alternatively, download and install the Windows version of the MATLAB Runtime for R2018b 
from the following link on the MathWorks website:

    http://www.mathworks.com/products/compiler/mcr/index.html
   
For more information about the MATLAB Runtime and the MATLAB Runtime installer, see 
"Distribute Applications" in the MATLAB Compiler documentation in the MathWorks Documentation Center.

**2. Files to Deploy and Package**

```diff
- Files to Package for Standalone
```
-main.exe (in "**./dataset/**" folder)

-MyAppInstaller.exe (in "**./dataset/**" folder)

    Note: if end users are unable to download the MATLAB Runtime using the
    instructions in the previous section, include it when building your 
    component by clicking the "Runtime included in package" link in the
    Deployment Tool.



**3. Definitions**

For information on deployment terminology, go to
http://www.mathworks.com/help and select MATLAB Compiler >
Getting Started > About Application Deployment >
Deployment Product Terms in the MathWorks Documentation
Center.



<img src="https://github.com/SensongAn/DNN-Schiffman-phase-shifter/blob/main/pics/Design_tool.png" width="60%">


