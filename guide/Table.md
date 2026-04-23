---
title: Table
description:
permalink:
lang: en-US
publish: true
draft:
enableToc: true
tags:
aliases:
cssclasses:
socialDescription:
socialImage:
created: 2025-11-07
modified: 2025-11-07
published: 2025-11-07
---
You can create tables by assembling a list of words and dividing them with hyphens `-` (for the first row), and then separating each column with a pipe `|`:

```md
First Header | Second Header
------------ | ------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column
```

First Header | Second Header
------------ | ------------
Content from cell 1 | Content from cell 2
Content in the first column | Content in the second column

---

```md
Tables can be justified with a colon | Another example with a long title
:----------------|-------------:
because of the `:` | these will be justified
```

| Tables can be justified with a colon | Another example with a long title |
| :----------------------------------- | --------------------------------: |
| because of the `:`                   |           these will be justified |

If you put links in tables, they will work, but if you use Piped Links, the pipe must be escaped with a `\` to prevent it being read as a table element.

```md
First Header | Second Header
------------ | ------------
[[Format your notes\|Formatting]]	|  [[Callouts\|Callouts]]
```

| First Header                                     | Second Header                        |
| ------------------------------------------------ | ------------------------------------ |
| [[VRT/Formatting/Format your notes\|Formatting]] | [[VRT/Formatting/Callout\|Callouts]] |

## Alignment
```md
| #  |   Item    | Value |
| :- | :-------: | -----:|
| 1  | Computer  | $1600 |
| 2  |  Phone    |   $12 |
| 3  |   Pipe    |    $1 |
```

| #   |   Item   | Value |
| :-- | :------: | ----: |
| 1   | Computer | $1600 |
| 2   |  Phone   |   $12 |
| 3   |   Pipe   |    $1 |

## Compact
```md
#|Item|Value
:-|:-:|-:
1|Computer|$1600
2|Phone|$12
3|Pipe|$1
```

#|Item|Value
:-|:-:|-:
1|Computer|$1600
2|Phone|$12
3|Pipe|$1
## Tables no pipes
```md
Header 1 | Header 2
-------- | --------
  Cell 1 | Cell 2
  Cell 3 | Cell 4
```

| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1   | Cell 2   |
| Cell 3   | Cell 4   |

```md
First Header  | Second Header
------------- | -------------
Content 1     | Content 2
Content 3     | Content 4
```

First Header  | Second Header
------------- | -------------
Content 1     | Content 2
Content 3     | Content 4
## Tables with leading pipe
```md
| Header 1 | Header 2
| -------- | --------
| Cell 1 | Cell 2
| Cell 3 | Cell 4
```

| Header 1 | Header 2
| -------- | --------
| Cell 1 | Cell 2
| Cell 3 | Cell 4

## Tables with full bars
```md
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |
```

| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |

```md
| First Header  | Second Header |
| ------------- | ------------- |
| Content 1     | Content 2     |
| Content 3     | Content 4     |
```

| First Header | Second Header |
| ------------ | ------------- |
| Content 1    | Content 2     |
| Content 3    | Content 4     |

## Tables with missing pipes
```md
# Missing tailing pipe

Header 1  | Header 2  
--------- | --------- |
Cell      | Cell      |
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- 
Cell      | Cell      |
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- |
Cell      | Cell      
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- |
Cell      | Cell      |
Cell      | Cell      
```

## Tables with missing tailing pipe

Header 1  | Header 2  
--------- | --------- |
Cell      | Cell      |
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- 
Cell      | Cell      |
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- |
Cell      | Cell      
Cell      | Cell      |

Header 1  | Header 2  |
--------- | --------- |
Cell      | Cell      |
Cell      | Cell      

## Tables with too many pipes n rows
```md
# Too many pipes in rows

| Header 1  | Header 2  |
| --------- 
| Cell      | Cell      | Extra cell? |
| Cell      | Cell      | Extra cell? |
```

## Too many pipes in rows

| Header 1  | Header 2  |
| --------- 
| Cell      | Cell      | Extra cell? |
| Cell      | Cell      | Extra cell? |

## Tables with mixed bars
```md
Header 1 | Header 2
| -------- | --------
Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |
```

Header 1 | Header 2
| -------- | --------
Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |

## Tables with bars and leading spacing
```md
| Header 1 | Header 2 |
 | -------- | -------- |
 | Cell 1 | Cell 2 |
 | Cell 3 | Cell 4 |
