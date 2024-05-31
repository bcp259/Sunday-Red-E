Hello and welcome to my Capstone Project!

Project overview:
========================================
My project is titled "Sunday Red E." (the E stands for Engineered)

The purpose of this project is to track performances of golfers competing in PGA's 4 Majors (and The Players) and predict the Sunday leaderboard and thus, the winners of each tournament. I see a large range of volatility in golf performance and would like to investigate the performances in each tournament to see if I can predict how well a player wil do. The largest benefactors for this project would be people with some sort of investment in the sport, whether it be financial such as bettors or staff, or even commentators and writers. By having the data to back outcomes, there is a better way to craft narratives and truly understand outcomes at the surface level.

My project incorporates machine learning by taking into account past performance data in the same course / tournament, variables such as tee time and overall performance in order to accurately predict performance in future tournaments. 

Data fields:  
My raw metrics are through datagolf.  
Link to file: https://docs.google.com/spreadsheets/d/1GbzUjp_GneKJeXbqgQWCQ9Tq81TX9njoDz1tspMhLlc/edit?usp=sharing  
=========================================  
`year`                : year in which tournament was played  
`season`              : season of which tournament was played  
`event_id`            : id for tournament  
`dg_id`               : id for player  
`fin_text`            : finishing position  
`round_num`           : round number  
`course_num`          : course number  
`course_par`          : par for respective course  
`round score`         : score for the round  
`sg_putt`             : strokes gained putting     
`sg_arg`              : strokes gained around the green    
`sg_app`              : strokes gained approach the green    
`sg_ott`              : strokes gained off-the-tee    
`sg_t2g`              : strokes gained tee-to-green (sg_arg + sg_app + sg_ott)  
`sg_total`            : strokes gained total (sg_putt + sg_arg + sg_app + sg_ott)  
`driving_dist`        : average distance of drives on par 4 and 5s  
`driving_acc`         : percentage of fairways hit  
`gir`                 : percentage of greens hit in regulation (including fringes)  
`scrambling`          : percentage of shots hit around the green from 50 yards and in that saved par (or were finished in 2                               strokes or less)  
`prox_rgh`            : average proximity of all shots hit from locations besides fairway and intermediate rough  
`prox_fw`             : average proximity of all shots hit from the fairway  
`great_shots`         : self explanatory but related to being in the 95th percentile of  strokes gained metrics  
`poor_shots`          : also self explanatory but related to the 5th percentile of strokes gained metrics  
`teetime_int`         : number of minutes after midnight (i.e. an 8:00am tee     
                        time will be 480 minutes after midnight)  
`tee_time_of_day_int` : grouping of teetime_int.   
                        group 1 = teetime from 8:00AM to 10:00AM  
                        group 2 = teetime from 10:00AM to 12:00PM  
                        group 3 = teetime anytime after 12:00PM  
`made_cut`            : binomial column, indicates whether a player made the cut(1) or not(0)  

Notes about data:
- if a player did not make the cut (`made_cut` = 0), they will not have an entry for `round_num` 3 or 4 and no subsequent stats related for the rounds
- `driving_dist` only includes drives on par 4s and par 5s since a driver is not used on par 3s

To do list:
=========================================
[X] Explore sample test data  
[X] Make preliminary pass throughs to evaluate the mapping needed to be cleaned (e.g. categorize teetime)  
[X] Test for correlations
[ ] Adjust dataframe for the purposes of running regression model
    > drop columns  
      - year, season, course_num, course_par (constant values)  
      - start_hole? need to dig deeper and see if masters is not shotgun start aka everyone will start at hole 1  
[ ] Incorporate additional datasets (possibility to include golfer place of birth/primary residence, course weather data)  
