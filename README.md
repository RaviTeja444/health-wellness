# Walk Tracker
WalkTracker is a digital health and wellness platform that provides services such as calorie tracking, one-on-one nutrition and fitness coaching, and diet and workout plans. Developed for both Android and iOS platforms, the app takes a holistic lifestyle tracking approach to keep users engaged and motivated.

## Link to Hosted Page
[Click here](https://raviteja444.github.io/health-wellness/)

## Link to Repository
[Click_here](https://github.com/RaviTeja444/health-wellness)

## Statement of purpose
WalkTracker is a free to download and use mobile application which provides a health promotional service assisting users to track their health and wellness progress. We plan to develop a software that helps to see better results in weight loss, building muscles, toning up, or controlling medical conditions. Premium plans along with personal coaching with fun health group and wellness challenges, while also being able to share results.
 
## Objective
Having a fit and healthy body is everyone's dream, but it has somehow not been everyone's cup of tea. Between 2017 and 2018, the National Health and Nutrition Examination Survey observes 1 out of every 4 children are suffering from Obesity, also obesity is linked to more than 60 chronic diseases and there is epidemic of obesity around the world.

In the U.S., childhood obesity alone is estimated to cost $14 billion annually in direct health expenses. Unhealthy lifestyle and eating habits has direct impact on physical health causing damage to metabolism, which has impact on mental well-being too. Most part of the problem comes from a lack of awareness of what people are eating and how much energy they burn every day.

WalkTracker is a digital technology to help people eat better, get fitter and lose weight. The primary solution is delivered via a smartphone app (iOS, Android, PC) with a team of qualified diet/ fitness expert’s available in-app. It also allows optional integration with various tracking wearables. The funds would be used in developing AI and ML interface, so that it can service more users with fitness suggestions, healthy alternative food and task recommendations.

Our app will help users to track their health and wellness progress using step count. Also, will be providing points based on the steps count. The rewarded points can be used to buy products like Our University T-Shirts,Caps.

## Benefits
1. The app helps users to track their steps, food intake and other health measurements which helps to track their health.
2. Users who gained points which can be used to buy products in our App market.
3. The user statistical data can be used to predict users health prior to attack.

## Budget
The project budget includes labor costs, material acquisition and operating costs.


Link to cost estimation: [Cost Estimation](https://github.com/RaviTeja444/health-wellness/blob/master/CostEstimate.xlsx)

![](https://github.com/RaviTeja444/health-wellness/blob/master/costtestimate.PNG?raw=true)


## Roles
| Client  | Dr. Rhonda Beemer  |
|---|---|
| Project Manager  | Ravi Teja Pagidoju  |
| DB Administrator | Gopichand Bhandarupalli |
| Team Lead | Sowjanya Janapatla |
| Full stack Developer | Bhanu Prakash Thota |
| Full Stack Developer | Navya Devineni |
| Full Stack Developer | Sindhu Rani |   


## Evaluation


## JIRA LINK to PROJECT :
[JIRA Link](https://health-wellness.atlassian.net/secure/RapidBoard.jspa?rapidView=1&view=planning.nodetail&selectedIssue=HEAL-3&issueLimit=100)

## Total number of Epics / User Stories / Tasks 
[EPIC Link](https://health-wellness.atlassian.net/browse/HEAL-2).
1. EPIC - 1
2. USer Storys - 23

## Sprint 1(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint1.PNG?raw=true)

## Sprint 2(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint2.PNG?raw=true)

## Sprint 3(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint3.PNG?raw=true)

## Backlog (Future GDP2)
![](https://github.com/RaviTeja444/health-wellness/blob/master/GDP2_BL.PNG?raw=true)

## Acceptance Criteria Sample
![](https://github.com/RaviTeja444/health-wellness/blob/master/Acceptance_Cri.PNG?raw=true)

## Entity Relationship Diagram
![ERD](https://github.com/RaviTeja444/health-wellness/blob/master/GDP1_ERD.png?raw=true)

## Entities Description

1.The following ER Diagram has various tables. Coming to the User table initially user want to login to the Walk tracker he/she needs create an account in the Walk Tracker. For   this, User has to fill out various details in the Walk Tracker App.

2.In the Daily Level table the step count is automatically updated in the APP while user moving.

3.Next, User_Role column in USER table indicates whether a user is admin or not. An admin role user in the USER table can create different Groups and each group has different     group members. Admin can invite various members into the Group so Group member has option to accept or else reject the invitation.All these members are stored in GROUP_MEMBER   Table.

4.Admin can create a CHALLENGE. The  Challenge_Name table have  different challenges, In that user can store challenge created date and lastly Date_LEFT_ACCESSED.Each Challenge   is associated with a Target which is stored in TARGET table. The Target Table is going to stores target description and Target_numerical _Goal. Every Challenge has a Target     based on the Challenge_Id.

5.Finally the User Points is calculated based on step count stored in DAILYLEVEL table. USER_POINTS will have userid and userpoints information.


## Business Rules for the ER Diagram:

1.A certain HEALTH WELLNEESS is interested in storing information about 
  USER,DAILYLEVEL,USER_POINTS,CHALLENGE_NAME,GROUP_MEMBER,GROUP AND TARGET.
  
2.For each USER,The HEALTH WELLNESS would like to store a Unique UserId, EMAIL,USER_NAME,USER_ROLE,PASSWORD,DATE CREATED,DATE_LAST_ACCESSED,HEIGHT,WEIGHT,IS DIABETES,AGE,GENDER.

3.For each GROUP,The Health wellness would like to store a Group unique Id,name,Creator and Date_Created,Date_Last_EDited.

4.FOR each Group_Member, The Health wellness  would like to store a unique GROUP_MEMBER_ID, DATE_INVITED,DATE_ACCEPTED_INVITE,DATE_REJECTED_INVITE,DATE_LEFT_GROUP.

5.FOR each DAILYLEVEL, The HEALTH WELLNES would like to store a unique DAILYLEVEL_ID  UserId,step    count,Hydration_level,Sleep_hours,Fruits_consumed,Calories_consumed,OTHERS,Date_of_measurement                  

6.FOR each USER_POINTS, The HEALTH WELLNESS would like to store a unique USER_POINTS_ID,USER POINTS.

7.FOR each TARGET, The Health wellness would like to store a unique TARGET_ID,TARGET_NAME,TARGET_DESCRIPTION AND TARGET_NUMERICAL_GOAL.

8.FOR each CHALLENGE_NAME, The HEALTH WELLNESS would like to store a unique CHALLENGE_ID CHALLENGE_NAME,designer,date_created,date_last_accessed.

## RELATIONS FOR ER-DIAGRAM:

1.USER(UserId,USER_NAME,USER_ROLE,EMAIL,PASSWORD,DATE CREATED,DATE_LAST_ACCESSED,HEIGHT,WEIGHT,IS DIABETES,AGE,GENDER)

2.USER_POINTS(USER_POINTS_ID,UserId,User_points)
  FK UserId->USER
  
  
3.GROUP(GroupId,NAME,CREATOR,DATE_CREATED,DATE_LAST_EDITED)
  FK CREATOR->USER
  
4.GROUP_MEMBER(GROUP_MEMBER_ID,GroupId,DATE_INVITED,DATE_ACCEPTED_INVITED,DATE_LEFT_GROUP)
  FK GroupId-> GROUP
  
5.DAILYLEVEL(DAILYLEVEL_ID,UserId,step count,Hydration_level,Sleep_Hours,Fruits_consumed,Vegetable_consumed,Calories_consumed,OTHERS,Date_of_measurement)
  FK UserId->USER
  
6.CHALLENGE_NAME(CHALLENGE_ID,UserId,CHALLENGE NAME,DATE_CREATED,DESIGNER,DTAE_LEFT_ACCESSED)
  FK UserId->USER
  
7.TARGET(TARGET_ID,TARGET_NAME,TARGET_DESCRIPTION,CHALLENGE_ID,TARGET_NUMERICAL_GOAL)
  FK CHALLENGE_ID-> CHALLENGE



## Link to Sample Input Data for Database
[Sample Data File](https://github.com/RaviTeja444/health-wellness/blob/master/GDP_Sample_Input_data.xlsx)

## Entities Sample Data


## USER ENTITY TABLE DATA


| UserId | User_NAME | EMAIL                  | PASSWORD   | DATE_CREATED | DATE_LAST_ACCESSED | HEIGHT | WEIGHT | IS DIABETES | AGE | GENDER |
|--------|-----------|------------------------|------------|--------------|--------------------|--------|--------|-------------|-----|--------|
| 101    | Timo      | Müller123@GMAIL.COM    | Greenway   | 11/9/2019    | 1/11/2019          | 5.5    | 60     | YES         | 33  | MALE   |
| 102    | Lias      | Weber123@GMAIL.COM     | Devon12    | 11/8/2019    | 11/9/2019          | 5.6    | 61     | NO          | 34  | MALE   |
| 103    | Gabriel   | Schneider123@GMAIL.COM | Wildwood   | 11/7/2019    | 11/8/2019          | 5.7    | 62     | YES         | 35  | MALE   |
| 104    | Pauline   | Schulz123@GMAIL.COM    | Raven123   | 11/6/2019    | 11/7/2019          | 5.8    | 63     | NO          | 36  | MALE   |
| 105    | Levin     | Schäfer123@GMAIL.COM   | Oxford123  | 11/5/2019    | 11/6/2019          | 5.9    | 64     | YES         | 37  | MALE   |
| 106    | Gabriel   | John123@GMAIL.COM      | Evergreen  | 11/4/2019    | 11/5/2019          | 6      | 65     | NO          | 38  | MALE   |
| 107    | Damian    | Schmidt123@GMAIL.COM   | Ridgeland  | 11/3/2019    | 11/4/2019          | 6.1    | 66     | YES         | 39  | MALE   |
| 108    | Tobias    | Meyer123@GMAIL.COM     | Lexinton   | 11/2/2019    | 11/3/2019          | 6.2    | 67     | NO          | 40  | MALE   |
| 109    | Alina     | Meyer123@GMAIL.COM     | LakeView   | 11/1/2019    | 11/2/2019          | 6.3    | 68     | YES         | 41  | MALE   |
| 110    | Bruno     | Meyer123@GMAIL.COM     | Central123 | 1/9/2019     | 11/1/2019          | 6.4    | 69     | NO          | 42  | MALE   |
| 111    | Lasse     | Meyer123@GMAIL.COM     | Wildwoord  | 1/8/2019     | 1/9/2019           | 6.5    | 70     | YES         | 43  | MALE   |

## USER_POINTS ENTITY DATA


| UserId | USER_POINTS_ID   | User_points  |
| ------ | ---------------- | ------------ |
| 101    | 200              | 50           |
| 102    | 201              | 51           |
| 103    | 202              | 52           |
| 104    | 203              | 53           |
| 105    | 204              | 54           |
| 106    | 205              | 55           |
| 107    | 206              | 56           |
| 108    | 207              | 57           |
| 109    | 208              | 58           |
| 110    | 209              | 59           |
| 111    | 210              | 60           |

## GROUP ENTITY DATA


| GroupId | NAME      | CREATOR | DATE_CREATED | DATE_LAST_EDITED |
| ------- | --------- | ------- | ------------- | ------------------ |
| 201     | Müller    | 101     | 11/9/2019     | 1/11/2019          |
| 202     | Weber     | 102     | 11/10/2019    | 11/9/2019          |
| 203     | Schneider | 103     | 11/11/2019    | 11/8/2019          |
| 204     | Schulz    | 104     | 11/12/2019    | 11/7/2019          |
| 205     | Schäfer   | 105     | 11/13/2019    | 11/6/2019          |
| 206     | John      | 106     | 11/14/2019    | 11/5/2019          |
| 207     | Schmidt   | 107     | 11/15/2019    | 11/4/2019          |
| 208     | Meyer     | 108     | 11/16/2019    | 11/3/2019          |
| 209     | Hoffmann  | 109     | 11/17/2019    | 11/2/2019          |
| 210     | Fischer   | 110     | 11/18/2019    | 11/1/2019          |
| 201     | Wagner    | 111     | 11/19/2019    | 1/9/2019           |

## GROUP_MEMBER DATA


| GROUP_MEMBER_ID   | DATE_INVITED | DATE_ACCEPTED_INVITE    | DATE_REJECTED_INVITE   | GroupId |
| ----------------- | ------------- | ---------------------- | ---------------------- | ------- |
| 301               | 11/9/2019     | 11/9/2019              | 11/10/2019             | 201     |
| 302               | 11/10/2019    | 11/10/2019             | 11/11/2019             | 202     |
| 303               | 11/11/2019    | 11/11/2019             | 11/12/2019             | 203     |
| 304               | 11/12/2019    | 11/12/2019             | 11/13/2019             | 204     |
| 305               | 11/13/2019    | 11/13/2019             | 11/14/2019             | 205     |
| 306               | 11/14/2019    | 11/14/2019             | 11/15/2019             | 206     |
| 307               | 11/15/2019    | 11/15/2019             | 11/16/2019             | 207     |
| 308               | 11/16/2019    | 11/16/2019             | 11/17/2019             | 208     |
| 309               | 11/17/2019    | 11/17/2019             | 11/18/2019             | 209     |
| 310               | 11/18/2019    | 11/18/2019             | 11/19/2019             | 210     |
| 311               | 11/19/2019    | 11/19/2019             | 11/20/2019             | 211     |

## DAILYLEVEL ENTITY DATA


| STEP_COUNT | HYDRATION_LEVEL | Sleep_Hours | Fruits_consumed | Vegetable_consumed | Calories_consumed | Date_of_measurement |
| ----------- | ---------------- | ------------ | ---------------- | ------------------- | ------------------ | --------------------- |
| 2000        | 45               | 6            | 1                | 2                   | 1200               | 11/9/2019             |
| 2002        | 46               | 7            | 2                | 2                   | 1400               | 11/10/2019            |
| 2004        | 47               | 8            | 3                | 3                   | 1400               | 11/11/2019            |
| 2006        | 48               | 6            | 4                | 4                   | 1500               | 11/12/2019            |
| 2008        | 49               | 7            | 5                | 5                   | 1600               | 11/13/2019            |
| 2010        | 50               | 8            | 6                | 1                   | 1700               | 11/14/2019            |
| 2012        | 51               | 8            | 7                | 2                   | 1500               | 11/15/2019            |
| 2014        | 52               | 5            | 8                | 3                   | 1200               | 11/16/2019            |
| 2016        | 53               | 6            | 1                | 4                   | 1100               | 11/17/2019            |
| 2018        | 54               | 7            | 3                | 5                   | 1000               | 11/18/2019            |
| 2020        | 55               | 8            | 4                | 1                   | 1100               | 11/19/2019            |

## CHALLENGE_NAME ENTITY DATA


| DATE_LAST_ACCESSED | UserId |
| -------------------- | ------ |
| 1/11/2019            | 101    |
| 11/9/2019            | 102    |
| 11/8/2019            | 103    |
| 11/9/2019            | 104    |
| 11/10/2019           | 105    |
| 11/11/2019           | 106    |

## TARGET ENTITY DATA


| TARGET_ID  | TARGET_NAME              | TARGET_DESCRIPTION    | TARGET_NUMERICAL_GOAL   |
| ---------- | ------------------------ | --------------------- | ----------------------- |
| 600        | Cycling Challenges       | 10 ROUNDS             | 10                      |
| 601        |  Running Challenges      | RUN 5 MILES           | 5                       |
| 602        | Calories Burned          | 500 CALORIES PER  DAY | 500                     |
| 603        | Healthy Eating Challenge | DIET                  | 1200                    |
| 604        | Walking Challenge        | 10 MILES PER DAY      | 10                      |
| 605        | LUNGE                    | 100 PER DAY           | 100                     |


## Schedule
![Schedule Management](https://github.com/navyadevineni/health/blob/master/Screenshot%20(1).png?raw=true)

## Technology Stack
* Nodejs : Its an open source cross platform javascript runtime environment that executes javascript code without browser.

* HTML : Its an standard markup language used to design pages to display in broswer.

* CSS : Cascading styling sheets helps to style HTML Elements.

* Javascript : Javascript is a programming language gets executed in browser.

* Heroku : Cloud hosting platform to host our PWA in free tier.

* Github : Cloud Repository Platform used to store code
  
## APP_UX Design
[APP LINK](https://www.figma.com/proto/JuWZstQl4XFCJESZAaNcau/Untitled?node-id=92%3A4&scaling=scale-down)

## LogIn Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/Loginpage.png?raw=true)

## Forgot Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/Forgotpasswordpage.png?raw=true)

## Create Account Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/create%20account%20page.png?raw=true)

## Step Count Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/Step%20count%20page.png?raw=true)

## Training Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/Excercise%20page.png?raw=true)

## Account Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/points%20page.png?raw=true)

## ShopByPoints Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/market%20page.png?raw=true)

## Challenges Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/challenge%20page.png?raw=true)

## Settings Page
![](https://github.com/RaviTeja444/health-wellness/blob/master/profile%20settings.png?raw=true)

## DifferentUI_Color
![](https://github.com/RaviTeja444/health-wellness/blob/master/UI_Color.PNG)

## DifferentUI_Home
![](https://github.com/RaviTeja444/health-wellness/blob/master/UI_Home.PNG)

## Risk & Mitigation 
* As we are maintaining health data,we plan for safe and secure database to avoid risk of data loss.
* We maintain high secure Authentication for the users to avoid risk of hacking.

## References
[Google](https://www.google.com/)

## Original RFP Link
[Click Here](https://github.com/cbadami/rfp-health-and-wellness/blob/master/rfp-health-and-wellness.md)





