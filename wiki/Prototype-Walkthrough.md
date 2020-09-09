## Introduction
The paper prototypes were created and iterated on during the second stage of the project. The hypothesis, that is areas for investigation were borne out of the research, specifically the pain points and opportunities for a new system.

From the user mapping exercise carried out in the research phase, the team identified that the SOR could be broken down into three main areas/stages:
- Looking up SORs for editing/viewing/printing
- The data entry - the actual editing or creating of a new SOR.
- Distribution of the SOR and how this could feed into rota creation

The primary focus during prototyping has been on the data entry stage, as it was decided that this is where the greatest pain and opportunities lie. The looking up (stage one) and distribution (stage three) were also touched on during interviews. The main recommendations are around the entering of data and what could be captured to provide a clearer picture of a plant's profile and the abstract resources.

## Hypotheses and findings
- By removing person specific information from the SOR we will build an accurate picture of the plant and the resources needed. The information entered into the SOR should be employee agnostic that is, not capturing if a plant will have permanent FSA or contract staff or specific individual's working arrangements.
We found through our research that the SOR has grown out to a point where it is being used partly as a resource requirement and partly as a personnel planner.
  
  > Feedback: This is a key part of the vision we are trying to sell, and has been a difficult concept for user's to grasp as it is quite different to the process they are currently following. The personalised pieces of information should be coming at a rota creation level, not a resource requirement level.
- Adding a naming option for the SOR versions will make it easier to search for files and give options for templating. This could have a wider impact on forcasting as data could be analysed around specific periods of time. This could also encourage more regular updates to SORs therefore improving accuracy.
  
  > Feedback: Very positive. Users thought this would be a good idea.
- The SOR does not need discount information as a text box. Our findings show that ITLs creating SORs do not use the discounts box.
  
  > Feedback: Very positive. Users agreed that the discount text box should be removed. The rules around the discounts can be automated by the system, we know the business logic that calculates the discounts therefore we can apply them in this way. Alternatively, discounts could be removed entirely from the SOR and displayed to the FBO when they are given a final bill.
- Having a single "main" SOR and temporary SORs will encourage more frequent updates, and will provide a more accurate picture of seasonal changes. We know that users find it frustrating to create new SORs. We believe that allowing them to switch to a temporary SOR and back to a "business as usual" SOR will make finding the current and recent SORs clearer. This should be coupled with naming temporary SORs too.
  
  > Feedback: Positive. There will need to be further work on how to get this across to users, however once they had been reassured that there would always be a main SOR to switch back to they generally accepted this idea.
- Consolidating hours vs activities is difficult - a visual tool could make this easier.
  
  > Feedback: Positive. Users all said that having the visual cue of how many hours they had left to assign would make this easier. Strongly recommend a visual approach to this over text.
- The language around start and end times is confusing, user do not seem to be clear on what these times apply to throughout the system.
  > Feedback: More work to do during alpha. We have experimented with various naming conventions and still found there to be confusion. Users do agree that the language is confusing. Introducing the premesis opening and closing hours caused further confusion, however I believe this could be due to them approaching the prototypes in the same mindset of the current SOR rather than looking at this a new. Again, training and documentation will be key to this.
  
  > Further feedback showed that changing wording to say "Estimated" for throughput and line speed would be beneficial.
- Business rules to calculate if FBO should be charged for overtime. We know there are specific rules (and quite a lot of them) when it comes to calculating this, for example working unsociable hours. Once the user has gone through and entered all the other details for the SOR like line speed, species and everything, the system could  perform calculations and notify you that there will likely be overtime involved.
  
  > Feedback: Very positive. Removes the cognitive load on the user, would allow less experienced ITLs to complete SORs more accurately.

Within the data entry stage we believe that breaking this down into clearer sections would benefit the completion.
1. Plant information - Days and hours of premisis operation, species, **inspection points on site**, rotation staff needed
2. Data to build up a picture of each day of work
3. Activities to be carried out
4. Feedback around any additional charges based on the information given
5. Sign-off, audit capture and distribution

## Walkthrough

### Context

Our research shows that SORs are usually updated based on time periods (e.g. religious holidays where production will be higher) and rarely are they created from scratch as new plants coming online is a infrequent event. The scenario we presented to users was that of a Christmas period where the FBO wants to increase the through put.

For this walkthrough, the user wants to create a new SOR based on the Christmas period. They have selected the main line SOR to create a new copy from.

