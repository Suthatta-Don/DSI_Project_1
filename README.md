# DSI_Project_1
Project 1 (SAT and ACT analysis)

# ![](https://ga-dash.s3.amazonaws.com/production/assets/logo-9f88ae6c9c3871690e33280fcf557f33.png) Project 1: Standardized Test Analysis

### Overview

Our first module in DSI covers:
- Basic statistics and probability
- Many Python programming concepts
- Programmatically interacting with files and directories
- Visualizations
- EDA
- Working with Jupyter notebooks for development and reporting

You might wonder if you're ready to start doing data science. While you still have **tons** to learn, there are many aspects of the data science process that you're ready to tackle. Project 1 aims to allow you to practice and demonstrate these skills.

For our first project, we're going to take a look at aggregate SAT and ACT scores and participation rates in the United States. We'll seek to identify trends in the data and combine our data analysis with outside research to address our problem statement.

---
### Background
The SAT and ACT are standardized tests that many colleges and universities in the United States require for their admissions process. This score is used along with other materials such as grade point average (GPA) and essay responses to determine whether or not a potential student will be accepted to the university.

The SAT has two sections of the test: Evidence-Based Reading and Writing and Math ([*source*](https://www.princetonreview.com/college/sat-sections)). The ACT has 4 sections: English, Mathematics, Reading, and Science, with an additional optional writing section ([*source*](https://www.act.org/content/act/en/products-and-services/the-act/scores/understanding-your-scores.html)). They have different score ranges, which you can read more about on their websites or additional outside sources (a quick Google search will help you understand the scores for each test):
* [SAT](https://collegereadiness.collegeboard.org/sat)
* [ACT](https://www.act.org/content/act/en.html)

Standardized tests have long been a controversial topic for students, administrators, and legislators. Since the 1940's, an increasing number of colleges have been using scores from sudents' performances on tests like the SAT and the ACT as a measure for college readiness and aptitude ([*source*](https://www.minotdailynews.com/news/local-news/2017/04/a-brief-history-of-the-sat-and-act/)). Supporters of these tests argue that these scores can be used as an objective measure to determine college admittance. Opponents of these tests claim that these tests are not accurate measures of students potential or ability and serve as an inequitable barrier to entry.

**SAT School Day in West Virginia**

One reasons for 2018-2019's increased SAT participation is the continued growth of SAT School Day, including in West Virginia, which offered free SAT School Day to every students in 2018-2019. School Day gives more chance for all students to access to the SAT and provides the familiar surroundings with people they know. Students take the test at their own school, during a regular school day, usually at no cost to them ([*source*](https://reports.collegeboard.org/archive/sat-suite-program-results/2019/benefits-sat-school-day)). For West Virginia, this state offers the free SAT School Day to students and aims to increase participation rate. Free SAT School day can help students to open the dorr to college, university and scholarship ([*source*](https://collegereadiness.collegeboard.org/sat/k12-educators/sat-school-day/about)).

---
### Problem Statement

West Virginia has the policy to increase the participation rate in 2018 by offering the free SAT School DAY to students. The aim of this policy is opening the door to college, university and scholarship. This policy increased the participation rate significantly, but the total score did not increase. So, if West Virginia wants to increase both participation rate and average score. How to adjust the policy to be more effective?

---
### Executive Summary
This project examines data covering participation rates and scores for students taking the SAT and the ACT in 2017-2019 by state. The data are organised participation rate, total/composite score (only SAT has a score for each part). This encourages to analyse by comparison between the state in the data to get the interesting state (in this project is West Virginia) to look insight and get more profit from data. This project also analyses the range of score for university admission to get the median SAT score at 1150. This score is a recommended score for the student should reach for getting more chance and choice on university admission day. All datasets are analysed and found how to adjust the policy to maintain the participation rate. Colorado switch to mandatory SAT testing which can remain a constant participation rate at 100%. Therefore, West Virginia should mix policy to maintain participation rate and to increase the average score. SAT testing should be the requirement to graduate from high school and the minimum score should not lower than West Virginia's score in the previous year. If a student's score over a median score of the university's average median score at 1150, they will receive a free SAT School Day.

---
### Conclusions and Recommendations

According to data analysis, students preferred to take the SAT more than the ACT, and it seems like the SAT and the ACT will have the same level of preference from student because the average SAT and ACT participation are the same number (nearly 50%). The increased participation rate gives positive effects on the number of test taker, but not on the average score of the test. The participation rate is negative correlated with the average score. Many states are facing this problem such as Colorado and Illinois, including West Virginia. These states have the policy to convince students to take exam namely mandatory SAT testing and free SAT School Day. 

According to the data, it shows that West Virginia's SAT participation increases by 70% but the average score decreases slightly, that opposite of the ACT. Colorado also has this problem, mandatory SAT policy made SAT participation 2018 hit 100% but the score decreases. West Virginia's SAT score is lower than the mean score in both two years (2018-2019) which means West Virginia's has a low score before the new policy.

West Virginia offers free SAT School Day to all students to increases the chance for university admission. Therefore, students in West Virginia should take the test and get more score at 1150 to reach the median score of university admission. West Virginia should make SAT testing to be a part of graduation requirements without free SAT School Day and determine the range of score to graduate and get a free SAT School Day test. The lowest score for graduation should not lower than the mean score of West Virginia in the previous year, and if a student's score reaches the average median of university admission (1150) they will get the free SAT School Day (return the fund). This new policy will encourage the student to prepare for testing and the school will give more training to the student. 

---
### Datasets

* [`act_2017.csv`](./data/act_2017.csv): 2017 ACT Scores by State which consists of the participation percentage, score for each part and composite
* [`act_2018.csv`](./data/act_2018.csv): 2018 ACT Scores by State which consists of the participation percentage and composite
* [`act_2019.csv`](./data/act_2019.csv): 2019 ACT Scores by State which consists of the participation percentage and composite
* [`sat_2017.csv`](./data/sat_2017.csv): 2017 SAT Scores by State which consists of the participation percentage, score for each part and total
* [`sat_2018.csv`](./data/sat_2018.csv): 2018 SAT Scores by State which consists of the participation percentage, score for each part and total
* [`sat_2019.csv`](./data/sat_2019.csv): 2019 SAT Scores by State which consists of the participation percentage, score for each part and total
* [`sat_act_by_college.csv`](./data/sat_act_by_college.csv): Range of Accepted ACT & SAT Student by Colleges
* [`act_2019_ca.csv`](./data/act_2019_ca.csv): ACT Scores in California by School in 2019 (This dataset is used for EDA part only)

**Data dictionary**

**1. Data dictionary for dataset named 'total_score'**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**state**|*object*|total_score|the name of U.S. state| 
|**participation_act2017**|*float*|total_score|percent of participant in 2017 for ACT|
|**composite_act2017**|*float*|total_score|ACT composite score in 2017|
|**participation_act2018**|*float*|total_score|percent of participant in 2018 for ACT|
|**composite_act2018**|*float*|total_score|ACT composite score in 2018|
|**participation_act2019**|*float*|total_score|percent of participant in 2019 for ACT|
|**composite_act2019**|*float*|total_score|ACT composite score in 2019|
|**participation_sat2017**|*float*|total_score|percent of participant in 2017 for SAT|
|**reading_writing_sat2017**|*integer*|total_score|average SAT evidence-based reading and writing score in 2017|
|**math_sat2017**|*integer*|total_score|average SAT math score in 2017|
|**total_sat2017**|*integer*|total_score|SAT total score in 2017|
|**participation_sat2018**|*float*|total_score|percent of participant in 2018 for SAT|
|**reading_writing_sat2018**|*integer*|total_score|average SAT evidence-based reading and writing score in 2018|
|**math_sat2018**|*integer*|total_score|average SAT math score in 2018|
|**total_sat2018**|*integer*|total_score|SAT total score in 2018|
|**participation_sat2019**|*float*|total_score|percent of participant in 2019 for SAT|
|**reading_writing_sat2019**|*integer*|total_score|average SAT evidence-based reading and writing score in 2019|
|**math_sat2019**|*integer*|total_score|average SAT math score in 2019|
|**total_sat2019**|*integer*|total_score|SAT total score in 2019|

**2. Data dictionary for dataset named 'df_uni'**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**school**|*object*|df_uni|The name of college and university|
|**number_applicants**|*integer*|df_uni|number of applicants|
|**accept_rate**|*float*|df_uni|acceptance rate (2018-2019)|
|**sat_25_75**|*object*|df_uni|SAT 25th-75th percentile (2018-2019)|
|**act_25_75**|*object*|df_uni|ACT 25th-75th percentile (2018-2019)|
|**act_25th**|*float*|df_uni|ACT 25th percentile (2018-2019)|
|**act_75th**|*float*|df_uni|ACT 75th percentile (2018-2019)|
|**sat_25th**|*float*|df_uni|SAT 25th percentile (2018-2019)|
|**sat_75th**|*float*|df_uni|SAT 75th percentile (2018-2019)|

**3. Data dictionary for dataset named 'act_ca'**

|Feature|Type|Dataset|Description|
|---|---|---|---|
|**school**|*object*|act_ca|name of high school in California|
|**district**|*object*|act_ca|name of district in California|
|**city**|*object*|act_ca|The name of city in California|
|**enroll12**|*float*|act_ca|enrollment of Grade 12 (2019)|
|**number_taker**|*float*|act_ca|number of test taker (2019)|
|**reading**|*float*|act_ca|average ACT reading score (2019)|
|**english**|*float*|act_ca|average ACT english score (2019)|
|**math**|*float*|act_ca|average ACT math score (2019)|
|**science**|*float*|act_ca|average ACT science score (2019)|
