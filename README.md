# group_project_1
Repo for group_proj

This project’s aim is to understand the trends of national outbreak data. Our data source contains a  full 2020 - 2021 CDC infectious outbreak dataset. The data include information relating to time, place, mode, etiology  of outbreak and other outcomes. 

This report includes 

- preprocessing of data
- Trends in the mode of infection.What was the top primary mode of infection by state per year?
- Trends of the setting and mode of the top outbreaks
- Trends of hospitalizations and deaths
- Summary and conclusion of data analyis
- Additional finding for farther research 


Preprocessing of data: 

NationalOutbreakPublicDataTool.csv -- Original Data pulled from CDC.gov  
Useable_data.ipynb -- Jupyter notebook to take original csv and reduce the columns and rows to useable data   
  -- removed any rows that had NaN values  
  -- reduced columns  
Cleaned_outbreak_data.csv -- CSV file meant for getting data for analysis  



What were the trends in the mode of infection.What was the top primary mode of infection by state per year?
 
There were 6 different primary modes  of outbreak in the full 2020 - 2021 dataset. These modes were: person to person, food, indeterminate/other/unknown, water, animal contact, environmental contamination other than food/water. In 2020 and 2021 the top primary mode was person to person. In 2020 57.4% of the states had person to person was the top primary mode of outbreak. In 2021 47.9% of the states had person to person as their primary mode of outbreak . Following person to person is water outbreaks for both years. 
Focusing in on a particular state, Wisconsin, in 2020 88.5% of the cases in Wisconsin were person to person. In 2021 72.8% of the cases in Wisconsin were  person to person. An independent t test was used to compare the two subsets of data (2020 vs 2021). The p-value of this test was .88, this showed the top primary mode of per state from 2020 to 2021 were not significantly different. 



What are the trends of the setting and mode of the top outbreaks?

The setting is where the illness was contracted (ex: "Daycare"), and the mode is how the illness was contracted("Person-to-person"). There are also 2 distinct groups per etiology(illness): a confirmed and suspected status. Confirmed is when the specific illness is tested in a medical lab via a biological sample collected from the patient. The test result would have to come back as "positive" for a confirmed status. Suspected would be if all symptoms match an specific illness, so one would have reasonable justification to report that illness.
The data frames and graphs show that confirmed and suspected cases are nearly equal. Nursing homes/Assisted Living is - by far - the most common setting to contract illnesses, followed by Daycare. The most common mode of infection is person-to-person contact, followed by food contamination.



What are the trends of hospitalization deaths?

Highest reported etiology:

The highest reported number of cases for 2020-2021 was “Norovirus unknown” with 17,424 cases, 355 hospitalized individuals, with 22 deaths. Followed by Norovirus Genogroup II with 11,536 cases, 189 hospitalized, and 19 deaths.

Highest hospitalization etiology: 

The highest outbreak that had the most hospitalized cases was “Salmonella enterica” with 1707 cases out of 8282 reported cases, yielding 11 deaths total in 2020-2021.
Highest likelihood of hospitalization: 

There was a 4-way tie of outbreaks that caused 100% hospitalization; “Legionella pneumophila; Legionella anisa”, “Campylobacter coli; Escherichia coli, Enterotoxigenic; Salmonella enterica; Cryptosporidium unknown; Escherichia coli, Enteropathogenic”, “Clostridium botulinum”, and “Legionella unknown”. Followed by “Listeria monocytogenes” with 91.30% likelihood.

Highest death etiology:

The outbreak that caused the most deaths in 2020-2021 (minus COVID19), was “Norovirus unknown” with 22 total deaths, 17,424 reported cases, and 355 hospitalizations. Followed by “Norovirus Genogroup II” with 19 deaths, 11536 reported cases, and 189 hospitalizations. Respectively they had .13% and .16% of being lethal.
Highest likelihood of Death:

The outbreak that had the highest chance of lethality in 2020-2021 was “Legionella pneumophila; Legionella anisa” with 33% death rate with 1 death for the 3 reported cases–3 hospitalizations. Followed by “Pseudomonas aeruginosa” with 17.39% death rate with 4 deaths out of the 23 reported cases–12 hospitalizations.

Correlation of Deaths vs Hospitalizations:

The linear regression equation from the data in the data set yielded y=22.23x +5.05 with an r value of .4865. With this, we can say that the number of deaths does correlate a little bit with the number of hospitalizations.

FULL SUMMARY AND CONCLUSION
Person-to-person is the primary mode for outbreaks in the U.S. with over 37,000 reported cases in 2020-2021.Looking at the primary mode for outbreaks per state, over 50% of states had person-to-person as the highest cause for outbreaks in 2020-2021; 57.4% in 2020, and 47.9% in 2021.Looking specifically at Wisconsin, person-to-person was the primary mode of infection in 2020-2021—supporting the above conclusions.Statistically speaking, the year 2020 and 2021 did not have a significant difference between the primary mode of outbreaks with a P-value of 0.88.

Long-term care/nursing home/assisted living facilities, as a setting, had the most confirmed and suspected outbreaks in 2020-2021.There was an even distribution of confirmed and suspected cases in 2020-2021—52% to 48% respectively.

The highest reported number of cases for 2020-2021 was “Norovirus unknown” with 17,424 cases, 355 hospitalized cases, and 22 deaths. This was followed by "Norovirus Genogroup II" with 11,536 cases, 189 hospitalized, and 19 deaths.The highest outbreak that had the most hospitalized cases was “Salmonella enterica” with 1,707 cases out of 8,282 reported cases, yielding 11 deaths total in 2020-2021.There was a 4-way tie of outbreaks that caused 100% hospitalization; “Legionella pneumophila; Legionella anisa”, “Campylobacter coli; Escherichia coli, Enterotoxigenic; Salmonella enterica; Cryptosporidium unknown; Escherichia coli, Enteropathogenic”, “Clostridium botulinum”, and “Legionella unknown”. Followed by “Listeria monocytogenes” with 91.30% hospitalization rate.​

The outbreak that caused the most deaths in 2020-2021, was “Norovirus unknown” with 22 total deaths, 17,424 reported cases, and 355 hospitalizations. Followed by “Norovirus Genogroup II” with 19 deaths, 11,536 reported cases, and 189 hospitalizations. Respectively, they had 0.13% and 0.16% death rate.The outbreak that had the highest death rate in 2020-2021 was “Legionella pneumophila; Legionella anisa” with 33% death rate with 1 death for the 3 reported cases--3 hospitalization. Followed by “Pseudomonas aeruginosa” with 17.39% death rate with 4 death out of the 23 reported cases–12 hospitalizations.The number of deaths had a weak correlation with the number of hospitalizations—with an r-value of .04865

ADDITIONAL FINDINGS 
- Multistate (unknown grouped states) had the most cases (7,758), hospitalizations(1752), and deaths(31). This was followed closely by Wisconsin with 4,377 cases, 140 hospitalizations and 12 deaths.

- The least amount of reported cases of outbreaks in 2020-2021 per state, was Mississippi, with 10 reported cases, 0 hospitalizations, and 0 deaths.

- 17 states reported having "Norovirus unknown" as the leading cause for outbreaks, followed by "Norovirus Genogroup II" with 15 states.