```

 | Header 1 | Header 2 |
 | -------- | -------- |
 | Cell 1 | Cell 2 |
 | Cell 3 | Cell 4 |

## Table with cuddled following content
```md
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |
after
```

| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |
after

## Table with cuddled leading content
```md
before
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |
```

before
| Header 1 | Header 2 |
| -------- | -------- |
| Cell 1 | Cell 2 |
| Cell 3 | Cell 4 |

## Single column single leading bar
```md
| Header 1
| --------
| Cell 1
| Cell 3
```

| Header 1
| --------
| Cell 1
| Cell 3

## Single column single trailing bar
```md
Header 1 |
-------- |
Cell 1 |
Cell 3 |
```

Header 1 |
-------- |
Cell 1 |
Cell 3 |

## Single column full bars
```md
| Header 1 |
| -------- |
| Cell 1 |
| Cell 3 |
```

| Header 1 |
| -------- |
| Cell 1 |
| Cell 3 |

## Narrow col 1
```md
| H |
| - |
| 1 |
| 2 |
```

| H   |
| --- |
| 1   |
| 2   |

## Narrow col 2
```md
| He |
| -- |
| 1 |
| 2 |
```

| He |
| -- |
| 1 |
| 2 |

## Narrow col 3
```md
| He |
| --- |
| 1 |
| 2 |
```

| He |
| --- |
| 1 |
| 2 |

## No dash
```md
| He |
| :: |
| 1 |
| 2 |
```

| He |
| :: |
| 1 |
| 2 |

## Table with markup in cells
```md
| Header 1 | *Header* 2 |
| -------- | -------- |
| `Cell 1` | [Cell 2](http://example.com) link |
| Cell 3 | **Cell 4** |
```

| Header 1 | *Header* 2 |
| -------- | -------- |
| `Cell 1` | [Cell 2](http://example.com) link |
| Cell 3 | **Cell 4** |

```md
| Function name | Description                    |
| ------------- | ------------------------------ |
| `help()`      | Display the help window.       |
| `destroy()`   | **Destroy your computer!**     |
```

| Function name | Description                    |
| ------------- | ------------------------------ |
| `help()`      | Display the help window.       |
| `destroy()`   | **Destroy your computer!**     |
## Table in blockquote
```md
> | One | Two | Three |
> | --- | --- | --- |
> |grinch|stole|xmas|
> |green|**eggs**|ham|
>
> -- Dr. Seuss
```

> | One | Two | Three |
> | --- | --- | --- |
> |grinch|stole|xmas|
> |green|**eggs**|ham|
>
> -- Dr. Seuss

## Table with blank cells
```md
| Header 1 |  |
 | -------- | -------- |
 | Cell 1 |          |
 |  | Cell 4 |
```

 | Header 1 |  |
 | -------- | -------- |
 | Cell 1 |          |
 |  | Cell 4 |


```md
| Header 1  | Header 2  |
| --------- | --------- |
| A         | B         |
| C         |           |
```

| Header 1 | Header 2 |
| -------- | -------- |
| A        | B        |
| C        |          |

```md
Header 1  | Header 2
--------- | ---------
A         | B
          | D
```

Header 1  | Header 2
--------- | ---------
A         | B
          | D

## Table in blockquote with empty cells
```md
> |  | Two | Three |
> | --- | --- | --- |
> |grinch|stole||
> |green|**eggs**|ham|
>
> -- Dr. Seuss
```
> |  | Two | Three |
> | --- | --- | --- |
> |grinch|stole||
> |green|**eggs**|ham|
>
> -- Dr. Seuss

## Escaping of pipes
```md
| A  | \| | C \| C |
|--- |--- | ------ |
|\|\|| BB | C |
```

| A    | \|  | C \| C |
| ---- | --- | ------ |
| \|\| | BB  | C      |

```md
| a\|b | c    |
| -----|------|
| 1    | 2\|3 |
| 4\|5 | 6    |
```

| a\|b | c    |
| -----|------|
| 1    | 2\|3 |
| 4\|5 | 6    |

## Table without rows
```md
| abc | def |
| --- | --- |
```

| abc | def |
| --- | --- |

## Trailing table whitespace
```md
| Pros                                   | Cons                                          |  
|-----------------------------------------|------------------------------------------------|  
| Unique and refreshing take on the genre | May not resonate with all viewers              |  
| Cult classic status                      | Over-the-top humor may polarize audiences      |  
| Influential in launching careers         | Niche appeal among comedy aficionados          |
```

| Pros                                   | Cons                                          |  
|-----------------------------------------|------------------------------------------------|  
| Unique and refreshing take on the genre | May not resonate with all viewers              |  
| Cult classic status                      | Over-the-top humor may polarize audiences      |  
| Influential in launching careers         | Niche appeal among comedy aficionados          |
## Whitespace tolerance
```md
This is a table (look out, less than 4 spaces
before headers and rule).

   Header  |  Header
  -------- | --------
     1     |    2
     3     |    4

Yeah, right.
```

This is a table (look out, less than 4 spaces
before headers and rule).

   Header  |  Header
  -------- | --------
     1     |    2
     3     |    4

Yeah, right.