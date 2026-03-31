# **Column descriptions**

### **Identification and organization**

1. **Job ID** — unique identifier of the job posting.  
    Number of unique values: 1400\.  
2. **Agency** — city agency or department that posted the vacancy.    
   Number of unique values: 56\.  
3. **Posting Type** — whether the posting is for internal or external candidates.  
4. **\# Of Positions** — number of open positions for the posting

## **Job title and classification**

5. **Business Title** — public-facing job title shown in the vacancy.    
Number of unique values: 1097\.
6. **Civil Service Title** — standardized official title in the NYC civil service system.\
Number of unique values: 295\.
8. **Title Classification** — administrative classification of the title.  
Unique values: 'Non-Competitive-5', 'Competitive-1', 'Exempt-4',   'Pending Classification-2', 'Labor-3'. 
9. **Title Code No** — code assigned to the civil service title.  
   Number of unique values: 307\.  
10. **Level** — internal assignment or classification level for the title.  
   Number of unique values: 16\.  
11. **Career Level** — general seniority or experience level of the position.  
    Unique values: 'Student',   'Entry-Level', 'Experienced (non-manager)', 'Manager',  'Executive'.

### **Job content**

11. **Job Category** — category or functional area of the job.  
    Number of unique values: 98\.  
12. **Job Description** — summary of the responsibilities and duties.  
13. **Minimum Qual Requirements** — minimum qualifications required for the job.  
    Number of unique values: 624\.  
14. **Preferred Skills** — additional preferred skills beyond the minimum requirements.  
15. **Additional Information** — extra details related to the posting.  
16. **To Apply** — instructions for submitting an application.  
17. **Hours/Shift** — shift or working hours information.  
18. **Division/Work Unit** — division, office, or work unit within the agency.  
    Number of unique values: 624\.

### **Employment and salary**

19. **Full-Time/Part-Time indicator** — whether the position is full-time or part-time.  
20. **Salary Range From** — lower bound of the salary range.  
21. **Salary Range To** — upper bound of the salary range.  
22. **Salary Frequency** — salary unit.  
    Unique values: annual, daily, hourly.

### **Location**

23. **Work Location** — work location in text form.  
24. **Work Location 1** — additional location field, often similar or duplicate of Work Location.  
25. **Residency Requirement** — whether residency requirements apply.

### **Dates**

26. **Posting Date** — date when the vacancy was posted.
27. **Post Until** — closing date or deadline for the posting.
28. **Posting Updated** — date when the posting was last updated.
29. **Process Date** — technical processing date in the dataset.

### **Administrative**

30. **Recruitment Contact** — contact field for recruitment purposes

## **Columns Removed from the Dataset**

To improve the quality and clarity of the analysis, some columns were removed from the dataset during the data cleaning stage. These fields were excluded because they were either administrative, redundant, highly unstructured, contained too many missing values, or were not relevant to the goals of the current analysis.

The analysis mainly focused on job postings, salary trends, hiring demand, and job categories, key skills. Therefore, only the variables that directly supported these objectives were retained.

### **Removed Columns and Justification**

**Title Classification**  
 This column was removed because it represents an internal administrative classification of job titles. It did not provide meaningful value for analyzing salary patterns, hiring trends, or job categories.

**Title Code No**  
 This field was excluded because it is a technical identifier used for internal classification purposes. While useful in administrative systems, it is not informative for the current analytical objectives.

**Level**  
 This column was dropped because it reflects an internal assignment or classification level whose meaning is not sufficiently clear or relevant for the scope of this analysis.

**Work Location**  
 This field was removed because location was not a primary focus of the study. In addition, the values were not standardized enough to support consistent geographic analysis.

**Work Location 1**  
 This column was excluded because it appeared to duplicate or overlap with other location-related information and did not add distinct analytical value.

**Division/Work Unit**  
 This field was removed because it contains very specific internal organizational details that were not necessary for analyzing broader job market patterns.

**Job Description**  
 This column was dropped because it is a large unstructured text field. Although it may be useful for separate text-mining tasks, it was not required for the current structured analysis.

**Additional Information**  
 This field was removed due to its high percentage of missing values and limited relevance to the main research questions.

**To Apply**  
 This column was excluded because it mainly contains application instructions rather than job-related characteristics useful for analysis.

**Hours/Shift**  
 This field was removed because it contained a large amount of missing data and was not essential to the objectives of the study.

**Recruitment Contact**  
 This column was dropped because it contained no values and therefore had no analytical value.

**Post Until**  
 This field was removed because it was not essential to the current analysis. Since the study focused on job characteristics, salary trends, and hiring patterns rather than vacancy closing periods, this column did not provide significant analytical value.

**Process Date**  
 This field was removed because it represents a technical processing timestamp rather than a meaningful variable related to the job posting itself.

