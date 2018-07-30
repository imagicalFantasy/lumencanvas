# LumenCanvas
LumenCanvas is an open source HTML5 drawing tool based on Fabric.js & JQuery. You can use it to embed drawing boards in web pages. You can save the drawings as a string or JSON and you can retrive it again. LumenCanvas is an object based drawing tool. You can move the drawn objects around and change the border of the filling color.

### Online Demo Link
[Click Here...](http://wizvalley.com/paint/)

### Example
```js
  new LumenCanvas({selector : ".drawing-canvas"})
```

### How to call a method
```js
  var LumenCanvasInstance = $(".drawing-canvas").data("LumenCanvas");
  var jsonData = LumenCanvasInstance.GetJSON();
```

### Options
Here's a list of available settings.
```js
new LumenCanvas({
    selector : "",
		textStetting: {familty:'Arial',size:16},
		spellcheck: false, /// set this true if you want to enable spellcheck in text tool
		width : window.innerWidth-100, // default will be window width
		height : 548,
})
```

### GetJSON
 Returns a json object that represents the drawing area.
 
### GetDataString
 Returns stringified json object that represents the drawing area.
 
 ### SetJSON(json) @param {json} fabric js JSON object.
 Set the drawing area to the passed object.

 ### GetDataURL(options) @param {options} see below defaultOptions object.
 Open the drawing in a new tab or return the URL string.
 ```js
 var defaultOptions = {
		format: 'png',
		left: 0,
		top: 0,
		width: 500,
		height: 350,
		openInNewTab : false
	}
```
 
 
