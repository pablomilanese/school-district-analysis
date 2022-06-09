# SCHOOL DISTRICT ANALYSIS
## OVERVIEW
The purpose of this project was to analyze math and reading testing results for various schools within a district in order to measure student performance, budget allocation, type of school and how these variables intertwine. By showing this information in a clear way the district can adjust their budget in order to boost student performance.

##### ACADEMIC DISHONESTY IN THOMAS HIGH SCHOOL
The school board alerted us that there was evidence of academic dishonesty concerning Thomas High School ninth graders. In order to uplhold state-testing standards it was decided to 'blank out' their math and reading results while keeping the rest of the data intact. One of the main purposes of this project was to compare how our original analysis fared against our redacted analysis.

## RESULTS

##### HOW IS THE DISTRICT SUMMARY AFFECTED?
The District Summary was not heavily affected. After going over our initial analysis and the new one we can see that the variables that changed were the percentages for passing math and reading. The overall percentage was affected by 0.1%.

<img width="929" alt="Screen Shot 2022-06-08 at 11 17 17 PM" src="https://user-images.githubusercontent.com/105120795/172763209-4bfd999c-b33f-4779-b7ef-dfe6f2a8a1bc.png">
<img width="929" alt="Screen Shot 2022-06-08 at 11 18 19 PM" src="https://user-images.githubusercontent.com/105120795/172763196-f5355bca-5418-4ba0-9785-4d33f656ddd7.png">


##### HOW IS THE SCHOOL SUMMARY AFFECTED?
Because the only school that presented academic dishonesty was Thomas High School, this was the only one that was affected. The main purpose of our reworking of the original code was to make sure that the rest of the information remained intact. Because of this we can corroborate that our job was succesful.

<img width="1004" alt="Screen Shot 2022-06-08 at 11 21 39 PM" src="https://user-images.githubusercontent.com/105120795/172763506-1234df7c-5266-41dc-ba00-5a631f85022a.png">
<img width="998" alt="Screen Shot 2022-06-08 at 11 21 28 PM" src="https://user-images.githubusercontent.com/105120795/172763516-766428a7-e9b8-4e6b-9868-aa77a667d1fc.png">


##### HOW DOES REPLACING THE NINTH GRADERS’ MATH AND READING SCORES AFFECT THOMAS HIGH SCHOOL’S PERFORMANCE RELATIVE TO THE OTHER SCHOOLS?
Replacing the ninth graders' math and reading scores affected Thomas High School's performance significantly. Thomas High dropped from being in the top bracket to the lower bracket.

##### HOW DOES REPLACING THE NINTH-GRADE SCORES AFFECT THE FOLLOWING:

##### MATH AND READING SCORES BY GRADE
Replacing the ninth-grade scores affected the math and reading scores by grade negatively, making their overall scoring drop. Given that the ninth grade results were replaced by NaN, this pulled down the performance of the rest of the school.

##### SCORES BY SCHOOL SPENDING
Replacing the ninth-grade scores did not affect the school spending by much. Given that the budget allocated considers numbers of students as a metric instead of grades, it was not affected by a lot.
<img width="1002" alt="Screen Shot 2022-06-08 at 11 29 47 PM" src="https://user-images.githubusercontent.com/105120795/172764496-d85cfa6a-8e39-4d52-a311-31069d6772ea.png">
<img width="1017" alt="Screen Shot 2022-06-08 at 11 29 41 PM" src="https://user-images.githubusercontent.com/105120795/172764500-5ead3197-4739-4d9a-a521-2fd01963f3dd.png">


##### SCORES BY SCHOOL SIZE
Thomas High School is a medium sized school. Given that only one grade level was affected within one school out of the total number of schools per size bracket, the results were not affected.

<img width="772" alt="Screen Shot 2022-06-08 at 11 36 13 PM" src="https://user-images.githubusercontent.com/105120795/172765080-b268039f-4255-47fc-b82f-1721d21df877.png">
<img width="773" alt="Screen Shot 2022-06-08 at 11 35 20 PM" src="https://user-images.githubusercontent.com/105120795/172765092-c32c4c42-f19a-4fb1-a029-3d31077d69b6.png">



##### SCORES BY SCHOOL TYPE
Because the datarange that was removed is small in comparison to the charter & district index, the results were not affected by much.
<img width="724" alt="Screen Shot 2022-06-08 at 11 40 54 PM" src="https://user-images.githubusercontent.com/105120795/172765657-8957ff8e-3c43-4a2a-8cfb-6b4269b03c2a.png">
<img width="718" alt="Screen Shot 2022-06-08 at 11 40 49 PM" src="https://user-images.githubusercontent.com/105120795/172765680-7fcbb96e-5b57-4ae4-aaff-ccfa993e0a63.png">

## SUMMARY · FOUR CHANGES IN THE UPDATED SCHOOL DISTRICT ANALYSIS
After fixing out dataframes there are many points that become evident:
1. Academic dishonesty can bring the overall passing percentage of a school drastically. As shown in our analysis, Thomas High went from having a percentage in the low 90s to a percentage in the high 60s.
2. Academic dishonesty within a school may not affect the overall results of a district. Because this only happened in a single grade, inside a single school, the amount of grades spread out between the rest of the schools still gave us a good idea of academic performance. If this same scenario had happened in multiple schools and multiple grades, our results would become so heavily skewed that the district might have to put in place safety measures across the board to prevent cheating in the future.
3. Replacing ninth graders' results with NaN while keeping student count and budget information helped us to extract other conclusions while blanking out testing results. If we had completely deleted Thomas High 9th graders' information we could have lost some other valuable information.
4. Using NaNs is a incredibly useful tool to respect overall results while also being able to analyze how a particular school can be affected by academic dishonesty.
