Here's how to replace blanks (spaces) with hyphens in JavaScript:

## Basic solution:
```javascript
let inputstring = "My fist-web page";
let outputstring = inputstring.replace(/ /g, '-');
console.log(outputstring); // "My-fist-web-page"
```

## To also replace multiple spaces and handle special cases:

```javascript
let inputstring = "My fist-web page";
let outputstring = inputstring.replace(/\s+/g, '-');
console.log(outputstring); // "My-fist-web-page"
```

## Complete example with your exact input:
```javascript
let inputstring = "My fist-web page";
let outputstring = inputstring.replace(/ /g, '-');
console.log(outputstring); // "My-fist-web-page"
```

## If you want to replace ALL whitespace (spaces, tabs, etc.):
```javascript
let inputstring = "My fist-web page";
let outputstring = inputstring.replace(/\s/g, '-');
console.log(outputstring); // "My-fist-web-page"
```

## To also convert to lowercase (common for URLs/slugs):
```javascript
let inputstring = "My fist-web page";
let outputstring = inputstring.toLowerCase().replace(/ /g, '-');
console.log(outputstring); // "my-fist-web-page"
```

## Function version:
```javascript
function convertToSlug(str) {
    return str.replace(/ /g, '-');
}

let inputstring = "My fist-web page";
let outputstring = convertToSlug(inputstring);
console.log(outputstring); // "My-fist-web-page"
```

**Note:** Your example shows "My fist-web page" → "My-fist-web-page" (only spaces become hyphens). The existing hyphen in "fist-web" remains unchanged.