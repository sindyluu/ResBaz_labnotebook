# Digital Lab Notebook (DLN) test repository
Trial of digital lab notebook at ResBazDunedin2018

## Header style 2 example
### Header style 3 example

Header style 1 example
===
Header style 2 example
---


# MarkDown Syntax
We're talking about **bolds**, *italics*, and ~strikethrough~

Another way for __bolds__, _italics_

Having these two different syntax for bolds and italics can allow us to combine the **_two together_**

There is no underline

-----------------

## Bullet points, numbered lists and checked lists
* bullet point 1 (exactly like shortcut in word: astericks with space)
- bullet point 2 (exactly like shortcut in word: dash with space)

1. numbered list 1 (exactly like shortcut in word: 1 with space)
1. Note, it can all be '1' and it will automatically list in order. 
1. This way we can move lists around and not worry about re-numbering

## Checked lists
To-do's and Done's
- [ ] item 1
- [ ] item 2
- [x] item 3 (done)

## Nesting lists
* Item 1
  * Item 1a
  * Item 1b
 * Item 2
  * Item 2a
  
-------------

# Making tables

Let's make a clean table with markdown

| Name  | Age | Department  | Job |
|---  | --- | :---: | ---: |
| Sindy | 31  | Anatomy | PhD candidate |
| Boro  | 2 | Otago | Mystery |

Notes:
* The title is automatically bold
* The title is indicated by the second line, with minimum of three dashes
* The number of '|' must match number of columns you are creating
* To centre align the column, you mark it with ':---:' in the title
* Similarly, to align the column to the right, you mark it with '---:' in the title


--------------

# Markdown texts, paragraphs, and quotes
By default, markdown collapses any white spaces between words.

This sentence contains only a single whitespace between words
    This      sentence     contains      a lot of       white spaces in between the words


A single white line in between sentences will create

another paragraph.
Otherwise it will combine and continue from the preceeding text.

> This is how you insert quotes


-------
## Links and hyperlinks

The syntax is relatively simple
[]()

This is a link to [Google](https://www.google.com)


---------

## Codes and syntax highlighting
This is useful if you work with a lot of codes and want to keep track of them

You can insert codes inline with a pair of `backticks`

Or you can insert loop codes with a series of three backticks at the beginning and end of the coding block

```
module load AdapterRemoval
cd $output

for samp in $samplist
do
AdapterRemoval \
--file1 ${datadir}$samp$fq1 \
--file2 ${datadir}$samp$fq2  \
--collapse  \
--trimns  \
--trimqualities  \
--minlength 25  \
--mm 3  \
--minquality 20  \
--basename $samp

gzip $datadir${samp}${fq1}
gzip $datadir${samp}${fq2}

done
```

------
## Inserting images

Upload files using the tool/button/function

![map](New_Ireland_Topography.png)
