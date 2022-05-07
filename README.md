# Understanding Your Customers 
> Guide for entering auto insurance industries through analysing auto insurance company data.
> 
> Presented By: Brenna Yin, Yijun Yang

## Table of Contents
1. Backstory
2. Data Overview
   - Features and Claims
   - Customers Profile
   - Scoring System
3. Selecting Important Features
   - The Importance of Using Categorical Features
   - From Numerical to Categorical – Age, Points Taken, Number of Children
   - From Complexity to Simplicity – Vehicle Type
   - Binary Features – License Revoked, Vehicle Use
4. Analyzing Zero Claim Customers
5. Takeaway - Scoring System
   - Final version
   - Validation
7. What's Next

## Backstory

When I bought my first car, I realized that auto insurance is no longer the advertisement I see on the billboards standing besides the freeways. It became a product that I am required to purchase and it needs to be chosen carefully. 

Being an ordinary customer, insurance is a necessity along with my car. A car must come along with its insurance. That grows billions of auto insurance markets today in the U.S. 

I got my first quote from an insurance company that works with my car’s dealership after filling a really long and detailed questionnaire. I told them basically everything about myself, my age, my education level, my citizenship, my salary, my marriage history/status, the number of children I have. Providing so much personal information just because I want to get the insurance for my car and myself with the lowest price.  At one point, I even filled out my undergrad GPA so that I could get a lower price for being a well-behaving person in academics.

We can see from that it is true that insurance companies have the closest access to the data which associates with people’s mundane life.

Getting to know the auto insurance industry helps us understand our life and the reality of the world we live in. 
Please continue reading if you are now one of these followings:
> someone just entering auto insurance field 
>  
> someone thinking about entering auto insurance field
>  
> someone who want to know about auto insurance with reality data

Entering the auto insurance industry, means we are dealing with highly personal information. Auto insurance industry exists to accommodate customers’ needs so people could drive legally with responsibility for others and themselves. Those companies are large, convoluted mechanics dealing with complex reality problems every day. 

But luckily, there is an easier way to get to know this big machine by directly looking at the data from it. Such a scenario above about getting a quote is extremely common and it provides massive data for auto insurance companies. 

Before data mining, we need to be aware of some **key questions** in the insurance industry:
>   Will this potential customer file a claim?
> 
>   Will this new customer file a claim? 
> 
>   Will this old customer file a claim?
>    
>   Will this old customer file a claim again?
    
Clearly, the critical point here is to file a claim or not for a customer. That is, frankly, the top question insurance companies are concerned with. Regardless of the fields. So as a “green-hand” in this field, it is a good idea to know ***first*** how to identify the filing risk of customers based on their provided personal information.

**That is, how to classify the customers?**

We here suggest you to do that through the company data. With some data mining, we could know
1. What a modern auto insurance industry looks like
2. What are customer profiles for an auto insurance company
3. How to evaluate the customers with certain risk scores

They are sufficient for starting to know this industry and are helpful to build your own journey later. 

#### * *Ethical Reminding* *
Just like credit scores, insurance information is highly personal and holds privacy because of its intrinsic characteristic.
When you have access to any insurance data, you should not disclose that private information to unauthorized parties.
You must refrain from publishing data that contains personally identifiable information (PII). Remember that PII can also include information that allows a person's identity to be inferred.
Keep all these in mind, let’s start to take a look at an auto insurance company data. 

## Overview of the Data
The sample data we are looking at comes from a five year claim history from an actual auto company. (data link: )
The tools we used to analyze and present our data are python and tableau. 

### Features and Claims
Usually, the data from an auto insurance company is massive. To better understand such a large volume of data, we divide the data into three groups:

1. Features describing the vehicles: type, color, usage, value, etc. 
2. Features describing the drivers: age, occupation, education, gender, # of children they have, income, home value, etc.
3. Information about the claim: claim or not, number of claims, amount of claim. 

In our sample data:
 > The total claim amount in five years for this company is `$11.33M`, with an average claim amount `$1481`.
 > 
 > The total number of claims in five years is `6046 claims`, with an average number of claims `0.79`. 
 > 
From above calculation results, we could see that the amount of money being processed is large and the frequency of filing claims happens very often (even more often than you thought).

