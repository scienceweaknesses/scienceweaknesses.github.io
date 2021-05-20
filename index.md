## A change-centric technique to DETECT and FIX weaknesses in configurable systems

### Abstract

Configurable systems developed in C use #ifdef directives to deal with variability and portability. Developing and evolving highly configurable systems is a complex task because developers need to deal with many configurations at the same time and weaknesses can be easily added and difficult to detect since some weaknesses belong to only a few specific configurations. This process makes the task of detecting and fixing weaknesses even more challenging because most static analysis tools are not variability-aware. In addition, to the best of our knowledge, there is a lack of studies that analyze how to automate the process of fixing weaknesses in configurable systems. We study two types of weaknesses (Null Pointer Dereference and Memory Leak) and observe a pattern used by many developers to fix them. In this work, we propose a change-centric technique to detect and fix weaknesses in configurable systems. We evaluate our proposal in 14 open projects available in the GitHub repository. To confirm the weaknesses detected and fixed, we send 12 pull requests to fix 65 Null Pointer Dereference and 5 Memory Leak. So far, experts analyzed 6 pull requests and confirmed all weaknesses reported in these patches (27 Null Pointer Dereference and 5 Memory Leak). The other pull requests are still open waiting for the developers to evaluate

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

Here's an image of a drag racer in action:

![Drag Racing](technique.jpeg)

Move along.


```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/scienceweaknesses/scienceweaknesses.github.io/settings/pages). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
