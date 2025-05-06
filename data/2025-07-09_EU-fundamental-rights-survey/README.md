# FRA-EU Survey

Building on last month’s dataset, this month’s data set is the EU LGBT Survey from 2019. The FRA is an organization which examines the rights, attitudes and living standards of LGBT people in Europe. They have been working on documenting these topics since 2010 and are currently working on their newest edition of the survey. Last month’s data was the first wave of this survey from 2012, this month’s data gives us the results from the second wave, showing us we still have a long way to go. Since we are dealing with longitudinal data, why not try to combine the last two data sets and see which trends you can discover!

The two main differences between the data sets are: 
1) The 2012 survey only includes people over 18 years old whereas the 2019 survey includes people starting at age 15
2) Data specific to intersex people was only collected in the second wave of the survey. 

A total of 139,799 persons aged 15 years or older who describe themselves as lesbian, gay, bisexual, trans or intersex (LGBTI) completed the online EU-LGBTI II Survey in all EU Member States and the candidate countries of North Macedonia and Serbia.

The survey was conducted online from 27 May to 22 July 2019. Its questionnaire covered a wide range of issues, such as experiences with discrimination, harassment or violence, rights awareness, openness about being LGBTI, positive and negative experiences at work and in education, socio-economic and living conditions, health and well-being, and housing issues.

The findings are based on data weighted to take into account differences in the estimated size of each LGBTI group in each survey country and by age group, based on information on the LGBTI population from previous LGBTI surveys in the EU. In addition, the data were weighted taking into account the respondents’ affiliation with LGBTI organisations and whether they have participated in other LGBTI surveys (including FRA’s LGBT survey of 2012). This was done to correct for possible over-representation of respondents closely affiliated with LGBTI organisations and with a higher propensity to participate in LGBTI surveys.


## About the data 

Each dataset was cleaned by removing the rows 1 to 14, deleted column `question_code` and `notes`, replaced all values in `percentage` column that contained ':' as a missing value holder with NA. Categories or factors with large amount of 'NA' values were removed. The `Trans subgroups` factor "cross-dresser" was excluded from this data.

**Note**
> EU-28 = UK,  UK and EU-28 exist together in dataset
  some age ranges for specific groups have missing countries

### Topics 

| number | topic                        		|
| :----- | :--------------------------- 		|
| 1      | Living openly and daily life 		|
| 2      | Experiencing and reporting discrimination    |
| 3      | Hate-motivated violence and harassment 	|
| 4      | The situation of intersex persons 		|

  
### Target group: 

  - lesbian women 
  - gay men
  - bisexual women
  - bisexual men 
  - trans people
  - intersex 
  
### Group factors  (subset)

| factor     | levels                                             |
| :--------- | :------------------------------------------------- |
| age        | (15-17), (18-24), (25-39), (40-54), (55+ )         | 
| education  | lower secondary or less, upper secondary, tertiary | 
| employment | - paid work (incl. self employment)                | 
|            | - unpaid voluntary work                            | 
|            | - unemployment                                     | 
|            | - student                                          | 
|            | - retired                                          | 
|            | - unable to work - health issues                   | 
|            | - otherwise not working                            | 
| openness   | about being LGBTI                                  |
|            | very open, fairly open, rarely open, never open    |
| partner    | female, male, other/non-binary, no partner         |
| residence  | city, suburbs, town, country village, countryside  | 
| gender_id  | trans women                                        |
|            | trans man                                          |
|            | trans person                                       |
|            | non-binary                                         |
|            | genderqueer                                        |
|            | genderfluid                                        |
|            | agender                                            |
|            | polygender                                         | 


### Questions

- 1. *Do you avoid holding hands in public with a same-sex partner for fear of being assaulted, threatened or harassed ?*  
- 2. *Do you avoid certain places or locations for fear of being assaulted, threatened or harassed due to being LGBTI?*   
- 3. *Where do you avoid being open about yourself as LGBTI for fear of being assaulted, threatened or harassed by others?*
- 4. *How old were you when you realized for the first time you were LGB?*             
- 5. *Feeling downhearted/ depressed in the past 2 weeks*


### Data file organization
Each of the 5 files is related to one of the questions mentioned above. Within each question the sheets are organized as follows.

| dataset sheet number    | filename             | description  (categories or factors)             |   
| :---------------------- | :--------------------|------------------------------------------------- | 
|  1                      | T1Q1-LGBTI-age       | topic 1 question 1 for all age categories        |  
|  2                      | T1Q1-LGBTI-edu       | topic 1 question 1 for all education categories  |    
|  3                      | T1Q1-LGBTI-emp       | topic 1 question 1 for all employment categories |    
|  4                      | T1Q1-LGBTI-open      | topic 1 question 1  level of LGBTI openness      |   
|  5                      | T1Q1-LGBTI-partner   | topic 1 question 1  partner type                 |    
|  6                      | T1Q1-LGBTI-res       | topic 1 question 1  place of residence           |   
|  7                      | T1Q1-T-gender        | topic 1 question 1 Transgender gender identities | 



## Why this is relevant 

The EU-LGBTI II is the second version of the broad survey conducted in Europe. In this new iteration, new issues were taken into account and an extra focus on intersex people was introduced. Updates on surveys such as this are always important to keep up with current issues or interests about, of and within a community. 

When assessing the lives and circumstances of the LGBTQ+ community, it is not enough to look at one snapshot. That is why repetitions of these kinds of surveys are important, it allows us not only to get the most recent data but it also provides us an opportunity to look at changes within the community over time. That is why #TidyRainbow invites you to look not only at this month's data by itself but also with regards to the data of last month and the changes we can observe over time.








