# Price_Transparency_Analysis

## Group 6 

### Hospital Price Transparency for top 20 US News and World Report Hospitals
How do we use and better understand pricing in healthcare and how it relates to quality.  It's important for our employer to understand this.  There has been lots of interest for a deep analysis but only few have been done.

### The data source used will be the published price transparency files from each hospital website.
  - Diagnostic related groups (DRGs)
  - Subset of payers (Blue Cross Blues Shield, United Health Care, Cigna, Health Partners, Aetna)

### Group hypothesis:  
   - Large difference between pricing among hospitals
   - Predict higher quality will have a higher price
   - Price consistency among payer groups
   - Payers have different contract rates
   - Payers consistently found in data will have greater variation in reimbursements
   - Hospitals in larger metropolitan areas will have higher prices
   
### Our analytic approach will be descriptive statistics, a linear regression, clustering, and decision trees.  We will remain flexible and see where the data takes us.

#### Beginning Statistics from Combined File.

Group by payer

![image](https://user-images.githubusercontent.com/90878901/155637816-59822b87-4be5-4830-9fa3-f3bda1b7eea2.png)

Group by DRG

![image](https://user-images.githubusercontent.com/90878901/155637857-711318e4-e9b4-411b-ba87-f6fddd4cb965.png)

Overall summary

![image](https://user-images.githubusercontent.com/90878901/155637890-a0645730-2d8c-46a0-af31-d0945be9ebcb.png)

Row count

![image](https://user-images.githubusercontent.com/90878901/155637925-b1df437c-7f43-407d-a3a0-6c89d6862b4c.png)

DRG file 

![image](https://user-images.githubusercontent.com/90878901/155638164-a48eeeaf-8832-49f4-88c1-7a550e0ca65a.png)

### Clustering by Payor
![Scatter_plot_Capture](https://user-images.githubusercontent.com/90974647/155854783-b309e81f-bb85-4e4c-9d12-1615d05b198e.PNG)


#### Sample Mapping

![image](https://user-images.githubusercontent.com/90878901/154609988-b2765087-327c-46e4-94ab-a54a24c043b4.png)

![image](https://user-images.githubusercontent.com/90878901/154609998-0acbf984-8d91-4703-a461-3047a78f17aa.png)

![image](https://user-images.githubusercontent.com/90878901/154610020-780bf6db-b0c0-48ec-ace0-d218506b0b8d.png)
