# [HAWKEYE AND FLOODFILL ⇾⚄ (EASY) - Editorial/Solution](https://www.hackerearth.com/practice/basic-programming/implementation/basics-of-implementation/practice-problems/algorithm/hawkeye-and-floodfill/description/)
Please refer to the problem statement linked above for understanding the problem and sample test cases.
  
## Before you start solving.
The intent behind creating this problem was to tell students that they should never directly jump to conclusions without doing any pre-assessment or investigation. Although the problem title states flood fill, the problem is not a typical flood fill problem.

## Problem break down.
• We can restate the problem as, at any given index x1,y1 you have to find how far the point of impact x2,y2 (where the arrow hit) is. Now from any current index x1,y1 in the metrics, the point of impact x2,y2 will either be x distance away horizontaly or y distance away verticaly.

![Metrics index representaion explaining horizontal and veritical distance](https://github.com/seal-7/Editorials/blob/main/HackEyeDiagram.png)

To calculate the power at any given index x1,y1 you have to subtract maximum of horizontal or vertical distance from the power at which the arrow hit 'P'.
## Sudo Code
      for( i , 0 .. n-1 ) {
        for( j, 0 .. n-1 ) {
          distance = max(abs(x-i), abs(y-j))
          impactAtCurrentIndex = (power - distance) > 0 ? (power - distance) : 0
          
The reason why I am not publising the working soultion is I want you to code if yourself after undertanding. Although if you still want the working solution, you can find it [here](https://www.hackerearth.com/practice/basic-programming/implementation/basics-of-implementation/practice-problems/algorithm/hawkeye-and-floodfill/editorial/) PS: it's not well coded for understanding, hence keeping my intent intact of you solving it by yourself :-p 
