# Depression and Long-Term Survival Following Moderate-to-Severe Traumatic Brain Injury: A Longitudinal Retrospective Analysis of the TBIMS NDB

## Introduction
This study seeks to examine associations between depression and all-cause mortality in the **{##}** years following hospitalization for moderate-to-severe traumatic brain injury (msTBI), with and without adjustment for known risk factors for death.

To be eligible for inclusion in the present study, patients must have been enrolled in the [Traumatic Brain Injury Model Systems National Database](https://www.tbindsc.org/) with an index injury date between October 1, 2006 and October 1, 2012. Follow-up in this study continued through October 1, 2022.

## Variables of Interest

### Primary Exposure: Depression Level at Year 1
Depression levels were computed from participants' responses to the Patient Health Questionnaire (PHQ-9) at the first follow-up interview following the index injury (i.e., Year 1). The PHQ-9 consists of 9 items that can be scored from 0 (Not at All) to 3 (Nearly Every Day), producing a total score that ranges from 0 to 27. In the present study, participants' depression severity levels are categorized into "No Depression," "Minor Depression," and "Major Depression" based on the individual's endorsement of *positive symptoms* and *cardinal symptoms* of depression within the two weeks preceding the interview. 

First, the positive symptoms of depression were calculated for each participant as the total number of PHQ-9 items scored at 1 or higher, indicating that the symptom was present for several days or more over the two-week period prior to the interview. The categorization process considers both the total count of positive symptoms (i.e., total number of PHQ-9 items endorsed at a frequency of several days or more within the previous two weeks) as well as the presence of cardinal symptoms of depression (i.e., anhedonia and depressed mood, represented by the first and second items of the PHQ-9, respectively). 

- The **No Depression** label is reserved for cases in which the total number of positive symptoms is 0 or 1 and/or for cases in which neither cardinal symptom is endorsed (regardless of the total number of positive symptoms endorsed);
- The **Minor Depression** label is reserved for cases in which the total number of positive symptoms is 2 to 4 inclusive and one or both cardinal symptoms are endorsed; and
- The **Major Depression** label is reserved for cases in which the total number of positive symptoms ranges from 5 to 9 inclusive, and one or both cardinal symptoms are endorsed.

**SOCIODEMOGRAPHIC CHARACTERISTICS**

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `AGE`                  | `age`             | Age at Injury                                 | 9999 - Unknown |
| `SexF`                 | `sex`             | Interview Question: Sex                       | 1 - Female<br>2 - Male<br>99 - Unknown |
| `Race`                 | `race`            | Interview Question: What is your race?        | 1 - White<br>2 - Black<br>3 - Asian/Pacific Islander<br>4 - Native American<br>5 - Hispanic Origin<br>7 - Other<br>99 - Unknown |
| `EDUCATION`            | `education_level_at_injury` | Interview Question: Education       | 1 - 8th Grade or Less<br>2 - 9th - 11th Grade<br>2.5 - GED<br>3 - HS/GED<br>3.5 - HS<br>4 - Trade<br>5 - Some College<br>6 - Associate's Degree<br>7 - Bachelor's Degree<br>8 - Master's Degree<br>9 - Doctorate<br>777 - Other<br>999 - Unknown |
| `EMPLOYMENT`           | `employment_at_injury` | Interview Question: At the time of injury, what was your employment status? | 2 - Full Time Student<br>3 - Part Time Student<br>4 - Special Education<br>5 - Employed<br>7 - Homemaker<br>8 - Employed<br>9 - Retired<br>10 - Unemployed<br>11 - Volunteer<br>12 - Other<br>888 - Not Applicable<br>999 - Unknown |
| `Mar`                  | `marital_status_at_injury` | Interview Question: What is your marital status? | 1 - Single (Never Married)<br>2 - Married<br>3 - Divorced<br>4 - Separated<br>5 - Widowed<br>7 - Other<br>99 - Unknown |



The present study utilizes a retrospective observational design and draws data from the [Traumatic Brain Injury Model Systems](https://msktc.org/about-model-systems/TBI) (TBIMS) longitudinal cohort study. The TBIMS is a well-established multi-center research initiative with extensive data from individuals with TBI throughout the United States.  Time-to-event is assessed using Cox proportional hazards modeling.


### Tools and Packages
This project uses the following R packages:
- [`survival`](https://github.com/therneau/survival)

### References and Documentation
Access and use of the [TBIMS National Database](https://www.tbindsc.org/) (NDB) data is governed by the TBIMS standard operating procedures.
