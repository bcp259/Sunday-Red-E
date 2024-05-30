Hello and welcome to my Capstone Project!

Project overview:
========================================
My project is titled "Sunday Red E." (the E stands for Engineered)

The purpose of this project is to track performances of golfers competing in PGA's 4 Majors (and The Players) and predict the Sunday leaderboard and thus, the winners of each tournament. I see a large range of volatility in golf performance and would like to investigate the performances in each tournament to see if I can predict how well a player wil do. The largest benefactors for this project would be people with some sort of investment in the sport, whether it be financial such as bettors or staff, or even commentators and writers. By having the data to back outcomes, there is a better way to craft narratives and truly understand outcomes at the surface level.

My project incorporates machine learning by taking into account past performance data in the same course / tournament, variables such as tee time and overall performance in order to accurately predict performance in future tournaments. 

Data fields:
My raw metrics are through datagolf.
=========================================
teetime  : the time a player started their round      
sg_putt  : strokes gained putting   
sg_arg   : strokes gained around the green  
sg_app   : strokes gained approach the green  
sg_ott   : strokes gained off-the-tee  
sg_t2g   : strokes gained tee-to-green (sg_arg + sg_app + sg_ott)  
sg_total : strokes gained total (sg_putt + sg_arg + sg_app + sg_ott)  
  
To do list:
=========================================
[ ] Explore sample test data  
[ ] Make preliminary pass throughs to evaluate the mapping needed to be cleaned (e.g. categorize teetime)  
[ ] Test for correlations  
[ ] Incorporate additional datasets (possibility to include golfer place of birth/primary residence, course weather data)  
[ ] Download draftkings
