## Some Important questions 

### What is import React from 'react' and why this is so important ?
- import React from 'react' simply imports React from the module named react , we need it because we write JSX inside react and in order to use JSX inside we need to import react as to make our code understand to  browser babble convert our JSX code to browser understandable react code in which their is a method react.creactElement is present inside React module
**Code We Write**
```
import React from 'react';
import React-Dom from 'react-dom';

ReactDom.render(<h1>Hello World</h1>,
document.getElementById("root");
)


What babble turn this to for our browser to understand 
Reactdom.render(react.CreateElement("h1,
null,
"Hello World),
document.getElementById("root"));

```


### why we need to import React-Dom


### what are single page application , benifits etc
