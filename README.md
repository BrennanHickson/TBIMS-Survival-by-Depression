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

### Proposed Covariates: Predictors of Mortality in TBI
The following TBIMS variables were proposed as covariates in the survival analysis due to their previously observed associations with mortality among TBI patients in the prior literature. Additional information about each variable may be accessed at the [TBIMS Data Dictionary](https://hub.tbindsc.org/tbimsdatadictionary/Home).

**SOCIODEMOGRAPHIC CHARACTERISTICS**

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `AGE`                  | `age`             | Age at Injury                                 | 9999 - Unknown |
| `SexF`                 | `sex`             | Interview Question: Sex                       | 1 - Female<br>2 - Male<br>99 - Unknown |
| `EduYears`            | `education_level_at_injury` | Interview Question: How many years of education have you completed? If you have not graduated from high school, choose the number of years spent in school. If you have at least a high school diploma, please indicate the highest degree earned (or worked toward). | 1 - 1 Year or Less<br>2 - 2 Years<br>3 - 3 Years<br>4 - 4 Years<br>5 - 5 Years<br>6 - 6 Years<br>7 - 7 Years<br>8 - 8 Years<br>9 - 9 Years<br>10 - 10 Years<br>11 - 11 or 12 Years: No diploma<br>12 - HS Diploma<br>13 - Work Toward Associate's<br>14 - Associate's<br>15 - Work Toward Bachelor's<br>16 - Bachelor's Degree<br>17 - Work Toward Master's<br>18 - Master's Degree<br>19 - Work Toward Doctoral Level<br>20 - Doctoral Level Degree<br>21 - Other<br>666 - Variable Did Not Exist<br>999 - Unknown |
| `EMPLOYMENT`           | `employment_at_injury` | Interview Question: At the time of injury, what was your employment status? | 2 - Full Time Student<br>3 - Part Time Student<br>4 - Special Education<br>5 - Employed<br>7 - Homemaker<br>8 - Employed<br>9 - Retired<br>10 - Unemployed<br>11 - Volunteer<br>12 - Other<br>888 - Not Applicable<br>999 - Unknown |
| `Mar`                  | `marital_status_at_injury` | Interview Question: What is your marital status? | 1 - Single (Never Married)<br>2 - Married<br>3 - Divorced<br>4 - Separated<br>5 - Widowed<br>7 - Other<br>99 - Unknown |

**BASELINE HEALTH AND ACUTE INJURY CHARACTERISTICS**

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `RehabPay1`            | `rehab_payor_primary` | Interview Question: Primary rehabilitation payor                                 | 1 - Medicare<br>2 - Medicaid<br>3 - Workers' Compensation<br>4 - Private Insurance<br>7 - Self or Private Pay<br>8 - State or County<br>10 - Auto Insurance<br>14 - Charity<br>15 - Other<br>55 - Payor Source Pending<br>999 - Unknown |
| `Cause`                | `cause_of_injury` | Interview Question: Cause of injury          | 1 - Motor Vehicle<br>2 - Motorcycle<br>3 - Bicycle<br>4 - All-Terrain Vehicle (ATV) and All-Terrain Cycle (ATC)<br>5 - Other Vehicular: Unclassified<br>10 - Gunshot Wound<br>11 - Assaults With Blunt Instrument<br>12 - Other Violence<br>13 - Water Sports<br>14 - Field/Track Sports<br>15 - Gymnastic Activities<br>16 - Winter Sports<br>17 - Air Sports<br>18 - Other Sports<br>19 - Fall<br>20 - Hit By Falling/Flying Object<br>21 - Pedestrian<br>22 - Other Unclassified<br>999 - Unknown |
| `PROBLEMUse`           | `problematic_substance_use` | Interview Question: Substance Problem Use | 0 - No<br>1 - Yes<br>77 - Refused<br>99 - Unknown |
| `PROBLEMUseF`          | `problematic_substance_use` | Interview Question: Substance Problem Use | 0 - No<br>1 - Yes<br>99 - Unknown |
| `Suicide`              | `suicide_attempt_hx_lifetime_at_injury` | Interview Question: Have you ever attempted suicide? | 0 - No<br>1 - Yes<br>66 - Variable Did Not Exist<br>77 - Refused<br>88 - Not Applicable<br>99 - Unknown |
| `SuicidePrior`              | `suicide_attempt_hx_past_year_at_injury` | Interview Question: If yes, did you attempt suicide in the year before the injury? | 0 - No<br>1 - Yes<br>66 - Variable Did Not Exist<br>77 - Refused<br>88 - Not Applicable<br>99 - Unknown |

**FUNCTIONAL INDEPENDENCE AT YEAR 1**

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `DRSF`                 | `drs_total_at_followup` | Interview Question: Disability Rating Scale Follow-up  | 999 - Unknown |
| `FIMTOTF`              | `fim_total_at_followup` | Interview Question: FIM Total (New) Follow-up | 9999 - Unknown |
| `GOSEF`                 | `gose_total_at_followup` | Interview Question: GOS-E Incl. Expired | 1 - Dead<br>2 - Vegetative State (VS)<br>3 - Lower Severe Disability (LSD)<br>4 - Upper Severe Disability (USD)<br>5 - Lower Moderate Disability (LMD)<br>6 - Upper Moderate Disability (UMD)<br>7 - Lower Good Recovery (LGR)<br>8 - Upper Good Recovery <UGR)<br>66 - Variable Did Not Exist<br>99 - Unknown |

