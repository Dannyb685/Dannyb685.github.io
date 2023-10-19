---
Alias: [FM, "Family Med", "Fam Med", GIM, "General Internal Medicine", "Primary Care Internal Medicine"]
---
Return to [[10 - Medicine]]
# Related Notes
- [[Primary Care Intern Learning Plan]]
- [[IM Hospitalist vs FM]]
- [[FM Is A Tough Field]]
- [[Dialogue & Pt Teaching]]
- [[Where Primary Care Happens]]
- [[Why Primary Care]]
- [[PCP Shortage]]
- [[Fixing Primary Care]]
- [[How to Call A Consult]]
- [[Primary Care Consulting]]
- [[Homelessness]]
- [[Baltimore HCH]]
- Chronic disease outcomes
- Staff efficiency and timeliness
- Evaluate for operational deficits
- [[Agenda Setting Form]]
- [[Healthcare Futurism|Future of heatlhcare]]
	- At home UA and CBC?
		- Specifically microalbumin/cr
	- What tests wouldn't work through the mail?
	- How to design cities for healthier communities?
- [[The Future of Preventive Medicine and Public Health in a Changing Primary Care Landscape]]
	- Health Care should be affordable and accessible for everyone.
# Common PC Topics
- [[Health Screening & Maintenance]]
- [[Arthrocentesis]]
- [[Chronic Headaches]]
	- [[Migraine]]
- [[Chronic Cough]]
- [[Chest Pain]]
- [[Colon Cancer Screening]]
- [[Complex Wound Management]]
- [[Constipation]]
- [[Contact Dermatitis]]
- [[Well Visit With Known Patient]]
- [[Well Child]]
- [[HEENT]]
- [[Diabetes|DM]]
- [[Dyslipidemia|HLD]]
- [[Cholesterol]]
- [[Back Pain]]
- [[Bacterial Diarrhea]]
- [[Bacterial Gastroenteritis]]
- [[Depression]]
- [[Hypertension]]
- [[CKD]]
	- [[Albuminuria]]
- [[MSK]] 
- [[Healthcare For The Homeless]]
	- [[Homeless-Klein-pages-1-11.pdf|Care of the Homeless Patient - Klein]]
- [[Colon Cancer Screening]]
- [[Constipation]]
- [[Chest Pain]]
- [[Bacterial Diarrhea]]
- [[Back Pain]]
- [[Depression]]
- [[GI bleed|GI Bleeding]]

## Primary Care [[Procedures]]
- Colposcopy/LEEP
- Colonoscopy
- Endoscopy
- Musculoskeletal iniections
- Spirometry
- Skin procedures
- Suturing lacerations 
- [[Ultrasound]] imaging 
- [[Vasectomy]]
## Additional Topics
- Transgender Health 
- Women's Health 
- Postpartum & Sleep Medicine 
- Immigrant & Refugee Health 
- Climate Change & Health
- Pain Management 
- [[Advance Care Planning]] & Code Status 
- End of Life & Pronouncement 
- Comfort Focused Care & Hospice 
- Frailty & Polypharmacy
- Skin Cancer
- Psoriasis
- Acne
- Alopecia
- Wounds
## [[Anticipatory Guidance]]
- [[Rear facing car seats]]

## Articles
- [Interprofessional primary care practice including social workers: exploring the experiences of patients in vulnerable situations](https://www.tandfonline.com/doi/full/10.1080/13561820.2021.2015302)
	- The link between social inequality and health has been widely recognized, as there are systematic differences in health between people from lower and higher social classes. Furthermore, the complexity and multidimensionality of health and social problems has resulted in primary health care services that are increasingly integrating the approach of interprofessional collaboration between medical professionals and social workers. Despite this current focus, there is a lack of empirical insights into patients’ experience of the quality of care resulting from these collaborations. This paper aims to contribute to knowledge by adopting a research approach that captures the narratives of patients in vulnerable situations from a primary care center by conducting semi-structured interviews. Through content analysis, data was analyzed according to five themes: (1) availability, (2) accessibility, (3) affordability, (4) comprehensibility, and (5) usefulness. The results suggest a positive role for interprofessional collaboration between medical professionals and social workers within a primary health care setting. This includes the opportunity for giving greater attention to social rights and collaboration within the local community.
- 

---

# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Primary Care]]) 
SORT sr-due ASC
SORT date-created ASC
SORT sr-ease ASC
WHERE sr-due >= date(today) - dur(31 day)
LIMIT 5
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Primary Care]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-due = "" or !sr-due)
SORT file.mdate ASC
LIMIT 20
```
