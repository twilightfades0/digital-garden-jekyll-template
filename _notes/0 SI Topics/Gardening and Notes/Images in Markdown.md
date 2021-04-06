
# How to do stuff with images in markdown!: 

```ad-tip 
title: To add a CSS snippet
collapse: open
content:

1. Paste the snippet into your text editor
2. Save as whateveryouwant.css in 
`...[vault folder]\.obsidian\snippets`
3. In Obsidian, go to Settings -> Appearance -> CSS snippets
4. Toggle it on!

```



## Align
Thanks for the following goes to **foreveryone** in the [Obsidian Members Group](https://discord.gg/) on [[Discord]]!


1. Get the snippet here: [Image Grids and Floats (github.com)](https://github.com/gitobsidiantutorial/assorted-css-snippets#image-grids-and-floats)
2. Add it to Obsidian (see the tip box at the top of the page)
3. Format your image according to the examples below:

<br>




##### Image align, with L/R text wrap:
```
![[example.png|left|300]]

![[example.png|centre|300]]

![[example.png|right|300]]
```


![[3706211.png|left|75]] ![[3706211.png|right|75]] Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus ut consequat nisi. Nullam et eleifend elit. Suspendisse in turpis tincidunt, aliquet risus et, vehicula velit. Proin sit amet neque vel est convallis dictum sit amet et urna. 

![[3706211.png|centre|75]] 

```
![[example.png|centre|75]] ![[example.png|left|75]] ![[example.png|right|75]] Lorem ipsum dolor sit amet.....
```

<br>

For Float:

```
![float-right](3706211.png)
```

<br>

##### Images next to each other:

```
![[example.png|grid|75]]
```

![[3706211.png|grid|75]] ![[3706211.png|grid|75]] ![[3706211.png|grid|75]] Lorem ipsum dolor sit amet, consectetur adipiscing elit.

```
![[example.png|grid|75]] ![[example.png|grid|75]] ![[example.png|grid|75]] Lorem ipsum dolor sit amet...
```


## Image Captions
Thanks for the following goes to **foreveryone** in the [Obsidian Members Group](https://discord.gg/) on [[Discord]]!

1. Get the snippet at the bottom of this section.
2. Add it to Obsidian (see the tip box at the top of the page)
3. Format your image according to the examples below:

<br>

![[3706211.png|left|75]]<figcaption id="left" style="width:75px">This is a caption</figcaption>  Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin quis velit efficitur, vestibulum dui ut, maximus purus. Maecenas ut vestibulum elit. Integer quis sapien est. Pellentesque viverra sem vel felis vehicula laoreet. Fusce mi est, ornare in facilisis ullamcorper, pretium sed ex. Duis viverra ante quis ante rhoncus tincidunt. Vestibulum ut volutpat massa.

```
![[example.png|left|75]]<figcaption id="left" style="width:75px">This is a caption</figcaption>  Lorem ipsum dolor sit amet...
```

<br>
<br>


#### For two images with captions on either side of the page

In this case you'll need to put the images first, then the captions. Like this:


![[3706211.png|left|75]] ![[3706211.png|right|75]] <figcaption id="left" style="width:75px">This is a caption</figcaption> <figcaption id="right" style="width:75px">This is a caption</figcaption> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin quis velit efficitur, vestibulum dui ut, maximus purus. Maecenas ut vestibulum elit. Integer quis sapien est. Pellentesque viverra sem vel felis vehicula laoreet. Fusce mi est, ornare in facilisis ullamcorper, pretium sed ex. Duis viverra ante quis ante rhoncus tincidunt. Vestibulum ut volutpat massa.

```
![[example.png|left|75]] ![[example.png|right|75]] <figcaption id="left" style="width:75px">This is a caption</figcaption> <figcaption id="right" style="width:75px">This is a caption</figcaption> Lorem ipsum dolor sit amet....
```

<br>

#### CSS Snippet

```
figcaption { /* if you want to style captions, set rules here, like color: and fontsize:*/
display: flex;
justify-content: center;
}

figcaption#left {
clear: left;
float: left;
}

figcaption#right {
clear: right;
float: right;
}

figcaption#centre,
figcaption#center {
margin-left: auto;
margin-right: auto;
}
```

## Images as Links


[![[3706211.png|75]]](http://t5witter.com/ameyawarde)

```
[![[example.png|75]]](http://link.com)
```

<br>

**With an image URL:**

[![@ameyawarde|40](https://github.com/twilightfades0/digital-garden-jekyll-template/blob/master/_notes/_theme/GradientTwitterBird40px.png?raw=true)](http://twitter.com/ameyawarde)

```
[![Alt Text|40](www.example.com/image.png)](http://linkyloo.com)
```

<br>

#### To link internally:


[![[3706211.png|75]]]([[Kanban]])

```
[![[3706211.png|75]]]([[Internal_Link]])
```

If the internal link has spaces or special characters, you'll need to run it through: [URL Encode Decode (url-encode-decode.com)](https://www.url-encode-decode.com/)