[Slideshow walkthrough.](https://docs.google.com/presentation/d/1FrA8BptNLlrluDhEzBRt7C_6nIUPuBfeReyjyxIH2hw/edit?usp=sharing)

### Section 1A - SOR information

#### Page 1

[![FBO and SOR information](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%201%20-%20FBO%20and%20SOR%20information.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%201%20-%20FBO%20and%20SOR%20information.jpeg)

* The new SOR is given an ID by the system.
* The user enters a unique name for reference purposes, in this case XMAS TEMP 2019.
* They have indicated this is a temporary change. At all times there will be a permanent SOR available. The temporary option allows this "mainline" to not be lost and so be easily and quickly reverted to after a period of time. This can be thought of like the daylight savings switch on a clock.
* The SOR is given an effective from date, once this date is reached it will automatically be switched to. The review date for the SOR will be set 6 months automatically for permanent changes and a custom period of time for temporary.
Having the review date may encourage ITLs to update SORs more regularly. Once this date is close, it is envisaged that the system will notify the ITL automatically via email and/or system notification.

### Section 1B - Plant information

#### Page 1

* Entering the plant approval number will result in the name and type being filled from the database.

#### Page 2

[![Plant operating details](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%202%20-%20Plant%20operating%20details.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%202%20-%20Plant%20operating%20details.jpeg)

- This page contains the plant operating details. We are asking for quite high level information at this point.
  The first questions are asked to set up if the user needs to set different times for each day or if each day is fairly regular in operation. For all the inputs that occur for everyday of operation, the table at the bottom of the page will be automatically filled in. **All inputs will always be editable by the user.**
- The user is asked to input the open and close times per day. This is the premises open and close times rather than production line working times, it is the times that FSA staff can get onto the site and when it site closes for the day. We include this information to build up a plant profile that could then be used for forecasting and other operational purposes. 
  _Research with the Service Delivery Partner showed that they have comprehensive plant profiles full of useful information that the FSA does not have._
  Ticking the box will then show the open close inputs.
- Again, in order to build up a plant profile, we ask for the number of production lines in use at the same time.
- And the same again for the number of shifts.
- The table at the bottom of the page will have filled up with any information entered above. Alternatively the user can manually fill and tick all the required cells of the table:
  - Tick days of operation
  - Opening time
  - Closing time
  - Shifts per day
  - Production line

It should be noted that as information about the plants is built up, this information can be brought in from a database.

#### Page 2A - Species processed

The user selects the species to be processed. They can add multiple if needed. In the future this information can come from a database.


[![Single species inspection points](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%203_1%20-%20Single%20Species%20Cattle.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%203_1%20-%20Single%20Species%20Cattle.jpeg)

* The user enters the number of inspection points for each species and the number of rotation staff needed. This information will allow FSA to build up a detailed plant level view of resources needed on a national scale.
#### Page 2B - Species processed
Example of entering another species for the plant.

[![Multi-species inspections points](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%203_2%20-%20Species%20Pigs.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%203_2%20-%20Species%20Pigs.jpeg)

### Table views for daily workload.
A table view of weekly resource patterns is then generated from the information entered (species, shifts, production lines and inspection points). The system can use business logic to calculate how many inspectors and vets are required based on the species, lines in use at once and inspection points.
The user will then enter the start and end times for the kill. This deliberately does not take into account whether the plant will be using permanent or contract staff. Nor does it need to record the extra 30 minutes at the start of a shift that the vets require. 

It is this idea of the SOR being decoupled from rota planning and used as a statement of what the plant will need.

The feedback suggested that users could struggle with this concept and so a clear guide and comprehensive training to change user approach to the data entry will be required. 

There will be one table for multiple species.

[![Single species, single shift, single production line](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20shift%20and%20line.png)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20shift%20and%20line.png)

_Single species, single shift, single production line_


[![Single species multi-shift, single production line](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20multi%20shift%20single%20lines.png)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20multi%20shift%20single%20lines.png)
_Single species, multi-shift, single production line_


[![Single species, single shift, multi-production line](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20single%20shift%20multi%20lines.png)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Single%20species%20single%20shift%20multi%20lines.png)
_Single species, single shift, multi-production line_


[![Multi-species, single shift, single production line](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Multispecies%20single%20shift%20and%20line.png)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Multispecies%20single%20shift%20and%20line.png)
_Multi-species, single shift, single production line_


[![Multi-species, multi-shift, multi production line](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Multi%20species%20multi%20shift%20single%20line.png)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Multi%20species%20multi%20shift%20single%20line.png)
_Multi-species, multi-shift, multi production line_

### Section 3 - Activity hours
#### Page 5_1
Activities will be shown per species and broken down into role below the species.

[![Activity hours](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205%20-%20Activity%20hours.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205%20-%20Activity%20hours.jpeg)

The system can use business logic to present the activities that each role will need to carry out daily. The system can know this as inspectors will need to do certain jobs for instance. 

After consulting the subject matter experts, we do not believe that these hours can be automatically calulated. We also know from the research that this hours vs activities consolidation caused problems for users. 

We recommend that a graphical interface is used to alleviate this. As the users enter hours against activities the bar fills up, this should make it easier to set the hours required over a day.

#### Page 5_2
For any activities that are ad-hoc per month or week they can be stated along with estimated hours.
[![Monthly activities](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_2%20-%20Monthly%20activities.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_2%20-%20Monthly%20activities.jpeg)

[![Species activity hours](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_2%20-%20Pig%20activity%20hours.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_2%20-%20Pig%20activity%20hours.jpeg)

[![Species activity hours](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_3%20-%20Pig%20activity%20hours.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%205_3%20-%20Pig%20activity%20hours.jpeg)


### Section 4 - Sign-off and distribution
#### Page 6
Based on the information entered, the system will then flag to the FBO/ITL any potential extra charges that the SOR may create along with solutions on how to fix these problems, eg, unsociable hours based on shift production start and end times between X and Y hours.

[![Possible charges](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%206%20-%20Charges.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%206%20-%20Charges.jpeg)

If no extra charges are likely this step will be skipped.

#### Page 7
The FSA user filling out the SOR will enter their SP number; populating their name and role. And enter the sign off date.

[![Sign and distribute](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%207%20-%20Sign%20off%20and%20distribute.jpeg)](uploads/prototypes/sor/Version%202.X/Version%202.8%20-%20Final/Version%202.8%20-%20Page%207%20-%20Sign%20off%20and%20distribute.jpeg)

User research informed us that most users did not keep digital records of signed off SORs and so we have added functionality to scan/take a photo and upload the image to a central database - this will create an audit trail.

The user can then save as a final version, print out or email the SOR to relevant people. To remove the problem of multiple versions being in email chains the system will email a link to a centralised SOR that can be printed. All discussions and work should be carried out in the system to ensure accurate record keeping for the SORs.