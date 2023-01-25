# NFLBigDataBowl2023
Kaggle competition for Big Data Bowl 2023
# Linebackers - Spin to Win!

*This notebook was created as part of the educational project. You can find more information here: [NFL Big Data Bowl by Practicum](https://www.kaggle.com/ernestglukhov/nfl-big-data-bowl-by-practicum)*

The best introduction we find to the role of a linebacker is that they are a quarterback of the defense line. A perfect linebacker has to be jack of all trades, has high game intelligence, be agile, swift, big but not too big. A good linebacker is a backbone of defense and it is usually one of the most valuable defense players. There are three linebackers in the top 5 defensive players ranked by salary in NFL 2022.

![spin](https://media.tenor.com/nnhFRQSsvskAAAAC/ballet-dance.gif "spinning")



In our work we try to answer the question:

**What makes the best linebackers the best?**

If one asks a scout - game IQ (vision, recognition) comes first, but it is not the focus of our research here. And so is it - size (`weight`, `height`), `speed`, `acceleration`? Maybe something else? 
* **Rotation**: ability to move quickly around yourself, squeeze through tight offensive lines dodging grabs and blocks
* **Change of direction**: ability to change direction of movement, zig-zag movements like a cone-drill


* While speed and acceleration are well studied, ability to change direction / rotational movements are not so much:
    * LB can move in a straight line or zig-zag around, fool linemen with their quick footwork effectively getting to the ball, stopping the offensive play. We believe that it should make a difference and one's ability to move their feet quickly should be seen in the performance.

**To illustrate our reasoning - here is the movement graph of a quarterback sack.**
<br>*The blue dots are the player's position on the field. Black lines indicate where they are facing, the length of the line indicates speed.*

![image](https://user-images.githubusercontent.com/12784655/214554669-dc0d8b44-d115-488d-b65e-073b8d8792cc.png)



One can recognize S.Barrett's play vs Miami Dolphins quarterback: [youtube video](https://youtu.be/HtUr_MW83sA?t=85) 



**Methodology: defining a successful play**:
* We look at the first 8 weeks of data of the NFL 2021-22 season and extract data from all pass rushes plays by linebackers.
* As an individual performance measure, methodology implies that a pass rush is successful if that player completes a quarterback sack, hit or hurry and fails otherwise.


**What do we do?**
1. *Load data, EDA*:  look at linebackers and number of sacks, hits and hurries. Try to define the most successful players.
2. *Form stats, metrics*: extract relevant data from frame by frame plays. Introduce new metrics to measure performance
3. *Study qb sacks:* take a closer look at qb sacks as one of the most valuable linebacker's plays. 
4. *Cross-data analysis:* What are the defining characteristics of a successful play?
5. *Cross-player analysis:* what makes the best players the best?
6. *Form the results*
 
   
**Summary of the results - *Spin to win!***

    
*  We found statistical evidence that in order to complete a successful pass rush a linebacker needs to move faster, rotate more, be able to change direction more:
    * During a sack, for example, linebackers on average both **rotate**  and **change direction** about full circle in total         
* From player specific data we found that **the best linebackers** are the ones who are able to generate enough momentum (*force* defined as a product of `weight` and `acceleration`) as well as demonstrating better `rotational movements` than their colleagues in this position.


**Applications and further research**:
* Coaches might want to include more exercise involving spinning and rotating to their drills
* Scouts are already look at the the bigger players but now they might also want to see how quick one on their feet and able to move through offense demonstrating rotation movements
* Further research might include a larger database to incorporate more data on sacks, hits and hurries. Also similar research could be done for different types of positions
