---
layout: post
title:  "CSS-Preprocessor"
date:   2018-11-17 12:00:00 -0600
tag: assignment

---

# What do you think of pre-compiling CSS?

CSS preprocessors are popular because they’re great tools. These tools have a unique syntax that allows the developer to express the style in a different way (often with more features). 
This website use **sass** (Syntactically Awesome Style Sheets) which is a popular choice. It’s features are Variables, Nesting, Partials,Import, Mixins, Extend/Inheritance and Operators. Since I was introduces to **sass** it’s hard to imagine going back, being able to reduce the code with mixins and import between style sheets is great.

But I must say that my favourite feature is being able to declare variables (no more .txt with hex codes). Declaring variables and expressing them with operators makes sure the website look and feels more like one entity.

In short, I prefer to work with it over regular CSS. It’s less code and more structured. However my favourite feature (variables) are now a part of regular CSS so it might be on the right track. Perhaps it won’t be worthwhile to use a preprocessor in the future if the techniques benefits aren’t greater than using the standard. 

Who knows?

### Which techniques did I use?

This website makes use of most **sass** techniques. The variables are declared on one file, another file styles the basic elements (a, img, ul…) and yet another file styles the layout in more detail and targets classes and ID.

This website is based on the Minima Theme. Instead of rewriting the entire styling I made use of the organized code and added my own style to it. I changed the existing variables and switched many of the variables already assigned to other variables (I guess looks is a matter of taste). There were also some need variables introduced to style the new elements that I created. I kept the existing structure and added the style to the appropriate file.

On the new elements (and existing ones) I worked with nesting whenever possible. The spacing between elements were based on a spacing variable, I had this as the baseline for all the new elements and modified it with operators. So to summarize, the main techniques that I worked with were variables, nesting and operators. The theme Minima contained and made use of all the techniques (more or less) but I didn’t work with them that much since they were already fine.

### Pros & Cons?

I've been a lot pro preprocessors in the text above (I confess).<br>
But here's a list to summarize:

#### Pros:
* More features.
  * Can be a lot more intuitive.
* More options to structure and organize.
* Another alternative to CSS.

#### Cons:
* Complex.
  * More features and tools to learn (and master).
  * More prone to bad practise since it's more complex.
* Slower development
  * The end result **should** be more structured and organized, but development could take longer.
* Debugging
  * More complex means it's harder to solve errors.

Please note that the list above is not some "official" list. Do you disagree or think something is missing?

**Make sure to let me know, leave a comment below.**