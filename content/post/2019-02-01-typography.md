---
title: "Typography"
date: 2019-02-01T21:56:55+02:00
draft: false
dropCap: true
description: "Typography and styles of the posts, this is the description of the post (displayed in the post's card)"
featuredImage: "img/20190201-featuredImage-typography.png"
featuredImageDescription: "Description for the featured image, used as the alt text"
displayInMenu: false
categories: ["About"]
tags: [ "typography", "About"]
displayInList: true
---

# Heading 1

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis explicabo nam commodi eos cumque possimus error cupiditate iste doloribus aut porro, beatae impedit, corporis sapiente laudantium id voluptatem sit distinctio sed sequi accusantium molestias, facilis sunt eum? Voluptates sit numquam, recusandae deleniti illo, nisi maxime sequi eligendi ad veniam quidem molestias aut assumenda doloremque delectus modi animi. Sint asperiores minus ducimus aut aliquid eos pariatur, id doloribus rem natus quam, adipisci reprehenderit? 

---

## Heading 2

### Heading 3

#### Heading 4

##### Heading 5

###### Heading 6

---

## Text

**bold**

_italic_ 

[link](https://www.google.com/)


Lorem ipsum dolor sit amet, consectetur adipisicing elit. Debitis explicabo nam commodi eos cumque possimus error cupiditate iste doloribus aut porro, beatae impedit, corporis sapiente laudantium id voluptatem sit distinctio sed sequi accusantium molestias, facilis sunt eum? Voluptates sit numquam, recusandae deleniti illo, nisi maxime sequi eligendi ad veniam quidem molestias aut assumenda doloremque delectus modi animi. Sint asperiores minus ducimus aut aliquid eos pariatur, id doloribus rem natus quam, adipisci reprehenderit? Architecto quis dignissimos porro pariatur impedit at odio illo ab sunt obcaecati eius consectetur distinctio, eligendi fuga sint fugit aspernatur ratione blanditiis veniam voluptates? Delectus magni optio voluptate odit incidunt nobis officiis mollitia fuga libero, reprehenderit fugit. 

Hic eos earum ipsum, reprehenderit, ut facere officiis vitae voluptas sunt atque quisquam, nobis deleniti sapiente laudantium quia libero nulla rerum beatae mollitia iusto similique! Nesciunt illo, harum facilis aperiam commodi. Amet perferendis voluptatem, itaque laboriosam, eos minima vero tempore at!

---

## Ordered List

```md
1. Number one
2. Number Two
    1. Indented Number 1
    2. Indented Number 2
```

1. Number one
2. Number Two
    1. Indented Number 1
    2. Indented Number 2

---

## Unordered List

```md
* Get groceries at Harris Teeter before the party
* Get a Spider Man cake
    * Chocolate or marble
    * Whipped cream frosting
* Don't forget to walk the dog before you leave
* Bring lots of plates and silverware so that we don't run out
    * Plastic Dixie brand is fine
```

* Get groceries at Harris Teeter before the party
* Get a Spider Man cake
    * Chocolate or marble
    * Whipped cream frosting
* Don't forget to walk the dog before you leave
* Bring lots of plates and silverware so that we don't run out
    * Plastic Dixie brand is fine

---

## Blockquote 

```md
> This is in a blockquote
  and a second line
```

> This is in a blockquote
  and a second line

---

## Tables

```md
| table heading 1 | table heading 2 | table heading 3 |
|---|---|---|
| row 1 content 1  | row 1 content 2  | row 1 content 3  |
| row 2 content 1  | row 2 content 2  | row 2 content 3  |
| row 3 content 1  | row 3 content 2  | row 3 content 3  |
```

| table heading 1  |  table heading 2  |  table heading 3 |
|---|---|---|
| row 1 content 1  | row 1 content 2  | row 1 content 3  |
| row 2 content 1  | row 2 content 2  | row 2 content 3  |
| row 3 content 1  | row 3 content 2  | row 3 content 3  |

A helpful tool for generating markdown tables [Markdown Tables Generator]( https://www.tablesgenerator.com/markdown_tables)

---

### Footnotes

```md
Footnotes[^1] 
[^1]: Footnote: this is a footnote!
```

Footnotes[^1] are also part of markdown features. So easy to create!
[^1]: Footnote: this is a footnote!

---


## Images

```md
![NYC Skyline](/img/20190201-featuredImage-typography.png)
```

![NYC Skyline](/img/20190201-featuredImage-typography.png)

### Small Images

```md
{{</* smallimg src="/img/20190201-featuredImage-typography.png" alt="typography" smartfloat="left" width="250px" */>}}
```
{{< smallimg src="/img/20190201-featuredImage-typography.png" alt="typography" smartfloat="left" width="250px" >}}

This image floats to the left of this paragraph and is 250px wide. Its aspect ratio is maintained so it will not stretch. The picture shows the New York skyline. You can see how the design is responsive and how the cards intelligently fit to the display. With flexbox and css grid, heavy frameworks such as bootstrap aren't necessary to create beautiful responsive designs. The cards in aether use flexbox to change the image from the right side on desktops to the top on mobile.

---

## Code

````md
```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
````

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```

``` scss
blockquote{
    margin-left: 5%;
    padding: 10px;
    box-sizing: border-box;
    border-left: $line;
}
```

### Inline code

```md
Here is `var s = "Hello World"` inline code
```

Here is `var s = "Hello World"` inline code

---

## Math


#### [Mathjax](https://www.mathjax.org/)

$$ \begin{matrix}
    1 & x & x^2 \\
    1 & y & y^2 \\
    1 & z & z^2 \\
    \end{matrix}
$$

$$\omega$$

$$
 f(x) = sin(o
\varphi
\sqrt{x^3+1, where\ne 2*a1}
$$


#### [LaTeX style math typsetting with KaTeX](https://katex.org/)

```md
{{</* raw */>}}
\[u(t) = K_p e(t) + K_i \int_{0}^{t} e(\tau) d\tau + K_d \frac{de(t)}{dt} \]
{{</* /raw */>}}
```

{{< raw >}}
\[u(t) = K_p e(t) + K_i \int_{0}^{t} e(\tau) d\tau + K_d \frac{de(t)}{dt} \]
{{< /raw >}}

