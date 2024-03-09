## Data Modelling

```json
{
	"title": "string",
	"author": "reference",
	"image": "string.url",
	"description": "string",
	"category": "reference",
	"date": "Date",
	"crosswords": "reference.array"
}
```


## Bookmarks
```json
{
	"title": "string",
	"urlId": "string.url.pathname"
}
```


## Category
```json
{
	"name": "string",
	"description": "string"
}
```


## Series Markup
```jsx
	<Tag />
	<Title />
	<SeriesCount />
	<Author />
	<Description />
	<ul>
		{crosswords.map(crossword => 
			(<li><SeriesCard data={crossword} /></li>)
		)}
	</ul>
```


## Archive

```jsx
<Title /> // {Series|Crosswords|Trivia} Archive
<slot name="more">
	<Quote>This is an article about `${series}`, For trivia,  Go <a href>here</a></Quote>
</slot>

<ul>

	{allData.map((data) => {
		<Card
			category={data.category}
			categoryLink={data.categoryLink}
			author={data.author}
			description={data.description}
		 />
	})}

</ul>
```