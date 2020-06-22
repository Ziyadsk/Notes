# Markdown
* Markdown is a lightweight markup language with plain-text-formatting syntax, often used to create README.md files like this one.
## Content

* [Heading](#heading)  
* [Bold & italic text](#bold-and-italic-text)  
* [Links](#links)  
* [Images](#images)  
* [Code blocks](#code) 
* [Tables](#tables)

## Heading
* to create a heading in markdown, write any text preceded by a (1 to 6) pound symbols (#), these represent [HTML](../HTML/README.md) **`<h1>`** to **`<h6>`**  
<ins>Examples:</ins>
```markdown
    # very big title
    ### subtitle
    ##### small title
```
> output:
>    # very big title
>  ### subtitle
>   ##### small title
## Bold and italic text
### italics
```
*italic text*
```
> output:
*italic text*
### bold
```
**bold text**
```
> output: 
> **bold text** 
### strikethrough
```md
~~striked~~
```
## Links
* to create a link in markdown , put the link text inside square `[]` brackets and then followed by parentheses `()` that contains the link  
<ins>Examples</ins>
```
[google link](www.google.com)
```
> output : [google link](www.google.com) 

## Images
* Creating images is similar to links, but with an exclamation mark `!` before.  
<ins>Examples</ins>
```
![](https://via.placeholder.com/150)
```
> output:  
![](https://via.placeholder.com/150)
## Lists

### Ordered list
```
1. One
2. Two
3. four
```
>output :
1. One
2. Two
4. four

### Unordered list  
```
* Apples  
* Oranges
```
>output :
* Apples  
* Oranges
### Nested items
```
* Parents
    * Child
    * Another child
```
>output :
* Parents
    * Child
    * Another child
 # Code
* To display a block on code use backticks ``  
<ins>Examples</ins>
#### Inline
**`echo "test" `**

### Blocks
```js 
function myFunc(name){
    console.log(`Hello ${name}`)
}
```

## Blockquotes
> some quote
## Tables
```
| product | price |
|--------|--------|
| tv     | 2000   |
| cat    | 90     |
```
> output  
 
| product | price |
|--------|--------|
| tv     | 2000   |
| cat    | 90     |


## line separator
**`---`**  to create a horizontal line
> output  
---