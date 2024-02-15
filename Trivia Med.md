## Data Modelling 
```json
{
	"title": "string",
	"author": "object",
	"category": "string",
	"description": "string",
	"image": "string.url.maybe?",
	"date": "Date",
	"words": [
		{
			"word": "string",
			"clue": "string",
			"image": "string.url.optional"
		}
	]
	
}
```


## Normal Mode
- Ask for clues and support images

## Timed Mode
- Have a `/d` seconds timer restart when one finishes each question and end the game if the timer ends before the user is able to

## Survival Mode
- Answer as many questions as possible in `/d` minutes