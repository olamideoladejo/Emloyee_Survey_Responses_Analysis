# Emloyee_Survey_Responses_Analysis
![cytonn-photography-n95VMLxqM2I-unsplash](https://github.com/user-attachments/assets/09312d13-216d-4727-bfc6-77d1ac2931a1)

### PROJECT OVERVIEW
The Employee Survey Responses are actual responses from an employee engagement survey conducted by Pierce County WA and completed voluntarily by government employees.
### DATA SOURCE
The data was provided by Digitaley Drive it consists of 10 columns (Response ID, Status, Department, Director, Manager, Supervisor, Staff, Question, Response, Response Text) and 14,725 rows
### DATA PREPARATION AND CLEANING
I loaded the data set in Power query in Power BI for transformation. I checked for null values and I noticed that the responses and response text columns had null values with corresponded with “incomplete” in the status column, I removed the null columns and also noticed that the Question column had 12 distinct values, which was supposed to be 10 unique values I found out question 7 had duplicate values (7. This last year, I have had opportunities at work to learn and grow an7. This last year, I have had opportunities at work to learn & grow) I replace the value “&” with “and” also found out Question 10 has duplicate values which were as a result of trailing white space, this was solved using the “TRIM” function in power query.
### Exploratory Data analysis
EDA involved exploring the survey data to answer key questions like
 Question 1. 
Which survey questions did respondents agree with or disagree with most? 
Question 2. 
Do you see any patterns or trends by department or role? 
Question 3. 
As an employer, what steps might you take to improve employee satisfaction based on the survey results? 
### Data analysis
Grouped the questions into 5  Categories using DAX.
- Job clarity
- Good work Environment and inclusivity
- Job Satisfaction
- Leadership and recognition
- Professional Growth

#### Measures Calculated
- Responses: Total Response by employees
- Agreement Percentage : Agreement rate to questions by employees
- Average Response: Average rating given to questions by employees
- Total Question: Number of Questions in the survey
- Department: Number of departments in the Organization
### Dashboard 
![Slide2](https://github.com/user-attachments/assets/da31a8b6-a3ea-4f28-a6b4-0b2ed78bc8b2)

### Key insights
###### Overview
- Total Responses: 14,575
- Agreement: 75% positive agreement
- Average Response: 3 out of 5
- Questions: 10 survey questions
- Departments: 21 departments
###### Questions Agreement Rate
- Question 1 “I know what is expected of me at work” was the most Agreed with (1341) responses while Question 6 “I have a best friend at work” was the most disagreed with (606) responses
###### Department Engagement
- Planning and Public Works department has the highest response rate (4.7K) while Family Justice Center shows lowest (39)
 ###### Role Participation
- Most of the responses were unspecified by roles , among the identified roles Supervisor had higher response and Manager had the lowest response.
###### Question theme
Job Clarity has highest Agreement rate (92.29%) which implies employees are informed about their roles, while Good Work Environment and Inclusivity has the  lowest (68.80%).
###### Recommendations
To improve Employee Satisfaction, the organization has to:
- Improve workplace environment and inclusion
- Enhance leadership development and employee recognition programs
- Organize training programs to strengthen career development
- Find out the root cause of low response rate in depatments and address concerns
- Encourage employees to specify their roles during surveys to improve analysis


