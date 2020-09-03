## Some Important questions 

### What is import React from 'react' and why this is so important ?
- import React from 'react' simply imports React from a module named react , we need this import because we need `react.CreateElement` which is inside react module , we dont direct write this but we write JSX inside react and in order to use JSX inside we need to import react because babble convert our jsx code to browser understandable react code in which method react.CreateElement is present.

**Code We Write**
```
import React from 'react';
import React-Dom from 'react-dom';

ReactDom.render(<h1>Hello World</h1>,
document.getElementById("root");
)
```

**What babble turn this to for our browser to understand** 

```
Reactdom.render(react.CreateElement("h1,
null,
"Hello World),
document.getElementById("root"));

```


### why we need to import React-Dom
- Because we need render() function , which is present inside react-dom module 

### What is use of render() function 
- The ReactDOM. render() function takes two arguments, HTML code and an HTML element. The purpose of the function is to display the specified HTML code inside the specified HTML element.

### what is a single page application .
- Single page application literraly means a single page , every thing is on a single page , think of our daily life example ,like Facebook , Instagram even Whatsapp , all these are examples of single page application , 


**In technical terms**
- A single page application is that which interacts with the browser in the same page and to open a new link it rewrites the current page and loads the data on that page from the server , not like opening n different tabs for each link .


**Benifits of single page application**
- They do not reload during the use.
- They do not use to open different page for other links and we don't need to wait for the new page to load.
- They improve UX(User Experience).
