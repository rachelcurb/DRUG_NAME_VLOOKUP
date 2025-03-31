# DRUG_NAME_VLOOKUP

## Welcome! ##

The purpose of this page is to quickly demonstrate my capabilites in Excel, specifically in using the VLOOKUP function. Because using actual patient information is a HIPAA violation, data used in the Excel workbook was generated from `mostly.ai`.

*The raw Excel and .csv files as well as the end result can be downloaded and viewed on this page.*

### Prompt: ###
A pharmacy obtained a list of names of patients who were prescibed pain management drugs but only had their drug IDs. The pharmacy needs to extract the name of the drug prescribed and its price by only using information from the table below:

![image](https://github.com/user-attachments/assets/8ad8a845-157c-44f8-941a-64cc895fcc37)

### Methodology: ###
The VLOOKUP function was used to list the drug name and price by only have a list of patient names and their drug ID. The first 10 patients are listed below:

![image](https://github.com/user-attachments/assets/6b60ec9b-5fa7-4874-84e9-92b3c0e759e2)

By using this formula,
`=VLOOKUP(G2,vlookup_unique_generic_drugs_wh!$A$1:$C$11,2,FALSE`, the name of the drug automatically populated the adjacent column.

This formula was used to populate the price of the drug: `=VLOOKUP(G2,vlookup_unique_generic_drugs_wh!$A$1:$C$11,3,FALSE)`

After building the formula, it can be duplicated to the rest of the column by dragging down the + cursor on the bottom right of the cell.

### Result: ###

![image](https://github.com/user-attachments/assets/44a6123a-a563-4447-a58b-856d7ee70c62)
