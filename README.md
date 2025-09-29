# HR-Employee-Attrition-analysis
This dataset tells about the employees age, jobs, salaries, satisfaction, and performance — and whether they leave or stay.
                               DATA UNDERSTANDING

This dataset tells about the employees age, jobs, salaries, satisfaction, and performance — and whether they leave or stay.

Attrition → Shows whether an employee left (Yes) or stayed (No)

Age → Employee age.

Gender → Male or Female.

MaritalStatus → Married, Single, or Divorced.

EmployeeNumber → Unique ID for each employee.

EmployeeCount → Always “1” (not useful).

Over18 → All values are “Y” (not useful).

StandardHours → All values are “80”

Department → Department of work (e.g., Sales, Research & Development, HR).

JobRole → Job title (e.g., Sales Executive, Research Scientist, Manager).

JobLevel → Level of the employee in the organization hierarchy (1 = entry-level, higher = senior).

BusinessTravel → Frequency of travel (Non-Travel, Travel_Rarely, Travel_Frequently).

DistanceFromHome → Distance (in kilometers/miles) from employee’s home to office.

EnvironmentSatisfaction → Self-reported satisfaction with work environment (1–Low, 2–Medium, 3–High, 4–Very High).

JobInvolvement → Engagement in job (1–Low, 4–High).

JobSatisfaction → Satisfaction with the job (1–Low, 4–Very High).

RelationshipSatisfaction → Satisfaction with relationships at workplace (1–Low, 4–Very High).

WorkLifeBalance → Perception of work–life balance (1–Bad, 4–Best).

DailyRate → Daily wage.

HourlyRate → Hourly wage.

MonthlyIncome → Monthly salary.

MonthlyRate → Monthly pay rate.

PercentSalaryHike → Percentage increase in salary during last hike.

StockOptionLevel → Stock options provided (0–3).

erformanceRating → Performance score (1–Low, 2–Good, 3–Excellent, 4–Outstanding; mostly 3–4 in this dataset).

TrainingTimesLastYear → Number of training sessions attended last year.

YearsAtCompany → Number of years at the company.

YearsInCurrentRole → Number of years in current role.

YearsSinceLastPromotion → Years since last promotion.

YearsWithCurrManager → Years working with the current manager.

TotalWorkingYears → Total years of work experience.

NumCompaniesWorked → Number of companies the employee has worked for.


Data Import & Inspection

    Loaded dataset HR-Employee-Attrition.csv into a Pandas DataFrame.

    Checked first few rows (head()), data types (info()), missing values (isnull().sum()), and duplicates.

    Confirmed: 1470 employees, 35 columns, no null values, no duplicate EmployeeNumber.

2. Descriptive Statistics

    Used .describe() to get distributions (mean, min, max, quartiles).

    Columns like Age, DailyRate, MonthlyIncome, YearsAtCompany explored.

3. Outlier Detection

    Applied IQR method on MonthlyIncome to identify outliers.

    Visualized using a boxplot.

4. Attrition Analysis

You systematically explored attrition across different factors:

Overall Attrition Rate

    Found 16.12% attrition, majority (83.88%) stayed.

    Visualized with a pie chart.

Job Roles with Highest Attrition

    Sales Representatives (~40%), Laboratory Technicians (~24%), HR (~23%) had highest attrition.

Marital Status & Attrition

    Single employees (~25%) left more than Married (~12%) or Divorced (~10%).

Business Travel Impact

    Frequent Travelers attrition ~25%, Non-travelers ~8%.

Age Group Trends

    <30 yrs: highest attrition (~26%).

    Attrition decreases with age.

Income & Attrition

    Employees who left had lower average income (~₹4787) vs those who stayed (~₹6833).

Distance from Home

    Employees who left lived farther (10.6 km vs 8.9 km).

Education Field

    Highest attrition in Human Resources (~26%) & Technical Degrees.

Job Level Comparison

    Entry-level (Level 1) had the highest attrition (~26%).

    Higher levels (4 & 5) had <10%.

Gender Differences

    Males: ~17% attrition, Females: ~15%.

Overtime Effect

    Overtime workers showed much higher attrition.

Work-Life Balance

    Employees rating 1–2 had higher attrition.

    Ratings 3–4 correlated with better retention.

Years at Company

    Highest attrition in first 0–5 years.

    Long-term employees much more stable.

Performance Rating

    Rating 3 employees showed higher attrition.

    Rating 4 employees had lower exits.

Job Satisfaction & Tenure

    Surprisingly, tenure remained ~7 years regardless of satisfaction level.

Years Since Last Promotion

    Attrition peaked in 0–1 years after promotion.

5. Key Insights / Risk Profile

From all analyses, top attrition drivers identified:

    Overtime workload

    Low salary

    Frequent travel

    Being single or early in career

    Certain job roles (Sales, Lab Tech, HR)

Attrition → Whether the employee left the company (Yes) or stayed (No).

OverTime → Whether the employee works overtime (Yes/No)..
