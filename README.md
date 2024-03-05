# Patients-Hospital-visits
![MasterHead](https://ichef.bbci.co.uk/news/976/cpsprodpb/17272/production/_122543849_gettyimages-1294582631.jpg)
<h1 align="center">Hi 👋, I'm Matthew Osadebamwen</h1>
<h3 align="center">A passionate Data Analyst and Data Scientist with crazy interest in Artificial Intelligence</h3> 
<img align="right" alt="Coding" width="400" src="https://imgvisuals.com/cdn/shop/products/animated-patient-flow-illustration-943688.gif?v=1697071141&width=1800"

<p align="left"> <img src="https://komarev.com/ghpvc/?username=matthew-osas&label=Profile%20views&color=0e75b6&style=flat"matthew-osas" /> </p>

- 🔭 In this project we're going to be working on **Analysing patients hospital visits**

<h3 align="left">Connect with me:</h3>
<p align="left">
<a href="https://linkedin.com/in/matthew-osadebamwen-ba4b26110" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="matthew-osadebamwen-ba4b26110" height="30" width="40" /></a>
</p>

<h3 align="left">Languages and Tools used for this project:</h3>
<p align="left"> <a 
href="https://www.microsoft.com/en-gb/microsoft-365/excel?ef_id=_k_CjwKCAiA_5WvBhBAEiwAZtCU78BaZH7BzevY2zQVGZOpfOOC2rf2_G0BTCbswPHNVSB2KuyHHY_2wRoCSGgQAvD_BwE_k_&OCID=AIDcmmp20rgnjr_SEM__k_CjwKCAiA_5WvBhBAEiwAZtCU78BaZH7BzevY2zQVGZOpfOOC2rf2_G0BTCbswPHNVSB2KuyHHY_2wRoCSGgQAvD_BwE_k_&gad_source=1&gclid=CjwKCAiA_5WvBhBAEiwAZtCU78BaZH7BzevY2zQVGZOpfOOC2rf2_G0BTCbswPHNVSB2KuyHHY_2wRoCSGgQAvD_BwE" target="_blank" rel="noreferrer"> <img src="https://techcommunity.microsoft.com/t5/image/serverpage/image-id/375416i783713B05CAD4A92/image-size/original?v=v2&px=-1" alt="Excel" width="40" height="40"/> </a> <a                                                                     href="https://www.microsoft.com/en-us/power-platform/products/power-bi" target="_blank" rel="noreferrer"> <img src="https://info.railsentinel.co.uk/wp-content/uploads/2023/02/PowerBI-Logo.png" alt="Power BI" width="40" height="40"/> </a> <a 
href="https://www.microsoft.com/en-us/sql-server" target="_blank" rel="noreferrer"> <img src="https://www.svgrepo.com/show/303229/microsoft-sql-server-logo.svg" alt="mssql" width="40" height="40"/> </a> <a href="https://www.mysql.com/" target="_blank" rel="noreferrer"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="mysql" width="40" height="40"/> </a> <a 

<p></p>

# Patients Hospital visits Analysis
For this analysis, we'll utilize the publicly accessible hospital patient visits dataset found on the internet
## <font color = red>**Introduction**</font>
The dataset under analysis consists of 9216 rows and 11 columns, each representing an individual patient encounter within a medical facility for the year 2019 and 2020. The dataset encompasses various demographic and clinical attributes associated with each patient hospital visit. Key attributes include the date and time of the visit, unique patient identifiers, demographic details such as gender, age, race, and satisfaction score. Additionally, administrative details such as patient administrative status, wait times, and department referrals are included.

This dataset presents an opportunity for comprehensive analysis to gain insights into patient demographics, clinical trends, administrative processes, and service utilization within the medical facility. By exploring these data points, healthcare professionals and administrators can potentially identify patterns, trends, and areas for improvement in patient care delivery, resource allocation, and operational efficiency. Furthermore, such analysis could inform decision-making processes aimed at enhancing the quality, accessibility, and effectiveness of healthcare services provided within the facility.



</head>
<body>

<h2>Patients Sample Dataset</h2>

<table>
  <tr>
    <th>Date</th>
    <th>Patient ID</th>
    <th>Patient Gender</th>
    <th>Patient Age</th>
    <th>Patient SAT Score</th>
    <th>Patient First Initial</th>
    <th>Patient Last Name</th>
    <th>Patient Race</th>
    <th>Patient Admin Flag</th>
    <th>Patient Wait Time</th>
    <th>Department Referral</th>
  </tr>
  <tr>
    <td>3/20/2020</td>
    <td>145-39-5406</td>
    <td>M</td>
    <td>69</td>
    <td>10</td>
    <td>H</td>
    <td>Glasspool</td>
    <td>White</td>
    <td>FALSE</td>
    <td>39</td>
    <td>None</td>
  </tr>
  <tr>
    <td>6/15/2020</td>
    <td>316-34-3057</td>
    <td>M</td>
    <td>4</td>
    <td>-</td>
    <td>X</td>
    <td>Methuen</td>
    <td>Native American/Alaska Native</td>
    <td>TRUE</td>
    <td>27</td>
    <td>None</td>
  </tr>
  <tr>
    <td>6/20/2020</td>
    <td>897-46-3852</td>
    <td>F</td>
    <td>56</td>
    <td>9</td>
    <td>P</td>
    <td>Schubuser</td>
    <td>African American</td>
    <td>TRUE</td>
    <td>55</td>
    <td>General Practice</td>
  </tr>
  <tr>
    <td>2/4/2020</td>
    <td>358-31-9711</td>
    <td>F</td>
    <td>24</td>
    <td>8</td>
    <td>U</td>
    <td>Titcombe</td>
    <td>Native American/Alaska Native</td>
    <td>TRUE</td>
    <td>31</td>
    <td>General Practice</td>
  </tr>
</table>


## <font color = red>**Aims**</font>

As an analyst within the healthcare industry, my objective is to derive insightful answers to the following questions using the provided dataset:
 
* <font color = green>What is the distribution of patient demographics within the dataset?</font> <br>
* <font color = green>What is the average wait time for patients before being seen by a healthcare provider? </font><br>
* <font color = green>Are there any patterns in department referrals based on patient demographics?</font> <br>
* <font color = green>Is there a correlation between patient satisfaction scores and wait times? </font><br>
* <font color = green>Are there any trends or patterns in patient admissions based on time of day or day of the week?</font><br>


</head>
<body>

<h1>To prepare and clean the patient's hospital visit dashboard, the following steps were followed:</h1>

<h2>Data Section:</h2>
<ul>
  <li>DAX Calculations for various metrics:</li>
  <ul>
    <li>Calculate % of visits by administrative staff</li>
      <p><img width="500" alt="1" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/962c9b84-05db-479c-b754-2b3724182b9e"></p>

    <li>Calculate % of visits without administrative staff</li>
    <li>Calculate % of female visits</li>
    <li>Calculate % of male visits</li>
    <li>Calculate % of visits with unknown gender</li>
    <li>Calculate % of visits with no rating</li>
    <li>Calculate % of referred patients</li>
    <li>Calculate % of unreferred patients</li>
    <li>Calculate average satisfaction score</li>
    <li>Calculate average waiting time</li>
    <li>Set up conditional formatting for maximum points by month and year</li>
    <li>Create a matrix caption for visits by race</li>
    <li>Determine total number of patients</li>
  </ul>
</ul>

<h2>Date Section:</h2>
<ul>
  <li>Create measures for date-related information:</li>
  <ul>
    <li>Define date</li>
    <li>Determine month</li>
    <li>Assign a number to each month</li>
    <li>Identify the day of the week</li>
    <li>Categorize weeks as "Weekend" or "Weekday"</li>
    <li>Determine the year</li>
  </ul>
</ul>

<h2>Parameter Section:</h2>
<ul>
  <li>Set up a slicer to interact with the table:</li>
  <ul>
    <li>Enable filtering by average satisfaction score</li>
    <li>Enable filtering by average waiting time</li>
  </ul>
</ul>

<h2>Dataset:</h2>
<ul>
  <li>Add additional columns for better analysis:</li>
  <ul>
    <li>Determine if the visit occurred in the morning or afternoon (Time of Day)</li>
    <li>Group patients into age categories (e.g., Infant, Young Child, Child, Teenager, Adult)</li>
    <li>Merge columns to create a unified name column for patient identification</li>
  </ul>
</ul>

<h2>Visualization Section:</h2>
<ul>
  <li>Utilize various Power BI visualizations (e.g., bar charts, line graphs, matrices) to present the data effectively.</li>
  <li>Design a dashboard layout that includes all relevant metrics and allows for easy interpretation.</li>
  <li>Apply appropriate colors and formatting to enhance visual appeal and readability.</li>
  <li>Test the dashboard to ensure that slicers and filters function correctly and that data updates accurately.</li>
</ul>

</body>
</html>
