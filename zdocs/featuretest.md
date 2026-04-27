---
title: 🍒Zensical featuretest
description: | 
  An overview of extra things zensical supports compared to standard markdown
---

# Zensical featuretest

See <https://zensical.org/docs/setup/extensions/> 

## Tabbed

Documentation:

<https://facelessuser.github.io/pymdown-extensions/extensions/tabbed/>

Example:

/// tab | Tab 1 title
Tab 1 content
///

/// tab | Tab 2 title
Tab 2 content
///

## Tasklist [x]

Documentation:

<https://facelessuser.github.io/pymdown-extensions/extensions/tasklist/>

Example:

[ ] A taks that needs to be done  
[x] A task that is done

Code

```text
[ ] A taks that needs to be done
[x] A task that is done
```


## Tilde -> delete and subscript

Tilde optionally adds two different features which are syntactically built
around the ~ character: 

* delete which inserts `<del></del>` tags and 
* subscript which inserts `<sub></sub>` tags.

Documentation:

<https://facelessuser.github.io/pymdown-extensions/extensions/tilde/>

Examples:

Next word should be 'deleted': ~~deleted~~.

Hydroxycitronellal can be written as C~10~H~20~O~2~

Use this code:

```text
~~deleted~~ double tildes
C~10~H~20~O~2~ single tildes
```

Note: similar effect can be obtained by using Unicode

* d̵e̵l̵e̵t̵e̵d̵
* C₁₀H₂₀O₂

To get this code find out how to enter the correct unicode or  
use an online tools such as 

* <https://yaytext.com/strike/> 
* <https://yaytext.com/tiny-text/>
* <https://jwilk.github.io/chemiscripts/>
