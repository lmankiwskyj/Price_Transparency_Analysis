# Price_Transparency_Analysis

## Group 6 

### Hospital Price Transparency for top 20 US News and World Report (USNWR) Hospitals
How do we use and better understand pricing in healthcare and how it relates to quality?  Current federal price transparency requirements for US hospitals does not require reporting on quality alongside price.  It is assumed that transparency regarding healthcare cost and quality will provide consumers with the necessary information to make more informed decisions.  Advocates of price transparency argue that it will lower consumer health costs by increasing competition among providers and giving patients the option of “shopping” for the best price.  As of January 1, 2021, each hospital operating in the United States was required to provide clear, accessible pricing information online about the items and services they provide.

#### Project hypothesizes:  
   - There will be a large difference between pricing among hospitals
   - Higher quality will have a higher price
   - There will be price consistency among payer groups
   - Payers will have different contract rates
   - There will be price variation among payers in diagnostic related group (DRG) reimbursements
   - Hospitals in larger metropolitan areas will have higher prices
The data source used will be the published price transparency files from each hospital website for the top 20 ranked USNWR hospitals, including DRGs, payers, and USNWR quality ranking.  Our focus wis limited to payers:  Blue Cross Blues Shield, United Health Care, Cigna, Health Partners, and Aetna.  The file types collected were csv, text, and Json and all needed substantial reformatting and cleaning for our analysis.

## Methods
Cleaning and compiling methods included:
-	Python
-	Tableau Prep
 ![Capture_Tableau](https://user-images.githubusercontent.com/90974647/156897201-b7b47b63-0ed2-49aa-8452-cf9ee503a2db.JPG)

-	Alteryx 
 ![MicrosoftTeams-image](https://user-images.githubusercontent.com/90974647/156897202-9d0fc478-2de4-4d0a-9b16-5aec67e7bc2c.png)
 
#### Beginning Statistics from Combined File
Group by payer

![image](https://user-images.githubusercontent.com/90878901/155637816-59822b87-4be5-4830-9fa3-f3bda1b7eea2.png)

Group by DRG

![image](https://user-images.githubusercontent.com/90878901/155637857-711318e4-e9b4-411b-ba87-f6fddd4cb965.png)

Overall summary

![image](https://user-images.githubusercontent.com/90878901/155637890-a0645730-2d8c-46a0-af31-d0945be9ebcb.png)

Complied Dataframe

![image](https://user-images.githubusercontent.com/90878901/155638164-a48eeeaf-8832-49f4-88c1-7a550e0ca65a.png)
 
#### Machine Learning
Our initial attempts to work with entire data using Python K-means and PCA were thrown out.  The file size was difficult to work with and the results were not as expected.  

3D Plot

![image](https://user-images.githubusercontent.com/90878901/156100598-5d89bd9a-f427-407a-b336-9905fc8e613a.png)

Elbow Curve

![image](https://user-images.githubusercontent.com/90878901/156100543-32e47d98-3d5b-44e2-8e44-651ddac3e1f7.png)

Clustering by Payor

![Scatter_plot_Capture](https://user-images.githubusercontent.com/90974647/155854783-b309e81f-bb85-4e4c-9d12-1615d05b198e.PNG)

Changing our focus to one subspecialty (cardiology) and using Pearson’s coefficient of correlation resulted the following correlation matrix:

![Capture_corr_matrix](https://user-images.githubusercontent.com/90974647/156897516-0a08b201-355d-49a3-ab32-a28415dbd4b6.PNG)

## Results
The Pearson coefficient values did not show any strong correlations between price (charge amount) and the different quality rankings.  

### Visualization with Tableau 
--->Insert link to dashboard

Northeastern Hospital Map - Per Capita

![image](https://user-images.githubusercontent.com/90878901/156901802-c8265a45-d5d0-4377-9dc8-815c1f05b9b8.png)

Northeastern Hospital Map - Owner Occupied Housing Value

![image](https://user-images.githubusercontent.com/90878901/156901946-3a029610-abcd-476b-8a92-a8b281e0c8e8.png)

Midwest Hospital Map - Per Capita

![image](https://user-images.githubusercontent.com/90878901/156901859-3efcb2fc-40ab-42e8-a270-2b5742ee4b79.png)

Midwest Hospital Map - Owner Occupied Housing Value

![image](https://user-images.githubusercontent.com/90878901/156902197-cc9df390-5502-4b01-a92b-8bd54e2bfb53.png)

Western Hospital Map - Per Capita

![image](https://user-images.githubusercontent.com/90878901/156901874-dd678479-fd52-4c87-893d-558c97e1a726.png)

Western Hospital Map - Owner Occupied Housing Value

![image](https://user-images.githubusercontent.com/90878901/156902184-6b7b0c09-1c16-440d-a512-e30638852838.png)

### Hospital Location Results
The Top 20 US News and World Report Hospitals reside in the counties, with the highest 2018 per capita income. Additionally those hospitals reside in the highest owner occupied median housing value.

## Conclusion   
There was mixed compliance with the federal rule requiring hospitals to publicize their negotiated prices with all contracted insurers, many hospitals reporting information that was incomplete, and difficult to find or interpret. There was widespread variation in prices across services, payer, and hospitals and no apparent correlation between quality rankings and price.  Mayo Clinic, the #1 rated hospital, was notably lower in their published prices.  There is a correlation between metropolitan areas and pricing, as the highest average prices were found in large metropolitan cities.

Price transparency has a way to go, to be of value to individual consumers.  Perhaps the most valuable result of these transparency regulations will be the availability of data to health policy researchers, who can use it to develop more powerful strategies to contain US health care costs.  More to come on this as insurance companies are expected to release their pricing information in July of 2022.

Recommendations for future analysis. This analysis was limited to DRGs, which limits the amount of data available. A future analysis could include pharmacy and hospital chargemaster from the machine readable files. These charges are very important in the industry. There could be an expansion of hospitals, especially hospitals in low per capita and low owner occupied median housing value. In this type of analysis a comparison of hospital median charges could be compared between high and low per capita. With a larger data set we could apply additional machine learning. Centers for Medicare and Medicaid are requiring insurance companies to post their files similar to hospitals. This information could be used to quality compare the hospital posted machine files. 

Changes that we could have made would have been reducing the data set further and expanding the quality metrics beyond the data found from US News and creation of our own quality score to judge the hospitals. We could expand our data and use both US News and World report as well as detail statistics from Newsweek. 
 

