# Study on the effectiveness of opioid control policies in the US
This is a team project done in IDS 720: Practical Data Science in 2021 Fall at Duke

In this project, we analyze the effect of drug (in particular, opioid) control policies in Florida, Texas and Washington on the opioid shipments and deaths caused by drug overdose in these states. Florida and Texas implemented policies that had a reductive effect on both opioid shipments and deaths caused by drug overdose. In comparison, Washington did not display a significant effect compared to its control states when measuring these trends.

## Data
- Opioid shipment: all prescription opioid drug shipments in the United States from 2006 to 2012, obtained from Washington Post (https://www.washingtonpost.com/graphics/2019/investigations/dea-pain-pill-database/)
- Overdose death: data on drug overdoses from the US Vital Statistics records, which include data on every death in the United States from 2003 to 2015
- FIPS code
- Population: total population of every county in the US from 2003 to 2015 from the US Census Bureau

## Difference-in-Difference plots
### Florida: policy year 2010

<p align="center">
  <img alt="Light" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/fl_opi_did.png" width="45%">
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Dark" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/fl_deaths_did.png" width="45%">
</p>
<p align = "center">
</p>

### Texas: policy year 2007
Because of the data source limitation, we made plots by month instead of year for Texas opioid shipment.

<p align="center">
  <img alt="Light" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/tx_monthly_opi_did.png" width="45%">
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Dark" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/tx_deaths_did.png" width="45%">
</p>
<p align = "center">
</p>

### Washington: policy year 2012

<p align="center">
  <img alt="Light" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/wa_opi_did.png" width="45%">
&nbsp; &nbsp; &nbsp; &nbsp;
  <img alt="Dark" src="https://github.com/ShiningYang0207/coding_sample_Shining_yang/blob/main/PDS_project/35_modified_plot/wa_deaths_did.png" width="45%">
</p>
<p align = "center">
</p>

## Results

According to the plots above, we can conclude that the opioid control policy in the US was most effective in Florida, where the opioid shipment as well as overdose deaths per capita yield completely reverse (downward) trends after the policy implementation compared to its control states. The 2007 Texas policy is the second most successful one, as after the policy, although the opioid shipments and overdose deaths are still increasing, they yield a much milder and flatter trend compared to the control states. However, the policy doesn’t seem to be effective in Washington, since the trends of the two datasets after the policy are not much different from their control states, and they are still increasing at the same rate before policy implementation.

Upon examination of the opioid control policy implemented in these states, we noticed that Washington’s regulation included doctors having to refer patients to pain specialists if they were taking high doses of opioids and their underlying condition was not improving. In comparison, Florida’s 2007 policy was harsher, involving arrests and fines for pain clinics that were prescribing large quantities of opioids. This could serve as a possible explanation as to why the policy in Florida seemed to have immediate effects on the usage of opioids and deaths caused by drug overdose but Washington’s was not as effective in churning out results.


