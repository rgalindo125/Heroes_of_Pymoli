# Heroes_of_Pymoli
 Heroes Of Pymoli Data Analysis

Of the 1163 active players, the vast majority are male (84%). There also exists, a smaller, but notable proportion of female players (14%).
Our peak age demographic falls between 20-24 (44.8%) with secondary groups falling between 15-19 (18.60%) and 25-29 (13.4%).  


 Note

Instructions have been included for each segment. You do not have to follow them exactly, but they are included to help you think through the steps.


    In [1]:
   # Dependencies and Setup
import pandas as pd
import numpy as np

# File to Load (Remember to Change These)
file_to_load = "Resources/purchase_data.csv"

# Read Purchasing File and store into Pandas data frame
purchase_data = pd.read_csv(file_to_load)  Player Count
 
Display the total number of players


    In [2]:
     

  
    
      
      Total Players
    
  
  
    
      0
      576
    
  

 Purchasing Analysis (Total)
 
Run basic calculations to obtain number of unique items, average price, etc.


Create a summary data frame to hold the results


Optional: give the displayed data cleaner formatting


Display the summary data frame


    In [3]:
     


  
    
      
      Number of Unique Items
      Average Price
      Number of Purchases
      Total Revenue
    
  
  
    
      0
      183
      $3.05
      780
      $2,379.77
    
  

 Gender Demographics
 
Percentage and Count of Male Players


Percentage and Count of Female Players


Percentage and Count of Other / Non-Disclosed


    In [4]:
     


  
    
      
      Total Count
      Percentage of Players
    
  
  
    
      Male
      484
      84.03
    
    
      Female
      81
      14.06
    
    
      Other / Non-Disclosed
      11
      1.91
    
  

 Purchasing Analysis (Gender)
 
Run basic calculations to obtain purchase count, avg. purchase price, avg. purchase total per person etc. by gender


Create a summary data frame to hold the results


Optional: give the displayed data cleaner formatting


Display the summary data frame


    In [5]:
     

  
    
      
      Purchase Count
      Average Purchase Price
      Total Purchase Value
      Avg Total Purchase per Person
    
    
      Gender
      
      
      
      
    
  
  
    
      Female
      113
      $3.20
      $361.94
      $4.47
    
    
      Male
      652
      $3.02
      $1,967.64
      $4.07
    
    
      Other / Non-Disclosed
      15
      $3.35
      $50.19
      $4.56
    
  

 Age Demographics
 
Establish bins for ages


Categorize the existing players using the age bins. Hint: use pd.cut()


Calculate the numbers and percentages by age group


Create a summary data frame to hold the results


Optional: round the percentage column to two decimal points


Display Age Demographics Table


    In [6]:
     


  
    
      
      Total Count
      Percentage of Players
    
  
  
    
      <10
      17
      2.95
    
    
      10-14
      22
      3.82
    
    
      15-19
      107
      18.58
    
    
      20-24
      258
      44.79
    
    
      25-29
      77
      13.37
    
    
      30-34
      52
      9.03
    
    
      35-39
      31
      5.38
    
    
      40+
      12
      2.08
    
  

 Purchasing Analysis (Age)
 
Bin the purchase_data data frame by age


Run basic calculations to obtain purchase count, avg. purchase price, avg. purchase total per person etc. in the table below


Create a summary data frame to hold the results


Optional: give the displayed data cleaner formatting


Display the summary data frame


    In [7]:
     

  
    
      
      Purchase Count
      Average Purchase Price
      Total Purchase Value
      Avg Total Purchase per Person
    
  
  
    
      10-14
      28
      $2.96
      $82.78
      $3.76
    
    
      15-19
      136
      $3.04
      $412.89
      $3.86
    
    
      20-24
      365
      $3.05
      $1,114.06
      $4.32
    
    
      25-29
      101
      $2.90
      $293.00
      $3.81
    
    
      30-34
      73
      $2.93
      $214.00
      $4.12
    
    
      35-39
      41
      $3.60
      $147.67
      $4.76
    
    
      40+
      13
      $2.94
      $38.24
      $3.19
    
    
      <10
      23
      $3.35
      $77.13
      $4.54
    
  

 Top Spenders
 
Run basic calculations to obtain the results in the table below


Create a summary data frame to hold the results


Sort the total purchase value column in descending order


Optional: give the displayed data cleaner formatting


Display a preview of the summary data frame


    In [8]:
     

  
    
      
      Purchase Count
      Average Purchase Price
      Total Purchase Value
    
    
      SN
      
      
      
    
  
  
    
      Lisosia93
      5
      $3.79
      $18.96
    
    
      Idastidru52
      4
      $3.86
      $15.45
    
    
      Chamjask73
      3
      $4.61
      $13.83
    
    
      Iral74
      4
      $3.40
      $13.62
    
    
      Iskadarya95
      3
      $4.37
      $13.10
    
  

 Most Popular Items
 
Retrieve the Item ID, Item Name, and Item Price columns


Group by Item ID and Item Name. Perform calculations to obtain purchase count, item price, and total purchase value


Create a summary data frame to hold the results


Sort the purchase count column in descending order


Optional: give the displayed data cleaner formatting


Display a preview of the summary data frame


    In [9]:
     

  
    
      
      
      Purchase Count
      Item Price
      Total Purchase Value
    
    
      Item ID
      Item Name
      
      
      
    
  
  
    
      178
      Oathbreaker, Last Hope of the Breaking Storm
      12
      $4.23
      $50.76
    
    
      145
      Fiery Glass Crusader
      9
      $4.58
      $41.22
    
    
      108
      Extraction, Quickblade Of Trembling Hands
      9
      $3.53
      $31.77
    
    
      82
      Nirvana
      9
      $4.90
      $44.10
    
    
      19
      Pursuit, Cudgel of Necromancy
      8
      $1.02
      $8.16
    
  

 Most Profitable Items
 
Sort the above table by total purchase value in descending order


Optional: give the displayed data cleaner formatting


Display a preview of the data frame


    In [10]:
     

  
    
      
      
      Purchase Count
      Item Price
      Total Purchase Value
    
    
      Item ID
      Item Name
      
      
      
    
  
  
    
      178
      Oathbreaker, Last Hope of the Breaking Storm
      12
      $4.23
      $50.76
    
    
      82
      Nirvana
      9
      $4.90
      $44.10
    
    
      145
      Fiery Glass Crusader
      9
      $4.58
      $41.22
    
    
      92
      Final Critic
      8
      $4.88
      $39.04
    
    
      103
      Singed Scalpel
      8
      $4.35
      $34.80
