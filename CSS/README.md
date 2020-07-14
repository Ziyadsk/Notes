# CSS 
*cascading style sheets*

## Selection
`*` : global selector that select every html tag on the page
`,` : use comma to select multiple elements
### Type selector
Select the type of a specifig tag  

<ins>Example:</ins>  
this style will be applied on every `p` tag on the page  
```css 
p {
	color : red ; 
}
```

### Classes and Ids
### Ids
`#title`
### Classes

`.links`  
`button.links`
`button.links.primary`

#### Select children 

#### Direct child
`>`
#### Siblings
`~` every sibling
`+` 1 next 
### Pseudo selectors
`hover`
`focus`
### Nth-Child
`first-child`
`nth-child()`
`only-child`
### Not()

### Pseudo elements
#### Before
#### After


##  CSS Propreties

## Attributes selectors

```CSS
[Attr] {
	color:blue ; 
}```

```CSS
[Attr^="java"] {
	color:blue ; 
}
```

## Colors
	* literal 
	* hex
	* rgb
	* hsl
## Background
	* color
	* image
	* size
	* background-blend-mode
	* mix-blend-mode

##  Padding & margins
### Width
###  Max-width & min-width
* %
* ch
### Padding
#### short form

#### semi-short

### Margin

## Display & Position
### Absolute
### relative
### fixes
### sticky

## Fonts
	* Size
	* Family
	* style
	* weight
	* Importing new fonts

## Borders & outline

## Shadows
	 * Box-shadow
	 * text-shadow

## Filters
* filter()
* backdrop-filter 


## Flex & Grid
* Flexbox
	* wrap 
	* direction
	* justify-content

* Grid
	* grid-template
	* place-items 
	* gap 

## Animations
### Transition
### Transform
* translate 
* rotate
* skew 
## other 
### opacity
### cursor

## Methodologies 
* atomicCSS : (FUNCTIONNAL css)
immutabily and separation

* OOCSS

* SMACSS

* BEM 
`element__child_elem`
