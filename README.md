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
    
## Results of the Analysis

