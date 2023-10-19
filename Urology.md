## Men's Health Topics
- Infertility
- [[Hematuria]]
- Sexual Dysfunction
- Male Hypogonadism
- Prostate Cancer
- STDs
- BPH
- Prostate Cancer
- Prostatitis
- [[Scrotal & Testicular Lesions]]
- [[Placing A Foley]]

### Consulting:
- Please call us for foley on an immediately postop urology patient. 
- NEVER place a foley in a guy who’s had a prostatectomy or any sort of urethral anastomosis in the past 4 weeks (that is a urology-only job), and call me to check if it’s ok before attempting a foley if they are within 2 months postop. 
- Please have a bladder scan value when you call or I will be sad.
# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Urology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-ease = "" or !sr-ease)
SORT sr-due ASC
LIMIT 10
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[Urology]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-ease = "" or !sr-ease)
SORT file.mdate ASC
LIMIT 10
```
