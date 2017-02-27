# String.raw
author: alexjmackey

levels:

  - medium

  - advanced

type: normal

inAlgoPool: false

category: must-know

links:

---
## Content

String.raw is used to work with template strings and is best explained with an example:

In JavaScript **\n** is used to indicate a new line.

Consider if we had the following template literal: 
```
`Line1\nLine2!`;
```
When output this would be interpreted as the following as \n signifies a new line:

```
"Line1
Line2"
```

However sometimes it is desirable to work with a string template in its raw format - **String.raw** allows you to do this - note how there is no new line now:

```
String.raw `Line1\nLine2`;
\\"Line1\nLine2"
```

If we were replacing values, expressions are still processed when using String.raw:

```
var company="Enki";
String.raw `Line1\n${company}Line2`;
\\"Line1\nEnkiLine2"
```
---