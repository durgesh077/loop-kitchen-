#### loop-kitchen
#Video loom for trigger_report API
https://drive.google.com/file/d/1pTWAYS63sB6rZqlGHJgGGL-S4JvQyTqP/view?usp=sharing

#Video loom for get_result API
https://drive.google.com/file/d/1eN7HQcja4QBcRA8TK6fFMz2-bpcWoyOO/view?usp=sharing

#directory structure for saving report 
![image](https://user-images.githubusercontent.com/66236446/221466707-ef096822-8d2b-450b-87bc-9691c8a2a1ca.png)

#on wrong report_id 
![image](https://user-images.githubusercontent.com/66236446/221466780-a86dd8d5-bc6d-4f26-bf26-5113cc49e54d.png)


#The logic for computing the hours overlap.
it assumes that the reading that came afterward is correct and each status by default is correct for 1 hour. 
if not reading is given for that , It assumes the previous reading 
for e.g. if time business hour is 1PM - 9PM
then if status is given as follows
-1:30PM , active
-2:36PM , inactive
-3:00 PM, active

1) since 1:30PM is first reading of the day, it will take the first reading say 1:30PM and add extra 30 minutes for active since business hour starts from 1 PM
2) from 1:30PM to 2:36 PM is will be intact for being inactive
3) then on 3:00PM , it will again become active and since no reading further it will assume active 


