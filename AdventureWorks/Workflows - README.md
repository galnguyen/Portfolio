**Workflows**
**1. Extract - Transform - Load Data (ETL):**  <br>
<br>
   In the first stage, I loaded the data (Excel file) into Power BI and then transformed it to ensure all data fields were defined and formatted properly. I also checked the data quality and profile to ensure no errors within the dataset. <br>
   <br>
   Since the AdventureWorks dataset is clean, no further transformation is taken. Then I loaded all the tables into PBI.  <br>
   <br>
   ![image](https://github.com/galnguyen/Power-BI/assets/171650238/e460aa95-7ae0-4343-86b8-c7a3a46e3d43)  <br>
   <br>
**2. Data model:** <br><br>
    Firstly, I identified fact and dimension (dim) tables. In the original dataset, we can see 6 dim tables (for master data) and 1 fact table (for sales transaction data).  <br>
    <br>
    Secondly, I identified and set up the relationships among tables. The cardinality I use in this case is "One to many" for all relationships from the dim to the fact table (as each item is unique on a dim table and could appear in several rows in the fact table). For the relationship between the Date and Sales table, since there are 3 matches, I activated the most common one (DateKey - OrderDateKey).  <br>
    <br>
    ![image](https://github.com/galnguyen/Power-BI/assets/171650238/8e0eae73-5a90-4902-8604-e467974c5abb)  <br>
    <br>
    From the data model, I brainstormed the measures needed for my report. Since AdventureWorks is a completely new case with no specific insights yet, I chose to approach the dataset holistically. That means I would see the Sales data from every angle.  <br>
    <br>
   When it comes to DAX functions, I mainly used Basic Aggregations, Time Intelligence, SWITCH, CALCULATION with FILTER, IF, and ALL functions. The measures are grouped into 5 main categories: Index (main measures such as total quantity, total sales,…); Index_Benchmark (main measures with Time intelligence functions, for comparison purposes); Change (Variance between this period and a benchmarked one); Format (for formatting purpose), VMP/VMC (for variance analysis).  <br>
    <br>
**3. Visualization:**  <br>
<br>
  As I am the main audience (FP&A manager role, who detects issues and actionable insights) of this report, I created 4 dashboards: 1 overview (to quickly see if the trend goes as I expect, from various aspects) and 3 deep-dive analyses (focus on Product, Customer, Territory).  <br>
  <br>
  I sketched the dashboards I wanted to present before creating them to ensure all the visualizations were presented cohesively and coherently.  <br>
  <br>
  ![image](https://github.com/galnguyen/Power-BI/assets/171650238/178b875c-65e6-4107-8536-bba4bce8d7d7)  
  ![image](https://github.com/galnguyen/Power-BI/assets/171650238/95f3a1dc-99d5-400b-b9aa-ecba3688530e)  <br>
  ![image](https://github.com/galnguyen/Power-BI/assets/171650238/df00580b-3e45-4500-853c-3a108570f209) 
  ![image](https://github.com/galnguyen/Power-BI/assets/171650238/15d3e30f-9de4-4dda-9d6b-4a36ccc38daf) <br>
  <br>
**4. Insights and Recommendations are presented separately from this Note. Please visit my Wordpress blog to read further.** <br>
<br>
**5. Working files (available for download):**  <br>
  Data: https://github.com/galnguyen/Power-BI/blob/d8e4d21fb906763bb6a26b4ee2fafd7c8d563af9/AdventureWorks/AdventureWorks%20Sales.xlsx <br>
  Power BI file: https://github.com/galnguyen/Power-BI/blob/d8e4d21fb906763bb6a26b4ee2fafd7c8d563af9/AdventureWorks/AdventureWorks.pbix <br>
  <be>
  **END.**
  