**DEPRESSION AT YEAR 1**

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `SuicideF`             | `suicide_attempt_hx_past_year_at_followup` | Interview Question: In the past year, have you attempted suicide? | 0 - No<br>1 - Yes<br>66 - Variable Did Not Exist<br>77 - Refused<br>88 - Not Applicable: Variable not due this year<br>99 - Unknown |
| `PHQPleasureF`         | `phq1` | Interview Question: a. Little interest or pleasure in doing things | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQDownF`             | `phq2` | Interview Question: b. Feeling down, depressed, or hopeless | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQSleepF`             | `phq3` | Interview Question: c. Trouble falling or staying asleep, or sleeping too much | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQTiredF`             | `phq4` | Interview Question: d. Feeling tired or having little energy | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQEatF`               | `phq5` | Interview Question: e. Poor appetite or overeating | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQBadF`               | `phq6` | Interview Question: f. Feeling bad about yourself or that you are a failure or have let yourself or your family down | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQConcentrateF`       | `phq7` | Interview Question: g. Trouble concentrating on things, such as reading the newspaper or watching television | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQSlowF`              | `phq8` | Interview Question: h. Moving or speaking so slowly that other people could have noticed. Or the opposite - being so fidgety or restless that you have been moving around a lot more than usual | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |
| `PHQDeadF`             | `phq9` | Interview Question: i. Thoughts that you would be better off dead or hurting yourself in some way | 0 - Not at All<br>1 - Several Days<br>2 - More Than Half of the Days<br>3 - Nearly Every Day<br>66 - Variable Did Not Exist<br>81 - Not Applicable<br>82 - Not Applicable: No data from person with TBI<br>99 - Unknown |

### Additional TBIMS Variables

| Original Variable Name | New Variable Name | Variable Label                                | Value Labels |
|------------------------|-------------------|-----------------------------------------------|--------------|
| `Mod1id`               | `id`              | Interview Question: ID Number for Participant Record |       |
| `FollowUpPeriod`       | `data_collection_period` | Interview Question: Follow-up period | 1 - Year 1<br>2 - Year 2<br>5 - Year 5<br>10 - Year 10<br>15 - Year 15<br>20 - Year 20<br>25 - Year 25<br>30 - Year 30<br>35 - Year 35 |
| `Birth`                | `date_of_birth`   | Interview Question: What is your date of birth?      | 9999-09-09 - Unknown |
| `Injury`               | `date_of_injury`  | Interview Question: Date of injury | 9999-09-09 - Unknown |
| `Followup`             | `date_of_followup` | Interview Question: Follow-up evaluation date | 4444-04-04 - Expired<br>5555-05-05 - Withdrew Authorization<br>7777-07-07 - Not Applicable: Includes refused, incarcerated, and lost<br>8888-08-08 - Not Applicable: Other<br>9999-09-09 - Unknown         |
| `Death`                | `date_of_death`   | Interview Question: Date of death             | 8888-08-08 - Not Applicable<br>9999-09-09 - Unknown |
| `DeathF`               | `date_of_death`   | Interview Question: Date of death | 4444-04-04 - Expired: Date Unknown<br>8888-08-08 - Not Applicable: Person Alive<br>9999-09-09 - Unknown |
| `IntStatus`            | `status_at_followup` | Interview Question: Interview status | 1 - Followed<br>2 - Lost<br>3 - Refused<br>4 - Incarcerated<br>5 - Withdrew<br>6 - Expired<br>7 - No Funding |

The present study utilizes a retrospective observational design and draws data from the [Traumatic Brain Injury Model Systems](https://msktc.org/about-model-systems/TBI) (TBIMS) longitudinal cohort study. The TBIMS is a well-established multi-center research initiative with extensive data from individuals with TBI throughout the United States.  Time-to-event is assessed using Cox proportional hazards modeling.

### Tools and Packages
This project uses the following R packages:
- [`survival`](https://github.com/therneau/survival)

### References and Documentation
Access and use of the [TBIMS National Database](https://www.tbindsc.org/) (NDB) data is governed by the TBIMS standard operating procedures.
