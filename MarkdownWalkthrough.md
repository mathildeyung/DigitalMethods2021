# Table of Contents 

* [Text Formatting](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#text-formatting)

* [Lists](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#lists)
  * [Unordered List](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#unordered-list)
  * [Ordered List](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#ordered-list)

* [Various Objects](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#various-objects)
  * [Links](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#links)
  * [Images](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#images)
  * [Blockqoutes](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#blockqoutes)
  * [Tables](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#tables)

* [Formatting - making it pretty](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#formatting---making-it-pretty)
  * [Alignment](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#alignment)
  * [Syntax Highlighting](https://github.com/mathildeyung/DigitalMethods2021/blob/main/MarkdownWalkthrough.md#syntax-highlighting)


# Writing in Markdown (this is header 1)
## A walkthrough (This is header 2)
### We'll see how it goes... (This is header 3)
###### You can make headers in 6 different sizes. It corresponds to the number of '#'. This is the smallest. 

## Text formatting
Okay, so first of all we want to try to make things either italic, bold, or crossed out. 
If we want to make something *italic* we use 1 asterisk. If we want to make something **bold** we use 2 asterisks. If we want to make something ~~crossed out~~ we use two tilts (~). You can also do it like this _italics_ __bold__ AND you can also combine them __*combined*__.
Alright, so far so good. But how come we don't have proper spacing? We don't seem to get anywhere when hitting 'enter'. Well, thats because you need to press it two times...

Like this. 

## Lists

Right. Next we'd like to make a list - we can make them both unordered and ordered.

### Unordered list 
* Item 1 
* Item 2 
  * Item 1 - *To make an sub-list you simply put 2 'spaces' before the asterisk.*
  * Item 2

You can also do like this 
- Item 1
- Item 2
- Item 3

### Ordered list
1. Item 1
1. Item 2
1. Item 3
   1. Item 3a - *To make sub-list you put 3 'spaces' before the '1.'*
   1. Item 3b
1. Item 4
   1. Item 4a

## Various Objects

### Links
Now we want to insert a link. This is how:

[GitHub MarkDown documentation](https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax)
*Good to know. Any url like (https://github.com/) will automatically be converted to a clickable link.*

### Images
What about images? To insert an image you do like this.:

We'll use a random one.

![Name of Image](https://picsum.photos/200/200) 

Naturally, it is also possible to use images from other sites or saved on your computer. Simply paste the url or attach the image (or other files) at the bottom of the page. This will paste the image where you've put the cursor.

### Blockqoutes
Next up is blockqoutes. This is easy.

> You just do like this.
>> That *is* pretty easy. 
>>> Yes. That's what I said.

### Tables
You can also do tables. Let's do that. 

First header | Second header | Third header
------ | ------ | ------ |
First thing | Second thing | Third thing
Again | Again again | Again again again

## Formatting - making it pretty

### Alignment
What if you want to align text to the centre or to the right? You'll need to use <div> tags around the text. 

<div align="center">
This is the text I want to centre
 
But now everything's centred. 
 
So we need to go back by aligning to the left again.

<div align="left">


### Syntax Highlighting
Okay lastly, we can do syntax highlighting.

```Python
user_words = []

for i in e2020_df.index:
    word_dict = {}
    text = e2020_df.text[i].lower().split(' ')
    for word in text:
        if word not in word_dict:
            word_dict[word] = e2020_df.text[i].count(word)
    user_words.append(word_dict)
```

You can also do another language. Lets say javascript for example. If it was another language you would just write that name after the 3 '`'
```javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

Perfect. This is it ???? (probably not relevant, but GitHub MarkDown also support emojis. Here you go: https://github.com/ikatyang/emoji-cheat-sheet/blob/master/README.md)

