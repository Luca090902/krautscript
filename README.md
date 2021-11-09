[KrautScript](https://luca090902.github.io/krautscript/)
==========
![German Flag](/assets/img/flag.png)  
KrautScript lets you write JavaScript in German; Finally there is a way for Germans to code in their native language!

See it in action [here](https://luca090902.github.io/krautscript/). 
### Including KrautScript files in your HTML

- Include [krautscript.js](dist/krautscript.js) and [krautscript.browser.js](dist/krautscript.browser.js).
- Make sure your html is set to allow utf-8 characters (add `<meta charset="utf-8">` in the `<head>`).

KrautScript supports the `text/krautscript` MIME type. Any script tag with that type will be compiled and run automatically:
```html
<script type="text/krautscript">
  wenn (x < 5) {
    konsole.log("Ja!");
  } ansonsten {
    konsole.log("Nein!");
  }
</script>
```

You can also specify a `src` for your script tags: 
```html
<script type="text/fikascript" src="snaps.fika"></script>
```

#### Optional

##### Convert from KrautScript to JavaScript:

```javascript
KrautScript.germanToEnglish(code); // returns a string representing the translated code
```

##### Convert from JavaScript to KrautScript:

```javascript
KrautScript.englishToGerman(code); // returns a string representing the translated code
```

### Missing/incorrect translations?
You can see the translations over [here](https://github.com/pushmatrix/fikascript/blob/gh-pages/dist/krautscript.js#L4). Feel free to submit a pull request!

###TO-DOs
- Translation
