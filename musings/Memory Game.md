---
github: https://github.com/Ikuewumi/memory-game
---
# Data Modelling

## Quiz
```json
{
	"title": "string",
	"author": "reference(author)",
	"image": "string.url",
	"date": "Date.maybe?",
	"difficulty": "easy | medium | hard",
	"description": "string",
	"text": "string.optional",
	"questions": "array(question)"
}
```

## Question
```json
{
	"question": "string",
	"answer": "string",
	"text": "string.optional",
	"image": "string.url.optional",
}
```
## Series
```json
{
	"title": "string",
	"author": "reference(author)",
	"image": "string.url",
	"description": "string",
	"course": "reference(course)",
	"quizzes": "reference.array(quiz)"
}
```

## Course
```json
{
	"title": "string",
	"description": "string",
	"icon": "svg's href"
}
```

## Author
```json
{
	"name": "string",
	"image": "string.url",
	"description": "string",
	"links": {
		"email": "string",
		"github": "string",
		"facebook": "string",
		"twitter": "string"
	}
}
```



---
# Data
This entails the order in which I intend to start adding quizzes

## Anatomy
1. Anatomy 101, terminologies 
2. Cell and Organelles
3. intercellular junctions
4. Types of Tissues
5. Cell Division
	1. More Definition 
	2. Mitosis
	3. Meiosis

## Pharmacology
1. Basics
	1. Pharmacokinetics 101
		1. Terminologies
		2. 
	2. Pharmacodynamics 101
	3.  


---
# Courses
- heading
- course
	- icon
	- title
	- description

# Course Page
- {d} title
- {d} description
- tabs system (Cuizzes (_n_) | Series (_n_) )

# Series Page
- {d} title
- A {n}-cuiz series
- description
- {d} bg-image 




