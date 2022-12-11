# Overview

The below is a technical backbone for instantiation of an algorithm that we believe should supplant the current system for congressional re-districting. We outline a process that:

- Begins with the generation of random seeds generated using a quantum computer
- Draws congressional districts having a minimum perimeter to area (P/A) ratio
- Is blind to the location of demographic information such as the current (or projected) addresses of registered voters nationwide 
- Is impractically difficult to influence (even by a skilled, malicious attacker with a partisan agenda) despite being running deterministically and in polynomial time

In summary, we report a system for Congressional Redistricting that may aptly be described as "robust to partisanship" or "unbiased" or "agnostic" or "fair".

As evidence of this, we submit detailed output and diagnostics on the generation of congressional districts N = 10,000,000 (10 millon) times. These data show that this algorithm draws districts in a way that best reflects the will of the American people.

# Congressional Districting
Population per seat (Total of 435 congressional districts s/p fixation in 1929 {see below}).
States typically redraw district boundaries after each census, with the changes being submitted to POTUS by 9 months after completion of the Census and taking effect 3 years after the completion thereof.
Each state determines its own district boundaries, either through legislation or through non-partisan panels. 

## State-Level Electoral Systems:
Elections for representatives are held in every even-numbered year, on Election Day the first Tuesday after the first Monday in November. 
Pursuant to the Uniform Congressional District Act, representatives must be elected from single-member districts. 
After a census is taken (in a year ending in 0), the year ending in 2 is the first year in which elections for U.S. House districts are based on that census (with the Congress based on those districts starting its term on the following January 3). 
As there is no legislation at the federal level mandating one particular system for elections to the House, systems are set at the state level. 
As of 2022, so-called "first-past-the-post" i.e., plurality voting is adopted in 46 states
Ranked-choice or "instant-runoff" voting in two states (Alaska and Maine).
The two-round system in two states (Georgia and Mississippi). 

## Apportionment 
Roughly, the process of dividing territory to result in roughly equally populated districts within each state as a function of time.
1787: Article I, Section 2 of the US Constitution Establishes the initial ratio of representatives to citizens set not to exceeed 1 : 30000 citizens, though each state must have at minimum 1 Representative.
1790: Congress enacts the ________ Act, specifying changes in the number of representatives.
1870: Amendment XV, Sction 2: Representatives shall be apportioned among the several States according to their respective numbers, counting the whole number of persons in each State ... 
1920: The US House of Representatives fails to reapportion itself after the 1920 Census.
1929: The Permanent Apportionment Act becomes law, fixing the number of representatives at 435. From this point forward, the number of citizens represented by each congressperson changes Census-to-Census. https://history.house.gov/Historical-Highlights/1901-1950/The-Permanent-Apportionment-Act-of-1929/, DoA 22 December 2022.

