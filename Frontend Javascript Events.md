# Javascript Events


## Chat

**chat:loaded**

```
app.on("chat:loaded", function(event){
  // Do Stuff
});
```

## Event

**event:loaded**

Called after the initial event data has been loaded and after the bare bone view has been rendered.

```
app.on("event:loaded", function(event){
  // Event Loaded
});
```

## Slide

**slide:click**

Slide clicks return a backbone model with information about the slide that was clicked. [Backbone Models](http://backbonejs.org/#Model)

```
app.on("slide:click", function(event, slide_info){
	alert( slide_info.get("title") );
});
```

**Slide Model Attributes**

```
{
  "content": "<p>Example HTML</p>",
  "linkUrl": "http://example.com",
  "imageUrl": "http://example.com/example-image.jpg",
  "title": "Poll Slide #1",
  "kind": "Poll",
}
```