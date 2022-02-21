# Bank-Marketing-Data-Analysis

Background

The data is related to direct marketing campaigns (phone calls) of a Portuguese banking institution. 
The classification goal is to predict if the client will subscribe to a term deposit (variable y).

 <img src="https://user-images.githubusercontent.com/99994988/154992225-2cfc4340-e7d8-4be5-8339-ff2d02447294.png" width="500" height="400" align="centre">


Handling Missing Values:

<img src="https://user-images.githubusercontent.com/99994988/154992808-7c995cb0-c616-4d8c-a44b-e391f03a726b.png" width="500" height="400" align="centre">


Exploring variables:


<img src="https://user-images.githubusercontent.com/99994988/154993076-698616ab-3fef-4c12-95db-9c7bf265001d.png" width="500" height="400" align="centre">


Chi-Square Test:  (752.2712305309708, 4.4970126314001315e-148, 18)
The P Value is less than 0.05, that indicates “JOB” is a significant variable to predict “y”.  

Conversion per month:

<img src="https://user-images.githubusercontent.com/99994988/154993457-68cf0eb0-6773-43a1-abe8-56bb167c7dc9.png" width="500" height="400" align="centret">

Maximum Conversion is in the month of Mar and Dec.

Conversion per day:

<img src="https://user-images.githubusercontent.com/99994988/154993782-5eed65e4-3876-4725-a962-7a833e40841e.png" width="500" height="400" align="centre">

Age and Duration:

<img src="https://user-images.githubusercontent.com/99994988/154993935-330677c4-8aa0-485f-87e7-d92d11329368.png" width="500" height="400" align="centre">

P Value as per Anova is less that 0.05, which indicates both “age” and  “duration” are statistically significant variables in the prediction of “y”. 


Campaign:

<img src="https://user-images.githubusercontent.com/99994988/154994172-ed7806d2-e2d4-4954-b186-b474e89bc630.png" width="500" height="400" align="centre">

P Value as per Anova is less that 0.05 for Campaign, which indicates “campaign” is a significant variables in the prediction of “y”. 
There 31724 out of 32950 are “999” which means the client was not at all contacted before. 
Therefore, due to insufficient data, “pdays” is not a significant variable for this prediction.

Pdays:

<img src="https://user-images.githubusercontent.com/99994988/154996639-bda8143f-62d9-41e9-a7ff-f36cb633ed6f.png" width="500" height="400" align="centre">

63.62% of the clients subscribed who were contacted during the previous campaign

9.24% of  the clients subscribed who were “not” contacted during the previous campaign

Chi-Square Test: (3491.770854457325, 0.0, 2) 
The P Value is less than 0.05, that indicates “pdays” is a significant variable to predict “y”.  

Dropping Insignificant variables:

Housing
Day of week
Loan

Encoding:

1. Label encoding for target variable
2. Ordinal Encoding for the variables  “education” and “job”, as the order is important
3. One Hot Encoding for “marital”,”contact”,”month” and “pdays”
4. Binarizer for “default” and “poutcome”

<img src="https://user-images.githubusercontent.com/99994988/154998181-c5e40b91-7dc8-4e31-9127-4b1e80b5d32d.png" width="500" height="400" align="centre">
