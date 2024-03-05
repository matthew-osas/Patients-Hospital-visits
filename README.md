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
    <li> Calculate % of visits by administrative staff<img width="500" alt="1" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/962c9b84-05db-479c-b754-2b3724182b9e"></li>
    <li>Calculate % of visits without administrative staff</li>
    <li>Calculate % of female visits</li>
    <li>Calculate % of male visits</li>
    <li>Calculate % of visits with unknown gender<img width="500" alt="2" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/f4f6f2a8-9304-4ae1-92b6-8a2e382eb666">
</li>
    <li>Calculate % of visits with no rating</li>
    <li>Calculate % of referred patients</li>
    <li>Calculate % of unreferred patients</li>
    <li>Calculate average satisfaction score<img width="500" alt="3" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/df1fc3ac-87d4-4ce7-ba26-f4638e737db0">
</li>
    <li>Calculate average waiting time</li>
    <li>Set up conditional formatting for maximum points by month and year</li>
    <li>Create a matrix caption for visits by race</li>
    <li>Determine total number of patients<img width="500" alt="4" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/755ca51e-aec5-4c7a-b2bf-69050a9f1168">
</li>
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
    <li>Categorize weeks as "Weekend" or "Weekday"<img width="500" alt="1" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/0eaa8c75-6fea-4b5e-871f-9a3b461de9f9"></li>
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
    <li>Group patients into age categories (e.g., Infant, Young Child, Child, Teenager, Adult)<img width="500" alt="1" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/fae0cdf3-9d48-4b42-af5f-835cd2b794e4">
</li>
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

<h3>Report Snapshot (Power BI Desktop):</h3><a href="https://app.powerbi.com/view?r=eyJrIjoiNjRlNmMwZjktM2MxMC00OWE1LThmMDItYmUyYTFhNzQ4Yjc2IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9">Dashboard Report For Patients Hospital visits</a><img width="800" alt="1" src="https://github.com/matthew-osas/Patients-Hospital-visits/assets/102475461/5d050df9-6122-4133-a15a-c22608be0793">

## <font color = red>**Insights obtained from analysis**</font>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

</head>
<body>

<p class="red-text"><strong>Question (A):</strong> What is the distribution of patient demographics within the dataset?</p>
<p><strong>Answer:</strong> From this data, we can draw some preliminary conclusions about the distribution of patient demographics:</p>
<ul>
  <li>There were a total of 9216 patients visiting the hospital.</li>
  <li>The number of visits during the day (AM) was slightly higher than at night (PM), with 4632 visits during the day and 4584 visits at night.</li>
  <li>More visits occurred on weekdays (6574) compared to weekends (2642), indicating that the hospital receives a higher number of patients on weekdays.</li>
  <li>Referred patients account for approximately 41.41% of the total visits, while unreferred patients account for approximately 58.59%.</li>
  <li>The facility receives 7106 visits from adult patients, followed by children with 719 visits, teenagers with 697 visits, and the least visits are from infants with 226 visits.</li>
</ul>

<p class="red-text"><strong>Question (B):</strong> What is the average wait time for patients before being seen by a healthcare provider?</p>
<p><strong>Answer:</strong> Based on the race and age group matrix distribution, it can be inferred that the average wait time is heavily influenced by the severity of the patient's condition. For example, there appears to be less wait time for patients suffering from cardio-related conditions compared to patients with general conditions.</p>

<p class="red-text"><strong>Question (C):</strong> Are there any patterns in department referrals based on patient demographics?</p>
<p><strong>Answer:</strong> Based on the bar chart, it can be deduced that the hospital receives a higher number of unreferred patients, followed by patients referred to the general practice department, then orthopedics. The renal department has the least number of hospital visits. This trend appears to be consistent regardless of patients' age, gender, or hospital status (whether they are hospital staff or not).</p>

<p class="red-text"><strong>Question (D):</strong> Are there any patterns in department referrals based on patient demographics?</p>
<p><strong>Answer:</strong> The analysis reveals that more than 75% of the patients visiting the hospital do not provide any rating for the services they received. Therefore, it is challenging to accurately investigate whether there is a correlation between average satisfaction time and average wait time.</p>

<p class="red-text"><strong>Question (E):</strong> Are there any trends or patterns in patient admissions based on time of day or day of the week? </p>
<p><strong>Answer:</strong> The hospital receives more visits during the weekdays, with 6574 visits compared to 2642 visits on weekends. Of the weekend visits, 48.7% are male, 51.1% are female, and 0.3% are of unknown gender. This trend appears to be consistent regardless of age class (adult, teenage, child, young child, and infant), age group (0-10, 11-20, 20-30,...), and time of day (AM or PM). </p>
</ul>
</body>

<title>Recommendations for Improving Healthcare Services</title>
</head>
<body>

<h2>Recommendations for Improving Healthcare Services:</h2>

<ol>
  <li>
    <h3>Improve Access to Healthcare Services:</h3>
    <p>Increase availability of healthcare services during weekdays to accommodate the higher number of visits observed during this time period.</p>
    <p>Consider extending clinic hours during weekends to provide better access to care for patients who are unable to visit during weekdays.</p>
  </li>
  <li>
    <h3>Enhance Patient Education and Prevention Programs:</h3>
    <p>Develop educational campaigns targeting specific demographics, such as parents of infants and teenagers, to raise awareness about preventive healthcare measures and reduce the likelihood of hospital visits.</p>
  </li>
  <li>
    <h3>Strengthen Referral Processes:</h3>
    <p>Implement a streamlined referral process to ensure patients are referred to the appropriate department promptly, reducing unnecessary visits and improving patient outcomes.</p>
  </li>
  <li>
    <h3>Improve Patient Experience and Engagement:</h3>
    <p>(a) Implement initiatives to collect patient feedback and ratings more effectively, such as using mobile apps or automated surveys, to gain insights into patient satisfaction and areas for improvement.</p>
    <p>(b) Enhance communication channels between patients and healthcare providers to address concerns and provide support throughout the healthcare journey, leading to increased satisfaction and reduced hospital visits.</p>
  </li>
  <li>
    <h3>Optimize Appointment Scheduling and Wait Times:</h3>
    <p>Implement strategies such as telehealth services or virtual consultations to provide timely access to healthcare professionals, reducing the need for in-person visits and improving overall patient satisfaction.</p>
  </li>
</ol>

<p>By implementing these recommendations, the hospital can effectively reduce the number of hospital visits by patients and increase patient satisfaction, ultimately improving patient outcomes and optimizing healthcare delivery.</p>

</body>




