# Javascript Splash Page

![alt text][javascript]

[javascript]: https://github.com/yourwpmadesimple/javascript-navigation-animation/blob/master/javascript_banner.jpg "Javascript Banner"

## Final Code
```javascript
const { body } = document;

// Change Background
function changeBackground(number) {
  // Check if background already showing
  let previousBackground;
  if (body.className) {
    previousBackground = body.className;
  }
  // Reset CSS class for body
  body.className = "";
  // Get the return value from the top buttons
  console.log(number);
  switch (number) {
    case "1":
      return previousBackground === "background-1"
        ? false
        : body.classList.add("background-1");
      break;
    case "2":
      return previousBackground === "background-2"
        ? false
        : body.classList.add("background-2");
      break;
    case "3":
      return previousBackground === "background-3"
        ? false
        : body.classList.add("background-3");
      break;
    default:
      break;
  }
}
```