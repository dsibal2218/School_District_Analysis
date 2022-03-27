# School_District_Analysis

**Overview**: We were given two datasets to review and analyze. The first dataset has more than 30,000 students information that include their basic demographic, grade they are in, their highschool name and their grades for reading and math. The second dataset has highschool information such as the type of school, size and their budget. We were told that the file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. We were asked to replace the math and reading scores for Thomas High School with NaNs while keeping the rest of the data intact. Once they're replaced, we will have to do some extensive analysis and write up a report to describe how these changes affected the overall analysis compare to how it was before the math and reading scores were replaced with NaNs. We have done the original analysis during the class module.

## Requirements and Details of the Analysis

1. Using the Pandas loc method with conditional statements and comparison and logical operators, select the ninth-grade reading and math scores for Thomas High School. Then, use the Pandas NumPy module to change the reading and math scores to NaN.

![Screen Shot 2022-03-27 at 2 13 04 PM](https://user-images.githubusercontent.com/98235755/160294869-81c5e968-f4e8-44d9-92b3-9fb62be92bb3.png)


2. Perform the following analysis and compare it to the initial analysis we did during class module:
  
    a.  The district summary: We will have to recalculate the total student count by subtracting the number of ninth grade students in Thomas High School from the total student count, then we'll recalculate the passing math and passing reading percentages, and the overall passing percentage with the recalculated total student count.
    
    b.  The school summary: After recalculating we will replace the % Passing Math, % Passing Reading, and % Overall    
        Passing scores in the current School Summary DataFrame with the new passing percentages for Thomas High School.
    
    c.  The top 5 and bottom 5 performing schools, based on the overall passing rate
  
    d.  The average math score for each grade level from each school
   
    e.  The average reading score for each grade level from each school
    
    f.  The scores by school spending per student, by school size, and byschool type 
    
  
## Results of the Analysis

1. How is the district summary affected? - As shown in the side-by-side comparison of the school district summary from the original analysis and one where we excluded the 9th grade from Thomas Highschool, all grades have gone down - both in average and passing rates but very very minimal.

<img width="1340" alt="Screen Shot 2022-03-26 at 10 33 49 PM" src="https://user-images.githubusercontent.com/98235755/160264194-00b1858c-ce43-4524-8a0d-8766671e5141.png">

2. How is the school summary affected? - It only really affected Thomas Highschool's metric. As shown below, for Thomas Highschool, all scores (both average and overall), except for average reading score, went down by a tiny bit. 

<img width="1414" alt="Screen Shot 2022-03-26 at 10 52 14 PM" src="https://user-images.githubusercontent.com/98235755/160264653-0b0ee432-cd08-4231-8518-1d0240896001.png">

3. How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools? - As mentioned above, it only negatively affected Thomas Highschool's scores by, again, a tiny bit. Also, changing the math and reading scores didn't affect Thomas Highschool's rank being in the top 5 school based on overall score.

4. How does replacing the ninth-grade scores affect the following:

    a.  Math and reading scores by grade - As shown below, Thomas Highschool's math and reading scores both show as "NaN" in the new analysis.
    
    <img width="1328" alt="Screen Shot 2022-03-26 at 11 06 21 PM" src="https://user-images.githubusercontent.com/98235755/160264958-ca349608-b714-46e1-822e-bac066063617.png">

    b.  Scores by school spending - A very slight decrease on the scores in the $631-645 spending range. 
   
   <img width="1458" alt="Screen Shot 2022-03-26 at 11 16 33 PM" src="https://user-images.githubusercontent.com/98235755/160265149-d1664d9c-cd87-48cd-9a58-0d318832d726.png">

    c.  Scores by school size -  A minimal decrease on the scores for medium sized schools
    
    <img width="1431" alt="Screen Shot 2022-03-26 at 11 20 21 PM" src="https://user-images.githubusercontent.com/98235755/160265219-f29d061c-267a-49c5-aec9-8a140e42fc73.png">

 
    d.  Scores by school type - A small decrease on the scores for charter school type

<img width="1438" alt="Screen Shot 2022-03-26 at 11 21 36 PM" src="https://user-images.githubusercontent.com/98235755/160265239-68382e6e-156b-4a41-9110-e0865a1eae66.png">

Summary: Overall, changing the 9th grade's math and reading scores to NaN for Thomas Highschool and excluding them in the calculations didn't affect the ranking of the school. Additionally, it barely affected the scores by school type, school size, and school spending (mostly <.05%) that you can't even tell the changes when you round the scores. 
