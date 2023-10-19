---
Aliases: ["Gastroenterology","GI", "Gastro"]
---

[[Hepatology]]
# GI Topics
- [[Acute Liver Failure]]
- [[Abdominal Pain]]
- [[Alcoholic Hepatitis]]
- Biliary Disease
- [[Bilious Vomiting]]
- [[Bowel Obstruction]]
- [[Bowel Regimen]]
- Celiac Disease
- [[Cirrhosis]]
- [[Colorectal Carcinoma|Colon Cancer]]
- [[Constipation]]
- Diverticular Disease
- [[Diarrhea]]
- Dysphagia
- End Stage Liver Disease
- [[Esophagus]]
- [[Functional Abdominal Pain]]
- Gallstones
- [[GERD]]
- [[GI bleed|GI Bleeding]]
	- [[GI Vascular Lesions]]
- H. Pylori
- Hemorrhoids
- [[Hepatic hydrothorax]]
- [[Hepatorenal syndrome]]
- Inflammatory Bowel Disease
- Irritable Bowel Syndrome
- Liver Chemistry Tests | [[LFTs|LFT]]
- Liver Transplant
- Motility Disorders & Celiac Disease
- NAFLD
- [[Nausea]]
- [[Non-Bilious Vomiting]]
- [[Nutrition]] & Feeding
- Pancreatic Disease
- Pancreatitis
- Peptic Ulcer Disease
- Weight & Weight Loss



# <mark>Time To Review:</mark>

```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[GI]]) AND (#review OR #review/card OR #review/topicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-ease = "" or !sr-ease)
SORT sr-due ASC
LIMIT 10
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[GI]]) AND (#review OR #review/card OR #review/topicnote)
WHERE (sr-ease = "" or !sr-ease)
SORT file.mdate ASC
LIMIT 10
```
