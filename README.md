## PATIENT EMERGENCY ROOM VISIT DASHBOARD
Have you ever rushed to an emergency room, only to encounter a long wait for treatment? This Power BI dashboard visualizes key metrics from emergency department patient admissions data, offering insights into average wait times, patient satisfaction, and referral trends. This analysis aims to help both patients and healthcare providers better understand the dynamics of emergency care, identify areas for improvement, and enhance the overall patient experience in the ER.

### Key Findings
1. Patient Satisfaction: The majority of patients reported being less than moderately satisfied with their experience.
2. Average Wait Time: The average wait time before being seen was 35.26 minutes.
3. Peak Wait Times: Wait times peaked on Mondays at 11 PM and were shortest on Wednesdays at 1 AM.
4. Referral Trends: The most frequent referral from the ER was to General Practice, followed by Orthopedics.

### The Data
This dataset comes from Real World Fake Data, representing a simulated hospital ER with 9,216 entries. Each entry corresponds to a patient and includes the following attributes:
https://data.world/markbradbourne/rwfd-real-world-fake-data
1. date: Day and time
2. patient_id: Patient Code
3. patient_gender: Gender (Male, Female, NC)
4. patient_age: Patient’s age
5. patient_sat_score: Patient satisfaction score
6. patient_first_initial: Patient’s first name initial (for privacy)
7. patient_last_name: Patient’s last name
8. patient_race: Patient’s race
9. patient_admin_flag: “Unknown explanation" (excluded from analysis)
10. patient_waittime: Patient’s ER wait time
11. department_referral: Department that the patient was referred to (e.g., General Practice, Orthopedics)

    
### Visualizations
### Total Number of Patients
Use the patient_id field and apply the Count function to obtain the overall count of patients entering the emergency room. The expected result should be 9,216.

### % of Patients by Gender
A pie chart represents the distribution of patients by gender. Use the patient_id for counting and the patient_gender field to calculate percentages.

### Patient Average Satisfaction
Create a line chart with the date in the columns and the average patient_sat_score in the rows, formatted to reflect the month and year.

### Patient Average Wait Time
Duplicate the sheet used for satisfaction to create another for patient_waittime, displaying the average wait time in minutes.

### Patients by Age Group
Generate age groups using a calculated field, resulting in three categories: 0–18, 19–65, and 66+.

### Average Wait Time by Day and Hour
Create a heatmap using the date converted to weekdays for columns and hours for rows, utilizing average wait time as the metric.

### Patients by Race
Construct a bar graph with patient_id counts in columns and patient_race in rows, adding a gradient color effect.

### Patients by Department Referral
Duplicate the patients by race visualization, substituting patient_race with department_referral.

### Dashboard Access
The interactive dashboard is available for viewing on Power BI.

### Insights
1. Patient Satisfaction
The average satisfaction score among patients in this emergency department was just 4.99 out of 10. Most patients had a negative experience, with the highest score in March (5.327) and the lowest in April (4.627).

2. Average Wait Times
Monthly averages for wait times showed minimal variation, with a maximum of 36.67 minutes in February and a minimum of 34.27 minutes in September.

3. Longest and Shortest Wait Times
The longest waits occurred on Monday nights at 11 PM (average of 40.69 minutes), while the shortest were on Wednesdays at 1 AM (average of 29.65 minutes).

4. Department Referrals
General Practice tops the list of ER referrals, often for conditions that could be addressed by a primary care physician, with Orthopedics being the second most common referral.

### Takeaways
Understanding these metrics can help patients make informed decisions about where to seek care and assist hospital leadership in implementing necessary improvements. The data clearly indicates that changes are essential to enhance patient care in this ER.

### Conclusion
Thank you for reading! I look forward to conducting more real-time analyses of healthcare data to promote data-driven decision-making. If this interests you, feel free to follow along for more updates!





![Healthcare pic](https://github.com/user-attachments/assets/bef2e526-8295-432f-9a71-de81246b5b68)
