# GEP_for_BCSIS

March, 2026

Generation Expansion Planning Toward the Decarbonization of the Baja California Sur Electrical System

Submission ID: 10343

IEEE Latin America Transactions

Authors: Antonino López Ríos, Gilberto López Ríos, Pablo Moreno Villalobos, and Mario R. Arrieta-Paternina

We provide the dataset for implementing the Generation Expansion Planning (GEP) to achieve the decarbonization of the Baja California Sur Interconnected System (BCSIS). We optimally solve three scenarios and a reference case using CPLEX and Gurobi algorithms embedded in PLEXOS®. Results for all scenarios are summarized in the file named  "Comparisons.pdf"

The input dataset files for the PLEXOS Software are located in the “Input Data To PLEXOS” folder, where data from 2025 to 2039 are detailed:

   •	Build Cost. 
   
   •	Fuel-Price.
   
   •	Rating Factor.
   
   •	Load.
   
   •	Load Participation Factor.
   
   •	CSP Max Energy Day (50MW).
   
   •	CSP Max Energy Day (75MW).
   
   •	CSP Max Energy Day (100MW).
   
   

It is important to note that the data are imported as .csv files, as the hourly, daily, monthly, and annual data processing is streamlined through the creation of Data Files within the PLEXOS interface.

To ensure that the dataset is correctly recognized by the PLEXOS interface, follow the steps below:

•  In the PLEXOS navigation panel, go to:

     system → Data Files
     
•  Right‑click on the Data Files folder and select:

     New Data File
     
•  In the window that appears, assign a name to the Data File, using the same naming convention as the elements listed in the model (for example: Load, Fuel Price, CSP Max Energy Day, etc.).

•  Once the Data File has been created, select it and, in the Filename field, specify the corresponding .csv file.

      Example:
      
              Data File: Fixed Charge
              
              Filename: Fixed Charge.csv
              
These steps allow PLEXOS to correctly locate and read the .csv files when the model is executed.



The “Input Data To TSL” folder contains the files needed to calculate the hourly capacity factors (Rating Factor) for renewable power plants. These files include:

   •  TSLData.csv
   
      Contains the installed capacity (MW) of each renewable unit and its geographic location.

  •  hcfobs.csv
  
      Provides a 24×12 generation profile (24 hours × 12 months) with estimated production for Existing and Candidate units included in the optimization process

