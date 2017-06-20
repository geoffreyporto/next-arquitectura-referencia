# Introduction


{% method -%}
## Install {#install}

The first thing is to get the GitBook API client.

{% sample lang="js" -%}
```bash
$ npm install gitbook-api
```

{% sample lang="go" -%}
```bash
$ go get github.com/GitbookIO/go-gitbook-api
```
{% endmethod %}


# Documentos de GoolgeDocs

https://docs.google.com/spreadsheets/d/1H9IV4KlGJ5oTsNrg4jO67LfutoVSarflanzPvM_6tmU/edit?usp=sharing

Liga: [Non-embedded spreadsheet](https://docs.google.com/spreadsheets/d/1H9IV4KlGJ5oTsNrg4jO67LfutoVSarflanzPvM_6tmU/edit?usp=sharing "Open in new window")


# Codigo embebido de Github
https://github.com/v5analytics/gitbook-plugin-github-embed/blob/1cd16ac/index.js#L3-L8


# Codigo completo
{% github_embed "https://github.com/geoffreyporto/message-queue-system/blob/master/nodejs/test.js" %}{% endgithub_embed %}

# Lineas de codigo 5-10
{% github_embed "https://github.com/geoffreyporto/message-queue-system/blob/master/nodejs/test.js#L5-L10" %}{% endgithub_embed %}

# Excepto las lineas de codigo 2,4, 7-10

{% github_embed "https://github.com/geoffreyporto/message-queue-system/blob/master/nodejs/test.js" ,
hideLines=[2, '4', '7-10'], reindent=true, showLink=true %}{% endgithub_embed %}




# Plugin  https://github.com/visallo/gitbook-plugin-github-embed

#Take a look at this video:

# Math1

Inline math: $$\int_{-\infty}^\infty g(x) dx$$


# Block math:

$$
\int_{-\infty}^\infty g(x) dx
$$



When {% math %}a \ne 0{% endmath %}, there are two solutions to {% math %}(ax^2 + bx + c = 0){% endmath %} and they are {% math %}x = {-b \pm \sqrt{b^2-4ac} \over 2a}.{% endmath %}

{%youtube%}dQw4w9WgXcQ{%endyoutube%}


{%youtube src="https://www.youtube.com/watch?v=9bZkp7q19f0" %} {%endyoutube%}


# Ejercicio

{% exercise %}
Define a variable `x` equal to 10.

{% initial %}
var x =

{% solution %}
var x = 10;

{% validation %}
assert(x == 10);

{% context %}
// This is context code available everywhere
// The user will be able to evaluate `exposedVar`
var exposedVar = 3;
// ... or call `exposedFunction`
function exposedFunction {
    return 3;
}
{% endexercise %}



# VBNET

``` java
Dim x = 5
x = x ^ 2 + 1
Console.WriteLine("x = {0}", x)
``` (remove the brackets here with the text inside)


# terminal

**[terminal]
**[prompt foo@joe]**[path ~]**[delimiter  $ ]**[command ./myscript]
Normal output line. Nothing special here...
But...
You can add some colors. What about a warning message?
**[warning [WARNING] The color depends on the theme. Could look normal too]
What about an error message?
**[error [ERROR] This is not the error you are looking for]


# Diagramas

{% swimlanes %}

Title: Welcome to swimlanes.io


One -> Two: Message

Note:
**swimlanes.io** is a simple online tool for creating _sequence diagrams_.

Edit the text to the left to update the diagram.

**Copy the url** to save or share the diagram, _note that the url change whenever you update the diagram_


Two -> Two: To self

Two -->> Three: _Notification_

Two -> One: `ok`

Note: See **[full syntax overview](/gallery/full-syntax)** for more details

{% endswimlanes %}

{% swimlanes %}

Title: Swimlanes.io full syntax overview


_: **1. Messages**
One -> Two: Simple
Two ->> Three: Open arrow (async)
Three <-> Four: Bi-directional
Two -> Two: To self

Two -> One: Actors can be
One <- Two: in any order

Two -> Three: Regular
Two <-- Three: Dashed (response)
Two <=> Three: Bold

One -> Four: Markdown support for messages: *Italic*, **Bold**, ~~strike through~~ and `inline code`


_: **2. Notes**

Note:
Simple text formatting; **bold**, *italic*, ~~strike through~~ and `inline code`

1. Ordered
2. list


* Unordered
* list

[link](http://www.swimlanes.io)


Two -> Three: A note is closed by a following element

Note: A note spans the length of the previoues message by default

Note One, Three: Specify the start end end actor to change the width of a note

_: **3. Sections**

if: Define conditional flows with _**if**_
  Two -> Three: Message
else: Optional alternative flow with _**else**_   
  Two -> One: Message
else
  One <-> Four: Section lables are optinal
  if: Sections can be nested one level
  end
// Sections are closed by an "end" statement
end

group: _**group**_ can be used instead of _**if**_ for simple grouping

end


_: **4. Lines**
_: thin
-: regular
--: dashed
=: bold
-: Markdown support for lines: *Italic*, **Bold**, ~~strike through~~ and `inline code`


_: **5: Order**
Note: Change the order of the actors with the _**order**_ statement

// Uncomment next line for re-ordering
// Order: Three, Two

{% endswimlanes %}
