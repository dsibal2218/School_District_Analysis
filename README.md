# School_District_Analysis

Overview: We were given two datasets to review and analyze. The first dataset has more than 30,000 students information that includes their basic demographic, what grade they are in, highschool name and grades for reading and math. The second dataset has highschool information such as the type of school, size and their budget. We were told that the file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. We were asked to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once they're replaced, we will do some extensive analysis and write up a report to describe how these changes affected the overall analysis compare to how it was before the math and reading scores were replaced with NaNs. We have done the original analysis during the class module.

## Requirements and Details of the Analysis

1. Using the Pandas loc method with conditional statements and comparison and logical operators, select the ninth-grade reading and math scores for Thomas High School. Then, use the Pandas NumPy module to change the reading and math scores to NaN.

2. Perform the following analysis and compare it to the one we did during class module:
    a.  The district summary: We will have to recalculate the total student count by subtracting the number of ninth grade students in Thomas High School 
        from the total student count, then you'll recalculate the passing math and passing reading percentages, and the overall passing percentage with
        the recalculated total student count.

    <img width="1098" alt="Screen Shot 2022-03-26 at 9 59 04 PM" src="https://user-images.githubusercontent.com/98235755/160263392-3c6838d4-50d1-496a-95d4-0e29e30ab9c8.png">


    a.  The district summary: We will have to recalculate the total student count by subtracting the number of ninth grade students in Thomas High School from the total student count, then we'll recalculate the passing math and passing reading percentages, and the overall passing percentage with the recalculated total student count.
    
    <img width="1005" alt="Screen Shot 2022-03-26 at 10 02 36 PM" src="https://user-images.githubusercontent.com/98235755/160263469-063a4663-8426-41d8-9afe-f44ff813177b.png">

    
    b.  The school summary: After recalculating we will replace the % Passing Math, % Passing Reading, and % Overall    
        Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School.
    
    <img width="1104" alt="Screen Shot 2022-03-26 at 10 03 55 PM" src="https://user-images.githubusercontent.com/98235755/160263504-15970434-f95d-4f02-9aa1-22f553d3626a.png">

    c.  The top 5 and bottom 5 performing schools, based on the overall passing rate
    
    <img width="863" alt="Screen Shot 2022-03-26 at 10 05 40 PM" src="https://user-images.githubusercontent.com/98235755/160263544-65ec7e60-eeec-40a8-9010-a22ee0df6d03.png">
  
    <img width="865" alt="Screen Shot 2022-03-26 at 10 06 16 PM" src="https://user-images.githubusercontent.com/98235755/160263567-4440120e-bb70-4f42-a4be-085d5e5129c1.png">

    d.  The average math score for each grade level from each school
    
    <img width="490" alt="Screen Shot 2022-03-26 at 10 07 21 PM" src="https://user-images.githubusercontent.com/98235755/160263592-01db4763-1eaf-4947-8d57-75bc39c1d421.png">
    
    e.  The average reading score for each grade level from each school
    
    <img width="485" alt="Screen Shot 2022-03-26 at 10 07 45 PM" src="https://user-images.githubusercontent.com/98235755/160263602-8e57efd0-4757-4778-a1e7-cb0fa435eef3.png">

    f.  The scores by school spending per student, by school size, and byschool type 
    
    <img width="897" alt="Screen Shot 2022-03-26 at 10 12 04 PM" src="https://user-images.githubusercontent.com/98235755/160263704-b414eceb-16d7-4873-a942-b99d9a06e974.png">

    <img width="746" alt="Screen Shot 2022-03-26 at 10 13 23 PM" src="https://user-images.githubusercontent.com/98235755/160263722-b433ab2c-2526-41b9-b6a4-4108ddd32301.png">

    <img width="844" alt="Screen Shot 2022-03-26 at 10 13 49 PM" src="https://user-images.githubusercontent.com/98235755/160263724-8ed0eff5-a548-4850-8edd-3503a3caafc5.png">


## Results of the Analysis

1. How is the district summary affected? - As shown in the side-by-side comparison of the school district summary from the original analysis and one where we excluded the 9th grade from Thomas Highschool, all grades have gone down - both in average and passing rates.

<img width="1340" alt="Screen Shot 2022-03-26 at 10 33 49 PM" src="https://user-images.githubusercontent.com/98235755/160264194-00b1858c-ce43-4524-8a0d-8766671e5141.png">

2. How is the school summary affected? - It only really affected Thomas Highschool's metric. As shown below, for Thomas Highschool, all scores (both average and overall), except for average reading score, went down by a tiny bit. 

<img width="1414" alt="Screen Shot 2022-03-26 at 10 52 14 PM" src="https://user-images.githubusercontent.com/98235755/160264653-0b0ee432-cd08-4231-8518-1d0240896001.png">

3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools? - As mentioned above, it only negatively affected Thomas Highschool's scores by a tiny bit. Also, changing the math and reading scores didnt affect Thomas Highschool's rank being in the top 5 school based on overall score.

4. How does replacing the ninth-grade scores affect the following:

    a.  Math and reading scores by grade - As shown below, Thomas Highschool's math and reading scores both show as "NaN" in the new analysis.
    
    <img width="1328" alt="Screen Shot 2022-03-26 at 11 06 21 PM" src="https://user-images.githubusercontent.com/98235755/160264958-ca349608-b714-46e1-822e-bac066063617.png">

    b.  Scores by school spending - A very tiny bit of impact on the scores in the $631-645 spending range. 
   
   <img width="1458" alt="Screen Shot 2022-03-26 at 11 16 33 PM" src="https://user-images.githubusercontent.com/98235755/160265149-d1664d9c-cd87-48cd-9a58-0d318832d726.png">

    c.  Scores by school size
    <img width="1431" alt="Screen Shot 2022-03-26 at 11 20 21 PM" src="https://user-images.githubusercontent.com/98235755/160265219-f29d061c-267a-49c5-aec9-8a140e42fc73.png">

 
    d.  Scores by school type

<img width="1438" alt="Screen Shot 2022-03-26 at 11 21 36 PM" src="https://user-images.githubusercontent.com/98235755/160265239-68382e6e-156b-4a41-9110-e0865a1eae66.png">

Summary: Overall, changing the 9th grade's math and reading scores to NaN for Thomas Highschool didn't affect the ranking of the schools. It barely affected the scores by school type, school size, and school spending (~.05%) that you can't even tell the changes when you round the scores. 
