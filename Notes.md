

# Obtain population density data


# Obtain Precise ___File of Congressional Districts
https://www.census.gov/programs-surveys/geography/guidance/geo-areas/congressional-dist.html


# US population data
# Total US population (2020 Census):

# Population per seat (Total of 435 congressional districts s/p fixation in 


# Single member states
Alaska, Delaware, Montana, North Dakota, South Dakota, Vermont, and Wyoming


# States typically redraw district boundaries after each census, though they may do so at other times, such as the 2003 Texas redistricting. 
# Each state determines its own district boundaries, either through legislation or through non-partisan panels. "Malapportionment" is unconstitutional and districts must be approximately equal in population (see Wesberry v. Sanders). 
# Additionally, Section 2 of the Voting Rights Act of 1965 prohibits redistricting plans that are intended to, or have the effect of, discriminating against racial or language minority voters.[15] Aside from malapportionment and 
# discrimination against racial or language minorities, federal courts have allowed state legislatures to engage in gerrymandering to benefit political parties or incumbents.[16][17] In a 1984 case, Davis v. Bandemer, the Supreme Court 
# held that gerrymandered districts could be struck down based on the Equal Protection Clause, but the Court did not articulate a standard for when districts are impermissibly gerrymandered. 

# 

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

# https://qrng.anu.edu.au/API/jsonI.php?length=10&type=hex16&size=2