---
aliases: [Micro, Microbio, "Infectious Disease", "ID"]
tags:
date created: Friday, January 21st 2022, 7:58:27 pm
date modified: Thursday, September 29th 2022, 4:45:44 pm
---
# Infectious Disease
- Medscape articles on ID: https://emedicine.medscape.com/infectious_diseases

## [[Microbes]]
## [[Virology]]
## [[Mycology]]
## [[Parasitology]]
## [[Antimicrobials]]

## Clinical Care
- Antimicrobial Dosing
	- [[Empiric Antibiotics]]
- [[Bacterial Gastroenteritis]]
- [[Bacterial Pneumonia]]
- [[Bacterial Sepsis]]
- [[Cellulitis]]
- C. Difficile
- [[Colon Diverticulitis]]
- [[Diarrhea]]
	- [[Bacterial Diarrhea]]
	- [[Watery diarrhea]]
- Fever of Unknown Origin
- HAP/VAP & Aspiration Pneumonia
- [[01. Topic Notes/Hepatitis B]]
- Hepatitis C
- Herpes Simplex Virus
- [[HIV]] / AIDS & Opportunistic Infections
- [[Influenza]]
- Invasive Fungal Infections
- [[Infective Endocarditis]]
- Meningitis & Encephalitis
- [[Microbe Differentiation]]
- Multidrug Resistant Organisms
- [[Monkey Pox]]
- [[Osteomyelitis]]
- Pneumocystis Prophylaxis
- [[Pneumonia]]
- Skin & Soft Tissue Infections
- STIs
- Tick-Borne Diseases
- Travel Medicine
- [[Tuberculosis]]
- Transplant / [[Immunodeficiencies]]
- [[Urinary Tract Infections]] (UTIs)
- Varicella Zoster
- Viral Respiratorv/Head & Neck Infections
- Infectious [[Infective Endocarditis|Endocarditis]]


# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Microbiology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-ease = "" or !sr-ease)
SORT sr-due ASC
LIMIT 10
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Microbiology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-ease = "" or !sr-ease)
SORT file.mdate ASC
LIMIT 10
```



