---
layout: essay
type: essay
title: "How Important is Coding Standards?"
date: 2024-09-25
published: true
labels:
  - Coding Standards
  - Community
---
<img class="img-fluid" src="../img/lint.avif" width=40% height=40%>

## Practicing Coding Standards
After using ESLint for about a week, I think it is only mildly annoying and does not do anything to help understanding of the code. Perhaps there are more to ESLint rules than the ones I have seen so far but little details like spaces before braces are just personal choices, doing nothing for the coder. While my experience with ESLint and TypeScript overall is very limited, my time in ICS212 has proven to me that there are bad practices of coding standards. Since we wrote code in the terminal and the school's Unix system, every detail has to be manually fixed. When our programs got quite big towards the end of the semester, it was a pain to check every file and every line of code to make sure it matches the professor's coding format. Even though that is a fault with the IDE, the standard itself did nothing to improve understanding of the code. The only thing beneficial is that we had a large comment block before each function to give details about the function. Other than that, using four spaces versus a tab, limiting to one return call, putting opening braces in the next line, and many others, only did so much as wasting more time than necessary. Instead of thinking how to implement functions, I had to waste time and effort making sure my code looks neat and clean in accordance to one person.

## How it Could Actually Help
I do believe that using coding standard could be a huge help in learning the langauge however. Many complex functions and method calls would look very daunting if not seperated by line. For example: 
```
numbers.filter(num => num % 2 === 0).map(num => num * num).reduce((sum, num) => sum + num, 0)
```

This seems confusing, cramp, and does not allow for comments per line/method call. However, if you formatted it like this:
```
numbers
  .filter(num => num % 2 === 0)         // Filter even numbers
  .map(num => num * num)                // Square even numbers
  .reduce((sum, num) => sum + num, 0);  // Sum the squares
```

This is easier to digest line by line and it allows us to explain what each method does before it is chained. I think there more examples out there where good coding standards makes a larger difference than just a couple of spaces. Outside of code readabilty, using a standardized coding format helps other people be able to read your code and also allows code spread across different files and different people to stay consistent. I think the best coding standards I have used so far is meaningful variable name, camel casing, and limit nested if-else statements. These has become more of coding habits than standards and I think that's what all coding standards should strive to achieve. Not a guideline to follow but something that feels natural and intuinitive.
