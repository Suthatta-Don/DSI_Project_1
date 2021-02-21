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
### Conclusions and Recommendations

According to data analysis, students preferred to take the SAT more than the ACT, and it seems like the SAT and the ACT will have the same level of preference from student because the average SAT and ACT participation are the same number (nearly 50%). The increased participation rate gives positive effects on the number of test taker, but not on the average score of the test. The participation rate is negative correlated with the average score. Many states are facing this problem such as Colorado and Illinois, including West Virginia. These states have the policy to convince students to take exam namely mandatory SAT testing and free SAT School Day. 

According to the data, it shows that West Virginia's SAT participation increases by 70% but the average score decreases slightly, that opposite of the ACT. Colorado also has this problem, mandatory SAT policy made SAT participation 2018 hit 100% but the score decreases. West Virginia's SAT score is lower than the mean score in both two years (2018-2019) which means West Virginia's has a low score before the new policy.

West Virginia offers free SAT School Day to all students to increases the chance for university admission. Therefore, students in West Virginia should take the test and get more score at 1150 to reach the median score of university admission. West Virginia should make SAT testing to be a part of graduation requirements without free SAT School Day and determine the range of score to graduate and get a free SAT School Day test. The lowest score for graduation should not lower than the mean score of West Virginia in the previous year, and if a student's score reaches the median of university admission they will get the free SAT School Day (return the fund). This new policy will encourage the student to prepare for testing and the school will give more training to the student. 

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
