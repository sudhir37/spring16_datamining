Exploring Disruption in Transportation: Car sharing, Peer-to-Peer Car Rental and Cars-for-hire and What Open Data Is Telling Us
=============

# OVERVIEW
You don't have to look very far to find a fascinating statistic about car ownership and driving trends in the US: that [the number of driver's getting licensed *by the time they are of eligible age* is declining](http://www.washingtonpost.com/local/trafficandcommuting/fewer-teens-get-drivers-licenses/2013/07/31/60a32aae-f9c7-11e2-a369-d1954abcb7e3_story.html), and in fact at a four decade low. Upon first reading this, one  might be compelled to think back to their High School days, when you couldn't wait to learn how to drive.  Getting a driver's license was a rite of passage and access to many new 'almost adult' freedoms:  you could drive yourself to school, work and to take your dates to the movies **without** getting a ride from your parents or older siblings. And depending on your age, gas was well under $1/gallon, insurance rates much cheaper, the cost of a decent used car within reach of a minimum wage job and [graduated driver's license (GDL) laws](http://en.wikipedia.org/wiki/Graduated_driver_licensing#United_States) were still beginning to roll out.

Disruption is going on in car sharing ([OccassionalCar](http://carshare.org/tag/occasional-car/) (which was purchased by [Enterprise](http://carshare.org/occasional-car-sells-to-enterprise/)), [ZipCar](http://www.zipcar.com/), etc.), peer-to-peer car rental ([RelayRides](http://www.relayrides.com/), [Getaround](http://blogs.wsj.com/venturecapital/2014/11/20/car-sharing-company-getaround-fuels-up-at-200-million-valuation/), etc.), and of course cars-for-hire ([Uber](https://www.uber.com/), [Lyft](http://www.lyft.com/), etc.).  With so much interest and money getting poured into funding these startups, one must wonder about the marketplaces emerging and ultimately who will become the consumers of these products and why.  Of course, without having direct knowledge of the internals of these companies and the data they've already collected about market trends and dynamics, we're only left with the data that is readily available.  This project will explore  and try understand __the data-driven case for who possible consumers of these products are__. In this project we will :

* explore open transportation data the may give support to and evidence for the growth of the transportation disruption occuring in the US,
* provide the analyses that may demonstrate and give support to this disrpution with attention to the characteristics of the data that might help us understand the local and regional trends and phenomenon in transportation.

# DATA


All of the data will be obtained from the US government census and transportation datasets maintained at:

* Transportation : [Bureau of Transportation Statistics](http://www.rita.dot.gov/bts/data_and_statistics/databases)
* Census : [http://census.gov/data/developers/data-sets.html](http://census.gov/data/developers/data-sets.html)


All of the data is either in CSV or Microsoft Excel format that will make it easy to convert in any analysis performed later.  Python / Jupyter Notebooks will be used to do the data analysis.


# RESEARCH QUESTIONS
Describe the core questions you will be pursuing within the project.  These questions will lead the reader to your interest in the data and provide the bridge between your motivation and analysis.  

While it is clear that Uber and others have tapped into a market that has a clear need, from the outside there are a number of questions, not only about *who is driving*, but *who is consuming the service*.  Thus, the research questions will be split into two categories.

## Who is Driving?
If the numbers are true that licensure of drivers is declining, who then is driving for Uber.  Thus, the research questions will explore:

Without a license one can't drive, and in fact drivers under 21 are not eligible to drive for Uber (older for other services), so :

* Does the license and transportation data show evidence to suggest which age groups are likely to be a driver for services like Uber?
* With car ownership rates also down, what does the data suggest about who might be likely drivers?
* Is there any evidence from Uber sources to suggest either of these to be true?

## Who is Consuming?
Taking a look at car "ownership" from two angles, vehicle registration and car sales demographics, the research questions will explore the other side of the analysis.  If there are fewer licensed drivers, we might expect a drop in vehicle registrations (for example, if one doesn't own a vehicle then there is no need to pay for registration).  The national registration rate of "private vehicles" (including cabs) to public and commercial vehicles, has remained a robust 98.3% from 2007-2012.

* What predictions can be made from _public_ data about who is using Uber and similar services?
* If the registration rates are stable, how is Uber going to grow their market?  Do regional dynamics or demographics play a role in such growth?
* How much does car ownership factor into _affordability_ of services likely to be used by consumers?  That is, with lower transportation costs (no car payment, no registration, no maintenance/fuel costs) what would we predict for the various segments of these services (car sharing/rental vs ride sharing/pickup).

## Economic Context
With 2007-2009 being  very bad years for the car industry during [The Great Recession](http://www.bls.gov/spotlight/2012/recession/pdf/recession_bls_spotlight.pdf), we can expect a drop in car sales, but what support is in the rest of the data we've got so far?

* How much are economic characteristics shaping the uptake of services like Uber and car sharing?
* Are there predictors that can be found and explored in data sources?  
* The cost of car ownership includes fuel, insurance, maintenance, etc.  How do the changes in these costs relate to the changes in fuel may influence the decision to use these services that are now becoming more popular?  Are there models that might help us make predictions based on the economics of car ownership?
  

# MODELS AND ANALYSIS

What models did you use to process your data and perform the analysis of your research questions?  

Describe your methods and how you applied your models to the data.  


# CODE AND APPLICATION

For your application you will be writing code.  Please make sure your group:

- provides the Github link to your code,
- provides detailed instructions on how to compile and deploy your code,
- provides any special instructions for running your code and/or applying data to see the results.

The code needs to be Github and instructions on installation are in the README.md file at the root level.

# PROJECT MANAGEMENT

You will need to provide details on:

- the team members,
- the roles of each member,
- the skills and contributions of each member.

You will also provide details about the project deliverables and milestones.  These example tables should be used as a guide.

# PROJECT TEAM, DELIVERABLES AND CHECKPOINTS
These tables show  examples of the data that should go into each column and row.


## TEAM

| Team member | Roles and skills | Contributions |
|-------------|-------------------------|---------------------------------------------|
| MEMBER NAME | What will they do in the project?  What skills do they bring?  What interests will they explore? | Fill the contributions in when the deliverables have been completed and you have results to report.  These can be summarized, but the intent is that this will allow an easy way to see who did what. |
| MEMBER #2 NAME | -- | -- |
| MEMBER # _N_ NAME | -- | -- |

## DELIVERABLES AND CHECKPOINTS

The deliverable and checkpoints will be iteratively completed.  At the end of the project, there should be a fair amount of content these tables that details the who, what and when of your project.  Don't worry if you don't have all the deliverables sketched out -- this is a LIVING table, and should be updated frequently by all team members involved in the project.

| Checkpoint date | Expected Deliverable                                                          | Responsible team member(s) | Checkpoint results                                                                                                                  |
|---------------|-------------------------------------------------------------------------------|----------------------------|-------------------------------------------------------------------------------------------------------------------------------------|
|WHEN | What will be delivered?  These should be small enough tasks to complete in the time given and large enough to represent some complexity. | Who will delivery this?    | WHAT WERE THE RESULTS?  FILL THIS IN AFTER THE CHECKPOINT HAS PASSED! |
|     ...          | -- | --                    |  -- |