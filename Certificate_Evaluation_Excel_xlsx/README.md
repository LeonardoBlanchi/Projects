# Certificate Evaluation – Excel Workbook

## Certificate_Evaluation_Excel.xlsx
Excel workbook prepared for the **Certificate Evaluation** course assignment. It contains the input data and the main calculations used to **price/evaluate the Commerzbank Top Return Certificate (30/04/2014–28/04/2018)** linked to the **Commerzbank Top Return Index** (basket of 6 funds with a target-volatility mechanism).

### Main sheets
- **Quotations / Q2**: historical prices/NAVs of the 6 underlying funds  
- **IR / SR**: historical **EURIBOR (1/3/6/12M)** and **EUR swap rates (2/3/5Y vs 6M)** used to build the interest-rate curve  
- **Index**: index reconstruction (basket aggregation, weights/target-volatility logic)  
- **BS_Valuation**: certificate valuation (Black–Scholes–style approach) at issue date and end-of-month dates
