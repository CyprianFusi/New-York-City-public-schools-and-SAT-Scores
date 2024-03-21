# New-York-City-public-schools-and-SAT-Scores
One of the most controversial issues in the U.S. educational system is the efficacy of standardized tests and whether they're unfair to certain groups.  We could correlate SAT scores with factors like race, gender, income, and more.

# Scholastic Aptitude Test (SAT) Controversies
The SAT, or Scholastic Aptitude Test, is an exam that U.S. high school students take before applying to college. The SAT has three sections, each is worth 800 points. Colleges take the test scores into account when deciding who to admit, so it's important to perform well.
One of the most controversial issues in the U.S. educational system is the efficacy of standardized tests and whether they're unfair to certain groups. Given our prior knowledge of this topic, investigating the correlations between SAT scores and demographics might be an interesting angle to take. We could correlate SAT scores with factors like race, gender, income, and more.

# Observations
* `total_enrollment` has a strong positive correlation with `sat_score`. This is surprising because we'd expect smaller schools where students receive more attention to have higher scores. However, it looks like the opposite is true -- larger schools tend to do better on the SAT.
    * Other columns that are proxies for enrollment correlate similarly. These include total_students, `N_s`, `N_p`, `N_t`, `AP Test Takers`, `Total Exams Taken`, and `NUMBER OF SECTIONS`.
* Both the percentage of females (`female_per`) and number of females (`female_num`) at a school **correlate positively** with SAT score, whereas the percentage of males (`male_per`) and the number of males (`male_num`) **correlate negatively**. This could indicate that *female candidates do better on the SAT thir male counterpart*.
* Teacher and student ratings of school safety (`saf_t_11`, and `saf_s_11`) correlate with `sat_score`.
* Student ratings of school academic standards (`aca_s_11`) correlate with `sat_score`, but this does not hold for ratings from teachers and parents (`aca_p_11` and `aca_t_11`).
* There is significant racial inequality in SAT scores (`white_per`, `asian_per`, `black_per`, `hispanic_per`).
* The percentage of students eligible for free or reduced school lunch based on household income (`frl_percent`) has a **strong negative correlation** with SAT scores.
* **Students from `white`and `asian` backgrounds seem to perform well in SAT than their counterparts from `black`and `hispanic` backgrounds**.
* **The SAT scores are high when the percentage of hsipanic students is low and low when the percentage of hsipanic students is high**! The SAT remains fairly constant from about 25% and above of hispanic students.
* **Female gender seems to correlate positively (albeit a very weak correlation) with SAT score while Male correlates negatively. This means as the number of female students increase SAT score also increases. This is the reverse with male students.**
* The Correlation between the **proportion of AP Test Takers and SAT Score** is surprisingly very weak! This means that the proportion of student who sit for AP exams does not noticeably increase as the SAT scores.

Our research revealed that **most of the high schools with low total enrollment and low SAT scores have high percentages of English language learners**. This indicates that it's actually **`ell_percent` that correlates strongly with `sat_score`**, rather than `total_enrollment`.

