# GEP_for_BCSIS
Generation Expansion Planning Toward the Decarbonization of the Baja California Sur Electrical System

The input data files for the PLEXOS Software are located in the “Input Data To PLEXOS” folder, where data from 2025 to 2039 are detailed:
   •	Build Cost.
   •	Fuel-Price.
   •	Rating Factor.
   •	Load.
   •	Load Participation Factor.
   •	CSP Max Energy Day (50MW).
   •	CSP Max Energy Day (75MW).
   •	CSP Max Energy Day (100MW).

It is important to note that the data are imported as .csv files, as the processing of hourly, daily, monthly, and annual datasets is streamlined through the creation of Data Files within the PLEXOS interface.

To ensure that the data are correctly recognized by the PLEXOS interface, follow the steps below:
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
