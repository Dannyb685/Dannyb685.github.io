---
aliases: 
tags: 
date created: Saturday, June 18th 2022, 6:21:34 pm
date modified: Thursday, February 16th 2023, 1:03:03 am
---
Memory Loci : [[CU Boulder Library]]

# Pulm Notes
[[Pediatric Pulmonology]]
[[Calling Pulm Consult]]
[[PFTs.+and+Pulm+PE.pdf ___2022-12-14 at 23.50.09@2x.png|Respiratory Physical Exam]]

# Pulmonology Topics
- [[ARDS]]
- [[Asthma]]
- [[Bronchiectasis]]˝
	- [[01. Topic Notes/Bronchiectasis Physical Exam Template]]
- [[COPD]]
- [[Cough]]
- [[Chronic Bronchitis]]
- [[Chronic Cough]] - _Statpearls_
- ECMO
- [[Interstitial Lung Disease]]
- [[Hypoxemia]] & Hypercapnia
	- [[Hypoxia & Hypoxemia.jpeg]]
- [[Hemoptysis]]
- [[Lung Cancer]]
- Mechanical Ventilation
- Noninvasive Oxygenation/Ventilation
- Obstructive Sleep Apnea
- [[Pneumonia]]
- [[PFTs|Pulmonary Function Tests]]
- [[Pulmonary Embolism]]
- [[Pleural Effusion]]
- Pulmonary Nodules
- [[Pulmonary Hypertension]]
- [[Respiratory Distress]]
- [[Respiratory Failure]]
- [[Sepsis & Septic Shock]] ([[Bacterial Sepsis]])
- [[Sedation & Aggression]]
- [[VTE]]
- [[Vasopressors]]
- Toxicology

# Various Pathologies
- [[Nasopharyngeal carcinoma]]
- [[Angiofibroma]]
- [[Acute Epiglottitis]]

# Pulmonology Quick Quiz
## Step 1
- Location that maxillary sinuses drain to = <b>middle nasal meatus</b>
- Blockage = <b>rhinosinusitis</b>
- Epistaxis:
	- Anterior bleeding source = <b>Kiesselbach plexus</b>
	- Posterior bleeding source = <b>sphenopalatine artery</b>
		- (life-threatening!)
- Smoker now has ulcer in throat/neck/tongue/mouth = <b>squamous cell carcinoma</b>
- Pregnant patient with difficult labor now has SOB and DIC = <b>amniotic fluid</b> embolism
- Patient who broke their hip several days ago now has SOB, confusion, petechial rash = <b>fat embolism syndrome</b>
- Patient with COPD + coughing up tons of crap for ≥3 months in a year for 2+ years = <b>chronic bronchitis</b>
	- Reed index tells <b>severity</b>
- Farmer has SOB, cough, headache every time he goes to work but it gets better when he's home on the weekend = <b>hypersensitivity pneumonitis</b>
	- Type III/IV hypersensitivity reaction, not Type I
- Patient with SOB and cough tells you they own a bunch of exotic parrots = <b>hypersensitivity pneumonitis</b>
- Can you measure VC by spirometry?  <b>yes, doesn't include RV</b>
	- ![[Pasted image 20230906000343.png]]
-  
## Step 2/3




---

# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Pulmonology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-due = "" or !sr-due)
SORT sr-due ASC
LIMIT 10
```

---

# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Pulmonology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-due = "" or !sr-due)
SORT file.mdate ASC
SORT sr-ease ASC
LIMIT 10
```
