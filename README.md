# Fuzzification_ Defuzzification_Implementation from scratch_ using_slope

# Description
	When the crisp value lies in the lines’ shape ranges:
    Mainly using slope to find the fuzzy value.
    Slope of each line for both shape (trapezoid, triangle) is calculated by that given ranges points.
    Triangle:
       # Equation for left-line:
        Slope = (Y2-Y1)/(X2-X1)   =  (1-0)/(range1-range0)   (calculated slope by the given points)
        (fuzzyValue-0)/(CrispValue-range0)=slope
        fuzzyValue= slope*(CrispValue – range0)
       # Equation for right-line:
        Slope = (Y2-Y1)/(X2-X1)   =  (1-0)/(range1-range2)   (calculated slope by the given points)
        (fuzzyValue-1)/(CrispValue-range1)=slope
        fuzzyValue= slope*(CrispValue – range1) + 1
        Trapezoid is similar, but there are two peaks (range1 & range2) which make a little change in the equations but with the same concept… 
  
  When lies in the edge points or outside the shape ranges, fuzzy value = 0
  
  When lies in/ between the middle or the peak point/s, fuzzy value =1
