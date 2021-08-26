# DNN-Schiffman-phase-shifter
A fast Schiffman phase shifter design tool enabled by DNN
The input parameters, simulation environment and results are defined below:  

-   **Substrate:** The phase shfiters are constructed based on the Rogers R4003C dielectric substrate, with the thickness of 1.524mm, permittivity of 3.55 and loss tangent of 0.0027. 

-   **Conductor:** Copper (lossy, annealed) for both microstrip circuits above the substrate and GND beneath.

-   **Parameters:** The four design parameters, including w1, w2, l1 and l2 showing in the figure below are listed in the **1st-4th** column in the "parameter" matrix. w_50 indicates the width of the 50 Ohms transmission line, which equals to 3.4 mm in this case.

-   **Excitation:** Wave ports for both port 1 and port 2.

-   **Boundary conditions:** Open and add space boundaries in all directions.

-   **Solver:** Frequency Domain Solver in CST.                              

-   **Frequency:** 1 to 5 GHz, with a frequency spacing of 0.1GHz. 401 frequency points in total.

-   **Simulation tool:** All data are derived with the frequency domain solver
    in commercial simulation package CST MICROWAVE STUDIO.

-   **Result:** Real parts and imaginary parts of the S11, S21 responses of
    each phase shifter structure are included in the “real_S11”, “imag_S11” matrix and “real_S21”, “imag_S21” matrix, respectively.
    

    
