# karen-embed

> [Karen](https://karenapp.io)  integration for html websites


## Include this script file

```html
<script type="text/javascript" src="https://kassets.s3.eu-west-3.amazonaws.com/html/karen-widget.js"></script>
```

## Include this css file
```html
<link href="https://kassets.s3.eu-west-3.amazonaws.com/html/widget.css" rel="stylesheet">
```

## Documentation

To embed inline widget use
```html
...
<div id="karenRendersHere"></div>
...
<script>
	Karen.initInlineWidget({
		url: '<user events url from karen account>',
		parentElement: document.getElementById('karenRendersHere'),
	});
</script>
```
To embed popup widget use
```html
<script>
 	Karen.initBadgeWidget({
		url: '<user events url from karen account>', 
		text: 'Sign Up For an Event', 
		color: '#12f4f2', 
		branding: true
	});
</script>
```
To embed popup text use
```html
<button onclick="Karen.showPopupWidget('<user events url from karen account>');return false;"> register </button>
```

