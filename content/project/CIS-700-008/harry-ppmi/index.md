---
title: Share my new passion for a vibrant new ecosystem Harry Potter Fan Fiction
summary: A small snippet of my paper, some initial analysis between Harry Potter Fanfiction and the original canons.
tags:
- CIS 700-008
date: "2016-05-04T00:00:00Z"

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: "\"You did it.  You crazy son of bitch, you did it!!!\""
  focal_point: Smart

links:
- icon: twitter
  icon_pack: fab
  name: Follow
  url: https://twitter.com/tensorglow
url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: example

---

to 
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
  <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
  <meta http-equiv="Content-Style-Type" content="text/css" />
  <meta name="generator" content="pandoc" />
  <title>Untitled</title>
  <style type="text/css">
    code{white-space: pre-wrap;}
    span.smallcaps{font-variant: small-caps;}
    span.underline{text-decoration: underline;}
    div.column{display: inline-block; vertical-align: top; width: 50%;}
    div.hanging-indent{margin-left: 1.5em; text-indent: -1.5em;}
    ul.task-list{list-style: none;}
  </style>
</head>
<body>
<h1 id="preliminary-results">Preliminary Results</h1>
<p>The following is an example of an event chain extracted from a story from the fan fiction:</p>
<ol>
<li><p>(’CLUSTER 0’, ’nsubj’), (’walked’, ’root’)</p></li>
<li><p>(’CLUSTER 0’, ’nsubj’), (’looked’, ’root’)</p></li>
<li><p>(’CLUSTER 0’, ’nsubj’), (’changed’, ’root’)</p></li>
<li><p>(’CLUSTER 0’, ’nsubj’), (’asked’, ’root’)</p></li>
</ol>
<p>In the example above, the character in Harry Potter referred to as ’CLUSTER 0’ first walks, then looks, changes, and finally asks. The first element in every tuple is the word in the document with its replaced coreference-resolution tag and the second element is its first order dependency parse that was used to extract the event chain of every noun subject of a story.</p>
<h1 id="results">Results</h1>
<h2 id="pointwise-mutual-information-pmi-analysis">Pointwise Mutual Information (PMI) Analysis</h2>
<p>The most probable bigrams and the bigrams with the highest PMI were ran over all words, verbs, and events of the two corporas: Harry Potter Fanfiction and Harry Potter Canons. PMI analysis reveals the unique co-occuring concepts in each of the corporas and highlights other stylistic writing differences on average from the authors. Most probable bigrams are shown along side the highest PMI bigrams in each of the tables to show that the magnitude of the frequency count of each bigram over total bigrams does not entail importance or significance in a document and underscoring the value of PMI analysis.</p>
<div id="long">
<table>
<caption>PMI Analysis on Words.<span id="long" label="long">[long]</span></caption>
<tbody>
<tr class="odd">
<td align="center">Harry Potter Fanfiction</td>
<td align="center">Harry Potter Canon</td>
<td align="center">Harry Potter Fanfiction</td>
<td align="center">Harry Potter Canon</td>
</tr>
<tr class="even">
<td align="center">of the</td>
<td align="center">of the</td>
<td align="center">bibbidi bobbidi</td>
<td align="center">avada kedavra</td>
</tr>
<tr class="odd">
<td align="center">in the</td>
<td align="center">in the</td>
<td align="center">merus lumens</td>
<td align="center">felix felicis</td>
</tr>
<tr class="even">
<td align="center">to the</td>
<td align="center">said harry</td>
<td align="center">zauberei dorf</td>
<td align="center">bertha jorkins</td>
</tr>
<tr class="odd">
<td align="center">it was</td>
<td align="center">he was</td>
<td align="center">hoity toity</td>
<td align="center">whomping willow</td>
</tr>
<tr class="even">
<td align="center">on the</td>
<td align="center">at the</td>
<td align="center">palatino linotype</td>
<td align="center">expecto patronum</td>
</tr>
<tr class="odd">
<td align="center">at the</td>
<td align="center">to the</td>
<td align="center">magikos akademia</td>
<td align="center">dressing gown</td>
</tr>
<tr class="even">
<td align="center">he was</td>
<td align="center">on the</td>
<td align="center">alarte ascendare</td>
<td align="center">grubbly plank</td>
</tr>
<tr class="odd">
<td align="center">to be</td>
<td align="center">it was</td>
<td align="center">inkosi inkosikazi</td>
<td align="center">zacharias smith</td>
</tr>
<tr class="even">
<td align="center">she was</td>
<td align="center">he had</td>
<td align="center">namby pamby</td>
<td align="center">law enforcement</td>
</tr>
<tr class="odd">
<td align="center">i was</td>
<td align="center">out of</td>
<td align="center">modus operandi</td>
<td align="center">auntie muriel</td>
</tr>
<tr class="even">
<td align="center">and i</td>
<td align="center">said ron</td>
<td align="center">cuevas gontan</td>
<td align="center">bathilda bagshot</td>
</tr>
<tr class="odd">
<td align="center">out of</td>
<td align="center">into the</td>
<td align="center">füvessy uram</td>
<td align="center">goal posts</td>
</tr>
<tr class="even">
<td align="center">going to</td>
<td align="center">to be</td>
<td align="center">toothflossing stringmints</td>
<td align="center">pansy parkinson</td>
</tr>
<tr class="odd">
<td align="center">with a</td>
<td align="center">in a</td>
<td align="center">babbitty rabbitty</td>
<td align="center">deathly hallows</td>
</tr>
<tr class="even">
<td align="center">he had</td>
<td align="center">from the</td>
<td align="center">higgledy piggledy</td>
<td align="center">phineas nigellus</td>
</tr>
<tr class="odd">
<td align="center">as he</td>
<td align="center">said hermione</td>
<td align="center">dawh dawh</td>
<td align="center">king’s cross</td>
</tr>
<tr class="even">
<td align="center">in a</td>
<td align="center">had been</td>
<td align="center">shoop shoop</td>
<td align="center">diagon alley</td>
</tr>
<tr class="odd">
<td align="center">for the</td>
<td align="center">he said</td>
<td align="center">loundon’s towne</td>
<td align="center">pumpkin juice</td>
</tr>
<tr class="even">
<td align="center">was a</td>
<td align="center">was a</td>
<td align="center">farlin flookey</td>
<td align="center">st mungos</td>
</tr>
<tr class="odd">
<td align="center">as she</td>
<td align="center">of his</td>
<td align="center">helter skelter</td>
<td align="center">godrics hollow</td>
</tr>
<tr class="even">
<td align="center"></td>
<td align="center"></td>
<td align="center"></td>
<td align="center"></td>
</tr>
</tbody>
</table>
</div>
<p>Two random variable X, Y are independent iff their joint distribution is equal to the product of their margin</p>
</body>
</html>