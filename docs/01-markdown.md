# **Markdown**

## **Summary**

[1 - What is markdown ](#1-what-is-markdown)

[2 - About Markdown syntax](#2-markdown-syntax)

[3- Header syntax](#3-header-syntax)

[4 - Emphasis syntax](#4-emphasis-syntax)

[5 - Images and gif syntax](#5-images-and-gifs-syntax)

[6 - Links syntax ](#6-links-syntax)

[7 - Line break syntax](#7-line-break-syntax)

[8 - Lists syntax](#8-lists-syntax)

[9 - Table syntax](#9-table-syntax)

[10 - Details syntax](#10-details-syntax)

[11 - Code syntax](#11-code-syntax)

[12 - Emojis syntax](#12-emoji)

## 1. **What is Markdown?**

Markdown is a simple mark language, used to write articles, notes, documents and much more using an simple syntax to the text to indicate which format that text will have.
Markdown converts all your markdown formatted text to HTML, also markdown accept HTML elements.

📝 Through my learning journey i will be using markdown to write and document everything that i am learning. 

![markdown convert example](https://gist.githubusercontent.com/felipeln/3688019c2ecd61930d83b416dbb063ec/raw/3ac215c2e3617194f5d5b5d4c9eef5cce2b4c701/markdown-flowchart.png)

&nbsp;

## 2. **Markdown syntax**

The markdown syntax have elements like, headers, markers, tables, images and much more. 

&nbsp;

### 3. **Header syntax**

# Header 1

## Header 2

## Header 2

### Header 3

#### Header 4

##### Header 5

###### Header 6  

&nbsp;

```md
# Header 1
## Header 2
## Header 2
### Header 3
#### Header 4
##### Header 5
###### Header 6
or
<h1> Header 1</h1>
<h2> Header 2</h2>
<h3> Header 3</h3>
<h4> Header 4</h4>
<h5> Header 5</h5>
<h6> Header 6</h6>
```

### 4. **Emphasis syntax**

&nbsp;

**bold text**  

```md
**bold text**
or
<strong>bold text</strong>
```

&nbsp;

*italic text*

```md
*italic text*
or
<i>italic text</i>
```

&nbsp;

***italic and bold***

```md
***italic and bold***
or
<i><strong>italic and bold</strong></i>
```

&nbsp;

~~strike text~~

```md
~~strike text~~
or
<s>strike text</s>
```

&nbsp;

>block quote

```md
>block quote
or
<blockquote>blockquote</blockquote>
```

&nbsp;

>multiples block quote
>> line 2
>>> line 3

```md
>multiples block quote
>> line 2
>>> line 3
or
<blockquote>blockquote
    <blockquote>line 2
        <blockquote> line 3</blockquote>
    </blockquote>
</blockquote>

```

&nbsp;

### 5. **images and gifs syntax**

&nbsp;

**Image** 

![text describing the image](https://i.imgur.com/0lhSv5g.jpeg "cat family")

```md
![text describing the image](https://i.imgur.com/0lhSv5g.jpeg)
or
<img src="https://i.imgur.com/0lhSv5g.jpeg" alt="text describing the image">
```

&nbsp;

**Gifs** 

![text describing the gif](https://media.giphy.com/media/Cmr1OMJ2FN0B2/giphy.gif "text to show when hover the image")

```md
![text describing the gif](https://media.giphy.com/media/Cmr1OMJ2FN0B2/giphy.gif)
or
<img src="https://media.giphy.com/media/Cmr1OMJ2FN0B2/giphy.gif" alt="text describing the gif">
```

&nbsp;

### 6. **Links syntax**

[this is a link for a website](https://github.com/felipeln)

```md
[this is a link for a website](https://github.com/felipeln)
or
<a href="https://github.com/felipeln">this is a link for a website</a>
```

&nbsp;

[this is a link for a file](/README.md)

```md
[this is a link for a file](/README.md)
or
<a href="/README.md">this is a link for a file</a>
```

&nbsp;

[this is a link with title](https://github.com/felipeln "my github profile")

```md
[this is a link with title](https://github.com/felipeln "my github profile")
or
<a href="https://github.com/felipeln" title="my github profile">this is a link with title </a>
```

&nbsp;

[link to my profile as reference][1]

<!-- something -->

[1]: https://github.com/felipeln

```md
[link to my profile as reference][1]
<-- here you can have some content in markdown -->
[1]: https://github.com/felipeln

```

&nbsp;

word for link reference [link]

[link]: https://github.com/felipeln

```md
word for link reference [link]
[link]: https://github.com/felipeln
```

### 7. **Line break syntax**

to break a line in markdown you need to add two white spaces at the end of the line.

this line will break  
just a line

```md
this line will break  
just a line
or
this line will break <br>
just a line
```

&nbsp;

### 8. **Lists syntax**  

**ordered list**

1. first item
2. second item
3. third item
    1. first indented item
    2. second indented item

```md
1. first item
2. second item
3. third item
    1. first indented item
    2. second indented item

or

<ol>
    <li>First item</li>
    <li>Second item</li>
    <li>third item</li>
        <ol>
            <li>first indented item</li>
            <li>second indented item</li>
        </ol>
</ol>
```

&nbsp;

**Disordered list**

- First item
- Second item
- third item
    - first indented item
    - second indented item

```md
- First item
- Second item
- third item
    - first indented item
    - second indented item

or

<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <ul>
        <li>First indented item</li>
        <li>Second indented item</li>
    </ul>
</ul>
```

&nbsp;

**Task list**

- [ ] first task
- [x] second task
- [x] third task

```md
- [ ] first task
- [x] second task
- [x] third task
```

&nbsp;

### 9. **Table syntax**
table 1

|Column| Column | Column|
|:---- | :----: | ----: |
|Left  |Center  |Right  |

&nbsp;

table 2
|Column| Column| Column|
|----: | :---- | :----:|
|Right | Left  | Center|
| 1    | 2     | 3     |

```md
table 1
|Column| Column | Column|
|:---- | :----: | ----: |
|Left  |Center  |Right  |

table 2
|Column| Column| Column|
|----: | :---- | :----:|
|Right | Left  | Center|
| 1    | 2     | 3     |

or

table 1
<table>
    <tr>
        <th>Column</th>
        <th>Column</th>
        <th>Column</th>
    </tr>
    <tr>
        <td align="left">Left</td>
        <td align="center">Center</td>
        <td align="right">Right</td>
    </tr>
</table>

table 2
<table>
    <tr>
        <th>Column</th>
        <th>Column</th>
        <th>Column</th>
    </tr>
    <tr>
        <td align="right">Right</td>
        <td align="left">Left</td>
        <td align="center">Center</td>
    </tr>
    <tr>
        <td align="right">1</td>
        <td align="left">2</td>
        <td align="center">3</td>
    </tr>
</table>
```

&nbsp;
### 10. **Details syntax**

<details>
    <summary>Summary list</summary>
    
* first item
* second item
* third item
</details>

```md

<details>
    <summary>Summary list</summary>
    
* first item
* second item
* third item
</details>

```

&nbsp;

### 11. **Code syntax**

output:
```C
 #include <stdio.h>
    
    int main(void){
        printf("Hello, World!");
        return 0;
    }
```

code:
```C
    ```C
    #include <stdio.h>
        
        int main(void){
            printf("Hello, World!");
            return 0;
        }
    ```

    or

    <code>
        #include <stdio.h><br>
        <br>
        int main(void){<br>
            printf("Hello, World!");<br>
            return 0;<br>
        }<br>
    </code>
```

&nbsp;

### 12. **Emoji**

You can add emojis and icons on your markdown, just copy and paste, you can find emojis on [Emojipedia](https://emojipedia.org/ "Emojipedia"), [Emoji-list](https://github.com/caiyongji/emoji-list "emoji-list")  and on other sites

smile :grinning:  
star  :star:  
heart  ❤️  
hamburger  🍔  

```md
smile :grinning: 
star  :star:
heart  ❤️
hamburger  🍔
```
