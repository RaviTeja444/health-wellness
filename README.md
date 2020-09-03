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

![](https://github.com/RaviTeja444/health-wellness/blob/master/costestimate.PNG?raw=true)


## Roles
| Client  | Dr. Rhonda Beemer  |
|---|---|
| Project Manager  | Ravi Teja Pagidoju  |
| DB Administrator | Gopichand Bhandarupalli |
| Team Lead | Sowjanya Janapatla |
| Quality Assurance Analyst | Bhanu Prakash Thota |
| Backend Developer | Navya Devineni |
| Front End Developer | Sindhu Rani |   


## Evaluation


## JIRA LINK to PROJECT :
[JIRA Link](https://health-wellness.atlassian.net/secure/RapidBoard.jspa?rapidView=1&view=planning.nodetail&selectedIssue=HEAL-3&issueLimit=100)

## Total number of Epics / User Stories / Tasks 
[EPIC Link](https://health-wellness.atlassian.net/browse/HEAL-2).
1. EPIC - 1
2. USer Storys - 23

## Story Points :
According to the acceptance criteria of each story,assigned the story points accordingly.Example of one user story screenshot is shown below.

![](https://github.com/RaviTeja444/health-wellness/blob/master/StoryPoints.PNG?raw=true)

## Sprint 1(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint1.PNG?raw=true)

## Sprint 2(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint2.PNG?raw=true)

## Sprint 3(GDP1)
![](https://github.com/RaviTeja444/health-wellness/blob/master/mySprint3.PNG?raw=true)

## Testing User Story
![](https://github.com/RaviTeja444/health-wellness/blob/master/Testing_UserStory.PNG?raw=true)

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

| UserId | User_NAME  | EMAIL                  | PASSWORD     | DATE_CREATED  | DATE_LAST_ACCESSED   | HEIGHT | WEIGHT | IS DIABETES | AGE | GENDER |
| ------ | ---------- | ---------------------- | ------------ | ------------- | -------------------- | ------ | ------ | ----------- | --- | ------ |
| 101    | Timo       | Timo123@GMAIL.COM      | Greenway     | 11/9/2015     | 1/11/2015            | 5.5    | 60     | YES         | 33  | MALE   |
| 102    | Lias       | Lias123@GMAIL.COM      | Devon12      | 11/10/2015    | 1/12/2015            | 5.6    | 61     | NO          | 34  | MALE   |
| 103    | Gabriel    | Gabriel123@GMAIL.COM   | Wildwood     | 11/11/2015    | 1/13/2015            | 5.7    | 62     | YES         | 35  | MALE   |
| 104    | Pauline    | Pauline123@GMAIL.COM   | Raven123     | 11/12/2015    | 1/14/2015            | 5.8    | 63     | NO          | 36  | MALE   |
| 105    | Levin      | Levin123@GMAIL.COM     | Oxford123    | 11/13/2015    | 1/15/2015            | 5.9    | 64     | YES         | 37  | MALE   |
| 106    | Gaabriel   | Gaabriel123@GMAIL.COM  | Evergreen    | 11/14/2015    | 1/16/2015            | 6      | 65     | NO          | 38  | MALE   |
| 107    | Damian     | Damian123@GMAIL.COM    | Ridgeland    | 11/15/2015    | 1/17/2015            | 6.1    | 66     | YES         | 39  | MALE   |
| 108    | Tobias     | Tobias123@GMAIL.COM    | Lexinton     | 11/16/2015    | 1/18/2015            | 6.2    | 67     | NO          | 40  | MALE   |
| 109    | Alina      | Alina123@GMAIL.COM     | LakeView     | 11/17/2015    | 1/19/2015            | 6.3    | 68     | YES         | 41  | MALE   |
| 110    | Bruno      | Bruno123@GMAIL.COM     | Central123   | 11/18/2015    | 1/20/2015            | 6.4    | 69     | NO          | 42  | MALE   |
| 111    | Lasse      | Lasse123@GMAIL.COM     | Wildwoord    | 11/19/2015    | 1/21/2015            | 6.5    | 70     | YES         | 43  | MALE   |
| 112    | Aaron      | Aaron123@GMAIL.COM     | Aaron222     | 11/20/2015    | 1/22/2015            | 5.5    | 60     | YES         | 33  | MALE   |
| 113    | Abagnale   | Abagnale123@GMAIL.COM  | Abagnale222  | 11/21/2015    | 1/23/2015            | 5.6    | 61     | NO          | 34  | MALE   |
| 114    | Abbey      | Abbey123@GMAIL.COM     | Abbey222     | 11/22/2015    | 1/24/2015            | 5.7    | 62     | YES         | 35  | MALE   |
| 115    | Abel       | Abel123@GMAIL.COM      | Abel222      | 11/23/2015    | 1/25/2015            | 5.8    | 63     | NO          | 36  | MALE   |
| 116    | Abelson    | Abelson123@GMAIL.COM   | Abelson222   | 11/24/2015    | 1/26/2015            | 5.9    | 64     | YES         | 37  | MALE   |
| 117    | Abourezk   | Abourezk123@GMAIL.COM  | Abourezk222  | 11/25/2015    | 1/27/2015            | 6      | 65     | NO          | 38  | MALE   |
| 118    | Abrams     | Abrams123@GMAIL.COM    | Abrams222    | 11/26/2015    | 1/28/2015            | 6.1    | 66     | YES         | 39  | MALE   |
| 119    | Ace        | Ace123@GMAIL.COM       | Ace222       | 11/27/2015    | 1/29/2015            | 6.2    | 67     | NO          | 40  | MALE   |
| 120    | Acton      | Acton123@GMAIL.COM     | Acton222     | 11/28/2015    | 1/30/2015            | 6.3    | 68     | YES         | 41  | MALE   |
| 121    | Addison    | Addison123@GMAIL.COM   | Addison222   | 12/7/2015     | 2/8/2015             | 6.1    | 66     | YES         | 39  | MALE   |
| 122    | Adorno     | Adorno123@GMAIL.COM    | Adorno222    | 12/8/2015     | 2/9/2015             | 6.2    | 67     | NO          | 40  | MALE   |
| 123    | Adler      | Adler123@GMAIL.COM     | Adler222     | 12/9/2015     | 2/10/2015            | 6.3    | 68     | YES         | 41  | MALE   |
| 124    | Aeschylus  | Aeschylus123@GMAIL.COM | Aeschylus222 | 12/10/2015    | 2/11/2015            | 6.4    | 69     | NO          | 42  | MALE   |
| 125    | Aesop      | Aesop123@GMAIL.COM     | Aesop222     | 12/11/2015    | 2/12/2015            | 6.5    | 70     | YES         | 43  | MALE   |
| 126    | Affleck    | Affleck123@GMAIL.COM   | Affleck222   | 12/12/2015    | 2/13/2015            | 5.5    | 60     | YES         | 33  | MALE   |
| 127    | Agena      | Agena123@GMAIL.COM     | Agena222     | 12/13/2015    | 2/14/2015            | 5.6    | 61     | NO          | 34  | MALE   |
| 128    | Agnew      | Agnew123@GMAIL.COM     | Agnew222     | 12/14/2015    | 2/15/2015            | 5.7    | 62     | YES         | 35  | MALE   |
| 129    | Ahbez      | Ahbez123@GMAIL.COM     | Ahbez222     | 12/15/2015    | 2/16/2015            | 5.8    | 63     | NO          | 36  | MALE   |


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
| 112    | 211              | 61           |
| 113    | 212              | 62           |
| 114    | 213              | 63           |
| 115    | 214              | 64           |
| 116    | 215              | 65           |
| 117    | 216              | 66           |
| 118    | 217              | 67           |
| 119    | 218              | 68           |
| 120    | 219              | 69           |
| 121    | 220              | 70           |
| 122    | 221              | 71           |
| 123    | 222              | 72           |
| 124    | 223              | 73           |
| 125    | 224              | 74           |
| 126    | 225              | 75           |
| 127    | 226              | 76           |
| 128    | 227              | 77           |
| 129    | 228              | 78           |





## GROUP ENTITY DATA


| GroupId | NAME      | CREATOR | DATE_CREATED  | DATE_LAST_EDITED   |
| ------- | --------- | ------- | ------------- | ------------------ |
| 201     | Müller    | 101     | 11/12/2017    | 12/11/2017         |
| 202     | Weber     | 102     | 11/13/2017    | 12/12/2017         |
| 203     | Schneider | 103     | 11/14/2017    | 12/13/2017         |
| 204     | Schulz    | 104     | 11/15/2017    | 12/14/2017         |
| 205     | Schäfer   | 105     | 11/16/2017    | 12/15/2017         |
| 206     | John      | 106     | 11/17/2017    | 12/16/2017         |
| 207     | Schmidt   | 107     | 11/18/2017    | 12/17/2017         |
| 208     | Meyer     | 108     | 11/19/2017    | 12/18/2017         |
| 209     | Hoffmann  | 109     | 11/20/2017    | 12/19/2017         |
| 210     | Fischer   | 110     | 11/21/2017    | 12/20/2017         |
| 211     | Wagner    | 111     | 11/22/2017    | 12/21/2017         |
| 212     | Maathai   | 112     | 11/23/2017    | 12/22/2017         |
| 213     | MacArth   | 113     | 11/24/2017    | 12/23/2017         |
| 214     | Macaula   | 114     | 11/25/2017    | 12/24/2017         |
| 215     | Macdona   | 115     | 11/26/2017    | 12/25/2017         |
| 216     | MacGreg   | 116     | 11/27/2017    | 12/26/2017         |
| 217     | Machado   | 117     | 11/28/2017    | 12/27/2017         |
| 218     | Machiav   | 118     | 11/29/2017    | 12/28/2017         |
| 219     | Madonna   | 119     | 11/30/2017    | 12/29/2017         |
| 220     | Madraiw   | 120     | 12/1/2017     | 12/30/2017         |
| 221     | Magee     | 121     | 12/2/2017     | 12/31/2017         |
| 222     | Maharaj   | 122     | 12/3/2017     | 1/1/2018           |
| 223     | Mahavir   | 123     | 12/4/2017     | 1/2/2018           |
| 224     | Maher     | 124     | 12/5/2017     | 1/3/2018           |
| 225     | Malcolm   | 125     | 12/6/2017     | 1/4/2018           |
| 226     | Malda     | 126     | 12/7/2017     | 1/5/2018           |
| 227     | Mallet    | 127     | 12/8/2017     | 1/6/2018           |
| 228     | Malley    | 128     | 12/9/2017     | 1/7/2018           |
| 229     | Malory    | 129     | 12/10/2017    | 1/8/2018           |


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





