# WM_hackathon_x_Price_Elasticity_Model
This Repo comprises of the code and the methodology for calculating the price elasticity of provided sku 

This Model Comprises of Five modules to calcuate the optimal Price discount in percentage 


1. Base line Demand prediction 

Predict baseline demand (if no promos) and provide  early insights on  price vs. quantity  relationship.

2. Discount elasticity

Discount elasticity provide insights on which brands/SKUs are elastic and which ones are not.

3. Relative margin impact
Relative margin impact gives insights on whether brands get positive ROI from the deployed discounts.

4. Optimal discount scenario
Scenario planner analysis provide insights on optimal discounts for maximizing profit and sales

5. Substitutability
Substitutability analysis provide guidance on which pair of brands we should minimize having deep discounts at the same time.


Objective: Following SKUs are removed:

SKUs with very high test wmape: Caused due to some specific SKUs- can be looked into further but ignoring due to very few such SKUs
SKUs with negative or very high elasticity: Negative elasticity is counter-intuitive and could be due to stock-outs and would require inventory data going back 2-3 years to investigate (however currently we don't have such historical inventory data). Also removing few very high wmape SKUs
SKUs with avg. test period units very different from avg. train period units: Few SKUs have test period avg. units very different than train period avg. units, leading to high wmape
SKUs that have very high baseline vs. actual units: Remove such few SKUs as they skew the total baseline
