Small Group Notes: [[MSK.pdf]]
Anatomy Notes: [[Notability/Basic Science/Anatomy/Shoulder and axilla.pdf]]

Related Notes
[[Pediatric Bone and Joint Issues|Peds MSK]]


"The physical exam is to diagnose, the MRI is to plan the surgery."

- [[Back Pain]] - *Stat Pearls*
- Elbow Pain
- Foot & Ankle Disorders
	- [[Achilles Tendinitis]]
- Fibromyalgia
- Glucocorticoids and Disease-Modifying Antirheumatic Drugs
- Gout & Pseudogout
- Hand Disorders
- [[Hip Pain]]
- Joint Pain and Monoarticular Arthritis
- [[Knee Pain]]
- [[Lupus]]
- Myalgias
- Myositis
- [[Osteoarthritis]]
- Polyarticular Arthritis
- Polymyalgia Rheumatica
- Rheumatologic Tests
- [[Rheumatoid Arthritis]]
- [[Shoulder Pain]]

# <mark>Time To Review:</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[MSK]]) OR ([[Lupus]]) OR ([[Osteoarthritis]]) OR ([[Pain]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE sr-due <= date(today) + dur(3 day)
WHERE !(sr-ease = "" or !sr-ease)
SORT sr-due ASC
LIMIT 10
```
# <mark>New To Learn</mark>
```dataview
TABLE sr-due AS "Due", sr-ease AS "Ease", file.mtime AS "Modified"
FROM outgoing([[MSK]]) OR ([[Lupus]]) OR ([[Osteoarthritis]]) OR ([[Pain]]) AND (#review OR #reviewcard OR #reviewtopicnote)
WHERE (sr-ease = "" or !sr-ease)
SORT file.mdate ASC
LIMIT 10
```