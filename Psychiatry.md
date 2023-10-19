---
Alias: [Psych, Psyc, Psychology]
---
# Psychiatry
- Medscape articles on psych: https://emedicine.medscape.com/psychiatry
- [[Psych Templates]]
- [[Psych Research Papers]]
- [[03. Attachments/Notability/Rotations/Psych/Psych Final SG 2020.pdf|Psych Final Notes]]
- [[Psych Pharm]]
## Pathologies
- [[Alcohol Use Disorder]]
- [[Anxiety]] Disorders
- Attention-Deficit Hyperactivity Disorder
- ADHD
- Bipolar Disorder
- [[Cannabis Use Disorder]] - Statpearls
- [[Corticosteroids]]
- [[Depression]]
- Eating Disorders
- Insomnia and Sleep Disorders
- [[Major Neurocognitive Disorders]]
- [[OCD]]
- Opioid Use Disorder
- Posttraumatic Stress Disorder (PTSD)
- [[Psychotic Disorders]]
- Personality Disorders
- [[Psych Pharm]]
- Schizophrenia
- [[Sedation & Aggression]]
- Somatic Symptoms and Related Disorders
- Substance Use & Addiction
- Suicide Risk Assessment
- Tobacco Use
- [[Our Most Lacking Resource is Listening - History, Chemistry, and Treatment of Borderline Personality Disorder]]



# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Psychiatry]]) OR ([[Addiction Medicine]]) OR ([[Depression]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-ease = "" or !sr-ease)
SORT sr-due ASC
LIMIT 10
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Psychiatry]]) OR ([[Addiction Medicine]]) OR ([[Depression]]) OR ([[Anxiety]]) OR ([[Psych Pharm]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-ease = "" or !sr-ease)
SORT file.mdate ASC
LIMIT 10
```
