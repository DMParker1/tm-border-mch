# Maternal & Child Health on the Thailand–Myanmar Border

For decades, the Shoklo Malaria Research Unit (SMRU) has provided reproductive and maternal health services to migrant, refugee, and border communities along the Thailand–Myanmar border, with much of this work led by Professor [Rose McGready](https://drrosemcgreadyfoundation.org.au/).

A recurring challenge in this work has been understanding and overcoming barriers to healthcare access. These include the distances between communities and healthcare facilities, transportation difficulties, economic constraints, and restrictions on mobility associated with migration and legal status.

Our research has included efforts to characterize the geography of healthcare access, examine the consequences of barriers to care, and investigate the challenges that remain when healthcare services are brought closer to communities.

---

## Understanding Geographic Barriers to Maternal Healthcare

Pregnant women along the Thailand–Myanmar border have often undertaken long journeys to receive antenatal care (ANC), in some cases traveling entirely on foot. However, systematically identifying the geographic locations of their home communities had been difficult.

The geographic database developed through the Malaria Elimination Task Force ([METF-mapping](https://github.com/DMParker1/METF-mapping)) provided an opportunity to address this problem. Although originally developed to support malaria elimination efforts in eastern Myanmar, the database had applications for other areas of public health research.

A visiting student, [Eric Steinbrook](https://medicine.yale.edu/profile/eric-steinbrook/), worked with historical handwritten ANC records from SMRU and with local Karen staff to cross-validate village names and link the maternal health records to the METF geographic database.

We were able to characterize the geographic distribution of women accessing maternal healthcare by bringing these two previously separate sources of data together; estimate their travel distances, examine changes in clinic catchment areas over time, and investigate relationships between geographic access and pregnancy outcomes.


![Three maps showing changing antenatal clinic catchment areas along the Thailand–Myanmar border in 2007–2009, 2010–2012, and 2013–2015. Colored standard deviational ellipses show the geographic distribution of patients' home villages for four clinics, with catchment areas differing substantially among clinics and over time.](SDEs_PregTravel.png)

*Maps indicating catchment areas for the clinics over time. Each of the four clinics is indicated by a different color scheme. The ellipses are standard deviational ellipses (with 2 and 3 standard deviations), with the darker circle representing roughly 98% of people’s home villages for that specific clinic and the lighter circle representing 99.9% of people’s home villages. WPA (green) and MKT (blue) provided both antenatal care and skilled birth attendants, and MRC (yellow) and WAL (orange) provided antenatal care. These ellipses were originally generated using CrimeStat; a similar process can now be done in R using the [SDEtool](https://github.com/parker-group/SDEtool).*  

*Map from supplemental material in Steinbrook et al. 2021. See citation below.*



---

## Key Findings

- **Late ANC initiation**: Women presenting for antenatal care in the 3rd trimester traveled 50% farther than those enrolled in the 1st trimester (Distance Ratio, DR = 1.5; 95% CI 1.4–1.5).  
- **Loss to follow-up (LTFU)**: Women who dropped out of care traveled 50% farther than those with full-term deliveries (DR = 1.5; 95% CI 1.4–1.5).  
- **Malaria in pregnancy**: Cases of *Plasmodium falciparum* infection were associated with 60% greater travel distance (DR = 1.6; 95% CI 1.6–1.8).  

---

## Implications

- Geographic access to ANC remains a significant barrier.
- The true magnitude of the access gap is unknown (we cannot account for those missing entirely from our data).
- Service delivery models need to reach women in their communities, rather than relying on them to undertake difficult journeys.

---

## Bringing Care to Communities

One approach to overcoming geographic barriers to healthcare is to change the geography of healthcare provision itself.

Beginning in 2021, through the Strengthening Migrant Access to Reproductive Healthcare in Thailand (SMARH-T) initiative, SMRU and the Borderland Health Foundation (BHF), working in collaboration with Thai public health partners, expanded reproductive and maternal healthcare services into migrant communities in Tak Province, Thailand.

While our earlier geographic research included communities on both sides of the Thailand–Myanmar border, this work focused specifically on undocumented Myanmar migrants living on the Thai side of the border.

Outreach teams operating from the two established clinics at Wang Pha and Maw Ker Thai provided antenatal care, family planning, childhood immunization, and healthcare for young children within migrant communities. Beginning with four outreach locations, the initiative eventually provided services at 21 sites, 13 of which remained operational at the time of manuscript submission.

Labor and delivery services, however, continued to be provided at the fixed clinics. Although women could receive routine antenatal care closer to home, they still needed to travel to healthcare facilities for skilled birth attendance.

In collaboration with Drs Mary Ellen Gilder and Rose McGready, and several other colleagues, we investigated factors associated with homebirth among women receiving outreach ANC. This mixed-methods study combined statistical analyses of routine clinical records with postpartum surveys and qualitative interviews to better understand women's experiences, preferences, and barriers to facility-based childbirth.

The quantitative component used mixed-effects logistic regression to investigate individual-level predictors of homebirth while accounting for clustering by outreach site.

### Key Findings

- **Homebirth:** Of 1,593 women who received outreach ANC and subsequently delivered, 183 (11.5%) gave birth at home.
- **ANC attendance:** Each additional ANC visit was associated with 34% lower adjusted odds of homebirth (AOR = 0.66; 95% CI 0.60–0.72).
- **Preferences for place of birth:** Among the 40 women surveyed following homebirth, 70% would have preferred facility-based childbirth.
- **Persistent barriers:** Transportation difficulties, concerns about police checkpoints, and rapid progression of labor contributed to difficulties reaching delivery facilities.
- **Consequences beyond clinical outcomes:** Obtaining birth certificates was an important concern for women who delivered at home, with potential long-term implications for their children.

### Reproducible Research

The statistical analysis code, accompanying data, data dictionary, and documentation for the quantitative component of this study are available in the [SMRU_homebirth repository](https://github.com/parker-group/SMRU_homebirth).

The repository includes the statistical modeling workflow and code for generating predicted probabilities of homebirth across different levels of ANC attendance and by parity.

---

## Broader Implications for Healthcare Access

Together, these studies illustrate complementary approaches to understanding and addressing barriers to maternal healthcare along the Thailand–Myanmar border.

The earlier research focused on characterizing the geographic relationships between populations and healthcare facilities and examining the consequences of barriers to care. The more recent work examined barriers that remain within a decentralized model of healthcare provision.

### Geographic Proximity and Healthcare Accessibility

Bringing healthcare services closer to communities can address some of the barriers associated with geographic distance. However, proximity to healthcare facilities does not necessarily translate into accessibility.

For undocumented Myanmar migrants living in Thailand, the ability to travel is shaped not only by physical geography and transportation infrastructure, but also by economic circumstances, legal status, and interactions with state authorities.

The distinction between a woman's ability to reach a healthcare facility and her preference for receiving care there is particularly important. Homebirth should not necessarily be interpreted as a preference for childbirth outside of healthcare facilities.

These findings illustrate the importance of understanding healthcare access in terms of the circumstances of the populations being served, rather than relying exclusively on geographic measures of accessibility.

### Populations Missing from Healthcare Data

An important limitation of both studies is that they were based on women who had already accessed antenatal care to some extent.

Although we can investigate differences in healthcare utilization and outcomes among these women, we know considerably less about those who remain entirely outside these healthcare services.

Understanding the characteristics, geographic distribution, and healthcare needs of populations missing from routine clinical data remains an important research challenge.

### Connections with Decentralized Malaria Healthcare

There are parallels between this work and our research on decentralized malaria diagnosis and treatment on the Myanmar side of the border.

Through the METF program, malaria posts were established within communities in eastern Myanmar to facilitate [early access to malaria diagnosis and treatment](https://github.com/DMParker1/early-dx-tx). The SMARH-T initiative similarly sought to improve access to maternal and reproductive healthcare by providing selected services within migrant communities in Thailand.

Although the health conditions, populations, and political contexts differ, both approaches involve reorganizing healthcare provision around the geography and circumstances of the populations in need of care.

The relationship between these research programs is therefore both methodological and practical. Geographic data collected through the METF program enabled research into maternal healthcare accessibility, while the decentralized models of healthcare provision used in both programs reflect a shared principle: taking healthcare to people where possible, rather than expecting people to overcome substantial barriers to reach healthcare.

This also highlights the importance of linking community-based services to referral systems and facilities capable of providing more specialized care.

---

## 🔗 Related Repositories

These repositories connect different parts of my spatial epidemiology research:

- [research-atlas](https://github.com/DMParker1/research-atlas) — Research atlas connecting projects across questions, places, and approaches.
- [earth-observation-hub](https://github.com/DMParker1/earth-observation-hub) — How Earth Observation methods became central to my work, with curated papers and case studies.  
- [activity-spaces](https://github.com/DMParker1/activity-spaces) — Research on multi-place exposure (farm huts, GPS, mobile phone data) and its health relevance.  
- [METF-mapping](https://github.com/DMParker1/METF-mapping) — Mapping malaria post placement & community engagement.  
- [tMDA-program](https://github.com/DMParker1/tmda-program) — Targeted mass drug administration trials & modeling.  
- [early-dx-tx](https://github.com/DMParker1/early-dx-tx) — Early access to malaria diagnosis & treatment.  

---

---