## Reapportionment
Presently the U.S. Census Bureau must deliver the results of a decennial census to the President of the United States within nine months of the census date (as per https://history.house.gov/Institution/Apportionment/Reapportioning/; DoA: 10 Dec 2022).. Within a week of the opening of the next Congress, the President is required by law to report the census results to Congress. 
Within 15 days, the Clerk must then disclose to the governor of each state how many seats his or her state is entitled. 
The state legislatures are charged with redrawing a state’s congressional districts. 
Apportionments take effect two Congresses (three years) after the last census 
An apportionment data time series published by the US Census Bureau may be viewed here: https://www.census.gov/data/tables/time-series/dec/apportionment-data-text.html DoA: 10 December 2022 (see https://www.visitthecapitol.gov/sites/default/files/documents/resources-and-activities/CVC_HS_ActivitySheets_CongApportionment.pdf).
Legal precedent following from Wesberry v. Sanders holds that it is unconstitutional for congressional districts to be unequal in population. 
Specifically, in Wesberry v. Sanders the US Supreme Court ruled that malapportionment, or the failure to guarantee equivalent numbers of citizens per district, is unconstitutional and districts must be approximately equal in population (see Wesberry v. Sanders). 

## The Voting Rights Act of 1965:
Section 2 of the Voting Rights Act of 1965 prohibits redistricting plans that are intended to, or have the effect of, discriminating against those in the minority due to race or language spoken.
However, apart from these basic protections (against malapportionment and against discrimination against racial or language minorities) *federal courts have allowed state legislatures to engage in gerrymandering to benefit political parties or incumbents.*
In a 1984 case, Davis v. Bandemer, the Supreme Court held that gerrymandered districts could be struck down based on the Equal Protection Clause, but the Court did not articulate a standard for when districts are impermissibly gerrymandered. 

## Status Quo Under the Current System
According to calculations made by Burt Neuborne using criteria set forth by the American Political Science Association, about 40 seats, **less than 10% of the House membership, are chosen through a genuinely contested electoral process, given partisan gerrymandering.**
Our simulations show ____________________.

# Data Sources:

## The US Census Bureau:
- Decennial Census Data (1910-2020): https://www.census.gov/programs-surveys/decennial-census/data/tables.html
- Population Change Data (1910-2020): https://www.census.gov/data/tables/time-series/dec/popchange-data-text.html
- Population Density Data (1910-2020): https://www.census.gov/data/tables/time-series/dec/density-data-text.html
- Historical apportionment Data https://www.census.gov/library/visualizations/interactive/historical-apportionment-data-map.html 

## Population Data (according to the 2020 US Census):
[Note, move this to a flat file or take the information from an API call in the future].

State Populations:
- Alaska	
- Alabama	
- ...

Total (i.e., National) Population:


## Population Density Data
In order to write software capable of Redistricting according to the principles enumerated above, it is necessary to have highly accurate information regarding population density nationwide, in addition to the total counts listed above.
As present congressional districting is based on data published decenially by the US Census Bureau. We follow this precedent; additionally we will issue as output results from our simulations in all conventional file formats (i.e. ______________________).

## Conventional File Formats for storing Congressional Districting specifications:
Obtain Precise ___File of Congressional Districts https://www.census.gov/programs-surveys/geography/guidance/geo-areas/congressional-dist.html


# High-Level Overview of the Algorithm

0. Note that a line is defined as the shortest distance between two points, and that on a curved surface the shortest such line is itself curved (link to proof).
1. There is a closed-form mathematical proof that 3 points specify a circle on a plan uniquely (link to proof).
2. It can also be shown that 2 fixed points (separated by a distance l) and a fixed radius, r (where r is greater than or equal l) specify 2 unique circles (1 if r == l). 
3. However, if r is allowed to vary freely, an infinite number of circles may be constructed that passes through both points. 
4. It can further be shown (need to write this) that if the population density of a geographical area is known with a high degree of precision, a subset of these circles will divide the population of a 2-district state into exactly equal portions.
5. A proof-by-induction suffices to further demonstrate this for 3-, 4-, and N-district geographical areas may be divided without violating the mandate of equal apportionment set forth in Article 1 Section 2 of the United States Constitution.
6. The use of a random number generator that outputs random binary strings may be used to specify points within each state, enabling agnostic, unbiased congressional re-districting without violating the mandate for equal apportionment.

# Selection of a Random Number Generator:
Generally, we favor random number generators having:
- Very high information entropy, e.g. quantum RNGs
- During the trial period, ideally the machine generating the random output is housed off of US Soil; afterwards, preferably the reverse.
- Have an API
- Implement a variety of output formats
The QRNG@ANU JSON API supports three parameters; please see: https://qrng.anu.edu.au/contact/api-documentation/ (DoA: 10 December 2022).

## Examples of the use of QRNG@ANU:
Requesting 10 random numbers between 0–255 (https://qrng.anu.edu.au/API/jsonI.php?length=10&type=uint8).
Requesting 5 random numbers between 0–65535 (https://qrng.anu.edu.au/API/jsonI.php?length=5&type=uint16)
Requesting 10 blocks of random numbers in hexadecimal format. Each block is between 0000–ffff (https://qrng.anu.edu.au/API/jsonI.php?length=10&type=hex16&size=2#).
