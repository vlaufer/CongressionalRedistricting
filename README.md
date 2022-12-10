
#### Relevant History:

## Congressional Districting
# Population per seat (Total of 435 congressional districts s/p fixation in 
# States typically redraw district boundaries after each census, though they may do so at other times, such as the 2003 Texas redistricting. 
# Each state determines its own district boundaries, either through legislation or through non-partisan panels. 

## Apportionment 
# Roughly, the process of dividing territory to result in roughly equally populated districts within each state as a function of time.
# 1787: Article I, Section 2 of the US Constitution Establishes the initial ratio of representatives to citizens set not to exceeed 1 : 30000 citizens, though each state must have at minimum 1 Representative.
# 1790: Congress enacts the ________ Act, specifying changes in the number of representatives.
# 1870: Amendment XV, Sction 2: Representatives shall be apportioned among the several States according to their respective numbers, counting the whole number of persons in each State ... 
# 1920: The US House of Representatives fails to reapportion itself after the 1920 Census.
# 1929: The Permanent Apportionment Act becomes law, fixing the number of representatives at 435. From this point forward, the number of citizens represented by each congressperson changes Census-to-Census. https://history.house.gov/Historical-Highlights/1901-1950/The-Permanent-Apportionment-Act-of-1929/, DoA 22 December 2022.

## Reapportionment
# Presently the U.S. Census Bureau must deliver the results of a decennial census to the President of the United States within nine months of the census date. Within a week of the opening of the next Congress, the President is required by law to report the census results to Congress. 
# Within 15 days, the Clerk must then disclose to the governor of each state how many seats his or her state is entitled. 
# The state legislatures are charged with redrawing a state’s congressional districts. 
# Apportionments take effect two Congresses (three years) after the last census.
# https://history.house.gov/Institution/Apportionment/Reapportioning/ DoA: 10 Dec 2022.
# An apportionment data time series published by the US Census Bureau may be viewed here: https://www.census.gov/data/tables/time-series/dec/apportionment-data-text.html DoA: 10 December 2022.


# https://www.visitthecapitol.gov/sites/default/files/documents/resources-and-activities/CVC_HS_ActivitySheets_CongApportionment.pdf
# 
# legal precedent following from Wesberry v. Sanders that congressional districts must be approximately equal in population. 
# Specifically, in Wesberry v. Sanders the US Supreme Court ruled that malapportionment, or the failure to guarantee equivalent numbers of citizens per district, is unconstitutional and districts must be approximately equal in population (see Wesberry v. Sanders). 

## The Voting Rights Act of 1965:
# Additionally, Section 2 of the Voting Rights Act of 1965 prohibits redistricting plans that are intended to, or have the effect of, discriminating against racial or language minority voters [15].
# Aside from malapportionment and discrimination against racial or language minorities, federal courts have allowed state legislatures to engage in gerrymandering to benefit political parties or incumbents [16][17].
# In a 1984 case, Davis v. Bandemer, the Supreme Court held that gerrymandered districts could be struck down based on the Equal Protection Clause, but the Court did not articulate a standard for when districts are impermissibly gerrymandered. 

## State-Level Electoral Systems:
# Elections for representatives are held in every even-numbered year, on Election Day the first Tuesday after the first Monday in November. 
# Pursuant to the Uniform Congressional District Act, representatives must be elected from single-member districts. 
# After a census is taken (in a year ending in 0), the year ending in 2 is the first year in which elections for U.S. House districts are based on that census (with the Congress based on those districts starting its term on the following January 3). 
# As there is no legislation at the federal level mandating one particular system for elections to the House, systems are set at the state level. 
# As of 2022, so-called "first-past-the-post" i.e., plurality voting is adopted in 46 states
# Ranked-choice or "instant-runoff" voting in two states (Alaska and Maine).
# The two-round system in two states (Georgia and Mississippi). 

## Effects of Current System
# According to calculations made by Burt Neuborne using criteria set forth by the American Political Science Association, about 40 seats, **less than 10% of the House membership, are chosen through a genuinely contested electoral process, given partisan gerrymandering.[18][19]**
# Our simulations show ____________________.

######
#### Data Sources:

## The US Census Bureau:
# Decennial Census Data (1910-2020): https://www.census.gov/programs-surveys/decennial-census/data/tables.html
# Population Change Data (1910-2020): https://www.census.gov/data/tables/time-series/dec/popchange-data-text.html
# Population Density Data (1910-2020): https://www.census.gov/data/tables/time-series/dec/density-data-text.html
# Historical apportionment Data https://www.census.gov/library/visualizations/interactive/historical-apportionment-data-map.html 

## Population Data (according to the 2020 US Census)
# U.S. Population:
# State Populations
# Alaska	
# Alabama	
# 

## Population Density Data

## Prior Districting

# Obtain Precise ___File of Congressional Districts https://www.census.gov/programs-surveys/geography/guidance/geo-areas/congressional-dist.html



#### US population data (i.e., the total US population from the 2020 Census):





# Single member states
Alaska, Delaware, Montana, North Dakota, South Dakota, Vermont, and Wyoming




# Obtain random numbers:
# https://qrng.anu.edu.au/contact/api-documentation/

# The QRNG@ANU JSON API supports three parameters. These are:

# Data type, the data type must be ‘uint8’ (returns integers between 0–255), ‘uint16’ (returns integers between 0–65535) or ‘hex16’ (returns hexadecimal characters between 00–ff).
# Array length, the length of the array to return. Must be between 1–1024.
# Block size, only needed for ‘hex16’ data type. Sets the length of each block. Must be between 1–1024.
# https://qrng.anu.edu.au/API/jsonI.php?length=[array length]&type=[data type]&size=[block size]
# If the request is successful, the random numbers are returned in a JSON encoded array named ‘data’.

# Examples
# Requesting 10 random numbers between 0–255

# https://qrng.anu.edu.au/API/jsonI.php?length=10&type=uint8
# Requesting 5 random numbers between 0–65535

# https://qrng.anu.edu.au/API/jsonI.php?length=5&type=uint16
# Requesting 10 blocks of random numbers in hexadecimal format. Each block is between 0000–ffff

# https://qrng.anu.edu.au/API/jsonI.php?length=10&type=hex16&size=2The QRNG@ANU JSON API supports three parameters. These are:

# Data type, the data type must be ‘uint8’ (returns integers between 0–255), ‘uint16’ (returns integers between 0–65535) or ‘hex16’ (returns hexadecimal characters between 00–ff).
# Array length, the length of the array to return. Must be between 1–1024.
# Block size, only needed for ‘hex16’ data type. Sets the length of each block. Must be between 1–1024.
# https://qrng.anu.edu.au/API/jsonI.php?length=[array length]&type=[data type]&size=[block size]
# If the request is successful, the random numbers are returned in a JSON encoded array named ‘data’.

# Examples
# Requesting 10 random numbers between 0–255

# https://qrng.anu.edu.au/API/jsonI.php?length=10&type=uint8
# Requesting 5 random numbers between 0–65535

# https://qrng.anu.edu.au/API/jsonI.php?length=5&type=uint16
# Requesting 10 blocks of random numbers in hexadecimal format. Each block is between 0000–ffff

# https://qrng.anu.edu.au/API/jsonI.php?length=10&type=hex16&size=2# CongressionalRedistricting
