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

<head>
    <script type="text/javascript"
            src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_SVG">
    </script>
</head>
\documentclass{article}
\usepackage{hyperref}
\usepackage[letterpaper]{geometry}
\usepackage{amsmath}
\usepackage{amssymb}
\usepackage{graphicx}
\usepackage{float}
\usepackage{array}
\usepackage{tikz}
\usepackage{enumerate}
\usepackage{booktabs}
\usepackage{tabularx}
\usepackage{xcolor,colortbl}
\usepackage{caption} 
\usepackage{authblk}
\usepackage{parskip}
\usepackage[shortlabels]{enumitem}
\usepackage{fancyvrb}

\documentclass{article}
\usepackage[utf8]{inputenc}
\usepackage{longtable}

\begin{document}
\section{Preliminary Results}
The following is an example of an event chain extracted from a story from the fan fiction:
\begin{enumerate}
    \item ('CLUSTER 0', 'nsubj'), ('walked', 'root')
    \item ('CLUSTER 0', 'nsubj'), ('looked', 'root')
    \item ('CLUSTER 0', 'nsubj'), ('changed', 'root') 
    \item ('CLUSTER 0', 'nsubj'), ('asked', 'root')
\end{enumerate}
In the example above, the character in Harry Potter referred to as 'CLUSTER 0' first walks, then looks, changes, and finally asks.  The first element in every tuple is the word in the document with its replaced coreference-resolution tag and the second element is its first order dependency parse that was used to extract the event chain of every noun subject of a story.   

\section{Results}
\subsection{Pointwise Mutual Information (PMI) Analysis}
The most probable bigrams and the bigrams with the highest PMI were ran over all words, verbs, and events of the two corporas: Harry Potter Fanfiction and Harry Potter Canons. PMI analysis reveals the unique co-occuring concepts in each of the corporas and highlights other stylistic writing differences on average from the authors.  Most probable bigrams are shown along side the highest PMI bigrams in each of the tables to show that the magnitude of the frequency count of each bigram over total bigrams does not entail importance or significance in a document and underscoring the value of PMI analysis.

 \begin{longtable}[c]{| c | c | c | c |}
 \caption{PMI Analysis on Words.\label{long}}\\
 \hline
 \multicolumn{2}{| c |}{Most Probable Bigrams} & \multicolumn{2}{| c |}{Highest PMI Bigrams}\\
 \hline
 Harry Potter Fanfiction & Harry Potter Canon & Harry Potter Fanfiction & Harry Potter Canon\\
 \hline
 of the & of the & bibbidi bobbidi & avada kedavra\\
 in the & in the & merus lumens & felix felicis\\
 to the & said harry & zauberei dorf & bertha jorkins\\
 it was & he was & hoity toity & whomping willow\\
 on the & at the & palatino linotype & expecto patronum\\
 at the & to the & magikos akademia & dressing gown\\
 he was & on the & alarte ascendare & grubbly plank\\
 to be & it was & inkosi inkosikazi & zacharias smith\\
 she was & he had & namby pamby & law enforcement\\
 i was & out of & modus operandi & auntie muriel\\
 and i & said ron & cuevas gontan & bathilda bagshot\\
 out of & into the & füvessy uram & goal posts\\
 going to & to be & toothflossing stringmints & pansy parkinson\\
 with a & in a & babbitty rabbitty & deathly hallows\\
 he had & from the & higgledy piggledy & phineas nigellus\\
 as he & said hermione & dawh dawh & king's cross\\
 in a & had been & shoop shoop & diagon alley\\
 for the & he said & loundon's towne & pumpkin juice\\
 was a & was a & farlin flookey & st mungos\\
 as she & of his & helter skelter & godrics hollow\\
 \hline
 \multicolumn{4}{| c |}{}\\
 \hline\hline
 \end{longtable}
 
Two random variable X, Y are independent iff their joint distribution is equal to the product of their marginal probabilities:
\begin{equation}
p( X, Y ) = p( X )p( Y )
\end{equation}
That is for all outcomes x, y:
\begin{equation}
p( X, Y ) = p( X )p( Y )
\end{equation}
So the mutual information "I" can be described as:
\begin{equation}
I(X; Y ) = 
\sum_{XY}^{}
p(X = x, Y = y) log p(X = x, Y = y)
p(X = x)p(Y = y)
\end{equation}
We find pairs of words \textit{wi, wj} that have high pointwise
mutual information, because this signifies the frequency count of their co-occurrence is much greater than how often each word appeared independently in the corpora, as seen in equation 4.  
\begin{equation}
    PMI(wi, wj ) = log\tfrac{p(wi, wj )}{p(wi)p(wj )}
\end{equation}

 In Table 1, you can see that the most probable bigrams aren't telling, but both the Canon and the Fanfiction feature common 'spells' from the text as their highest rated PMI bigrams.  From the canon you see  'avada kedavra' and 'expecto patronum' which were common spells from the books and films, and from the Fanfiction we see 'merus lumens' and 'alarte ascendare.'
 
 \begin{longtable}[c]{| c | c | c | c |}
 \caption{PMI Analysis on Verbs.\label{long}}\\
 \hline
 \multicolumn{2}{| c |}{Most Probable Bigrams} & \multicolumn{2}{| c |}{Highest PMI Bigrams}\\
 \hline
 Harry Potter Fanfiction & Harry Potter Canon & Harry Potter Fanfiction & Harry Potter Canon\\
 \hline
said said & said said & oyt cafru & slammed shut\\
let go & said looking & Erised oyt & starting feel\\
know said & do said & born dies & looking saw\\
said looking & know said & doo doo & trying sound\\
was was & said know & destroyed destroyed & came striding\\
go said & got said & cha cha & came hurrying\\
do said & I've got & de gnome & looking puzzled\\
have do & was said & drip drip & looking relieved\\
get said & is said & tick tick & looking bewildered\\
said know & said looked & beep beep & turned face\\
have said & said was & won won & trying catch\\
said looked & go said & captivate resonating & managed find\\
knew was & have said & click click & supposed be\\
asked said & said think &  live born & stopped talking\\
know is & said got & liked hated & wanted talk\\
know know & see said & vested pronounce & made feel\\
know do & get said & raptured ends & stood waiting\\
have go & asked said & ceases amaze & expecting see\\
see said & 's said & bid adieu & let go\\
want know & think said & loved hated & need talk\\
 \hline
 \multicolumn{4}{| c |}{}\\
 \hline\hline
 \end{longtable}
 
 The difference between unique co-occuring verbs between the fanfiction and the canon is telling.  One of the conclusions we can draw from the results of the PMI analysis of co-occuring verbs is writing style difference.  There are 4 main writing styles: Expository, Descriptive, Persuasive, and Narrative. The co-occuring verbs that were identified as the highest-valued unique concepts in the fanfiction (3rd column from the left) reveal a certain writing style that is most in common with 'Descriptive' and the Canon (last column in Table 2) is most in common with 'Narrative.'  In a descriptive writing style, the authors on average use language that lead by the five senses (what they hear, see, smell, taste, or touch), which is evidence by the "drip, drip" and "beep, beep" and "tick, tick" ranking amongst the highest PMI bigrams for this corpora.  By contrast, narrative style of writing is concerned with character development, constructing a story, conflict and setting, which is evidenced by the pleasant flow of co-occurring verbs in the canon.
 
 \begin{longtable}[c]{| c | c | c | c |}
 \caption{PMI Analysis on Events.\label{long}}\\
 \hline
 \multicolumn{2}{| c |}{Most Probable Bigrams} & \multicolumn{2}{| c |}{Highest PMI Bigrams}\\
 \hline
 Harry Potter Fanfiction & Harry Potter Canon & Harry Potter Fanfiction & Harry Potter Canon\\
 \hline
 (was, gone) & (wanted, watch) & (acknowledged, manifested) & (woke, remember)\\
 (love, hear) & (watch, was) & (orgasimed, griping) & (sleep, dozed)\\
 (drifted, sleep) & (was, rose) & (clamp, her mouth) & (fuming, hear)\\
 (turned, walked) & (rose, pressed) & (streaking, ripple) & (check, chose)\\
 (love, know) & (pressed, blinked) & (sed, shuld) & (clambered, hurried)\\
 (want, know) & (rolled, fell) & (hace, xplained) & (hurried, tell)\\
 (walked, left) & (fell, woke) & (contunue, document) & (living, giving)\\
 (knew, was) & (woke, remember) & (clanged, aperating) & (squeezed, could)\\
 (hope, enjoyed) & (was, heaving) & (reinforced, quenched) & (crumpled, burned)\\
 (was, be) & (slumped, fell) & (differ, a bushy - haired girl) & (avoid, hitting)\\
 (turned, left) & (looking, felt) & (rejuvenated, cleansed) & (hitting, groped)\\
 (knew, be) & (felt, was) & (delves, submerges) & (groped, smashed)\\
 (would, like) & (felt, fainted) & (punishing, pine) & (fighting, keep)\\
 (be, was) & (lay, looking) & (oohed, ahhed) & (know, meeting)\\
 (like, know) & (looking, sleep) & (memorised, visualised) & (meeting, holding)\\
 (know, was) & (sleep, dozed) & (dk, the little blue box) & (agrees, sent)\\
 (try, update) & (been, realized) & (proceeds, doodle) & (throws, getting)\\
 (left, left) & (wrenched, leaving) & (infatuated, unbelieving) & (getting, rid)\\
 (hope, liked) & (leaving, standing) & (releases, vanishes) & (go, turned)\\
 (had, was) & (standing, staring) & (bowing, restoring) & (cleared, read)\\
 
 \hline
 \multicolumn{4}{| c |}{}\\
 \hline\hline
 \end{longtable}
 
 In Table 3, an event was considered co-occuring if it occurred alongside another event in the same story and in the same chapter.  Events were extracted first using dependency parsing and semantic role labeling in conjunction with coreference resolution.  Each event consisted of a tuple with one verb and one argument (whether subject or object) and counted over the whole corpora.  The events here are not character dependent, this is an analysis over all the events found in the corpora in general.  Future work will include PMI analysis over co-occuring events within each character to delineate not only events that correspond to each character, but which events consititute a unique concept to that character.  These general results will also be applied in the future work as positive examples for predicitive modeling to predict an event given a previous event and/or it's temperal order.
 
 \subsection{Log-Odds Analysis}
 When comparing two corpora $A$ and $B$, it is of interest to determine whether certain words $w$ are more common in corpus $A$ than in corpus $B$, while controlling for their relative sizes. A simple metric that formally quantifies this notion is the log-odds-ratio defined as follows:
$$log \; odds \; of \; w = \frac{\frac{\# \; of \; occurences \; of \; w \; in \; A}{total \; \# \; of \; words \; in \; A}}{\frac{\# \; of \; occurences \; of \; w \; in \; B}{total \; \# \; of \; words \; in \; B}}$$

\subsubsection{Comparison of Corpora}. \label{corpus_level_odds}
We begin by performing a log-odds-ratio analysis to compare Harry Potter literature to a generic corpus of English language text. Table \ref{tab:compare_corpora} contains lists of tokens that appear out of place when specific pairs of corpora are compared. Unsurprisingly, we find that words pertaining to the Harry Potter books specifically, such as the names of characters, are statistically over-represented in both the Harry Potter canon and the fan fiction, relative to standard English. 

\begin{table}[htbp]
\centering
\resizebox{\columnwidth}{!}{
\begin{tabular}{|c|c|}
\hline
\textbf{Comparison} & \textbf{Tokens} \\ \hline
HP Canon vs. Standard English & hermione, hagrid, harry, dumbledore, weasley, malfoy, snape, harrys, ron, slughorn \\ \hline
HP Fan Fiction vs. Standard English & hermione, remus, ginny, draco, sirius, malfoy, harry, weasley, dumbledore, snape \\ \hline
HP Canon vs. HP Fan Fiction & scorpius, guy, alright, haired, figured, dorm, emma, hugo, amy, anyways, shit \\ \hline
\end{tabular}}
\caption{}
\label{tab:compare_corpora}
\end{table}

Next, we compare the canon to the fan fiction noting that terms such as `scorpius' and `hugo' appear more frequently in the fan fiction. `scorpius' likely refers to Scorpius Malfoy who is the son of Draco and Astoria Malfoy. Similarly, `hugo' likely refers to Hugo Granger-Weasley who is Hermione and Ron's child. These two characters never appear in the canonical books, and log-odds-ratio analysis is able to detect this fact. We also note that J.K. Rowling avoids the use of swear words in the original books, but this is not a constraint on the fan fiction as evidenced by the more frequent use of the word `shit'.

We note that in performing the above comparisons we randomly retained 10\% of the total fan fiction corpus in order to speed up the process of counting tokens. Future work may consider splitting the fan fiction stories to compare works by specific authors.

\subsubsection{Fan Fiction - Comparison of Character Behavior} \label{character_odds}

We are interested in examining whether the behavior of characters in the canon is noticeably different to their behavior in the fan fiction. We extract all verbs associated with a particular character from the narrative chains in which they appear as the protagonist. We then compare the verb counts for the character of interest against the verb counts for all the remaining protagonists using the log-odds-ratio. 

\begin{table}[htbp]
\centering
\resizebox{\columnwidth}{!}{
\begin{tabular}{|c|c|}
\hline
\textbf{Comparison} & \textbf{Tokens} \\ \hline
Voldemort & love, felt, run, write, stand, pull, head, help, hear, smile \\ \hline
Draco & belong, marry, own, knock, can, hang, gaze, apologize, protect, shove \\ \hline
Harry & belong, wink, mind, proceed, appreciate, remind, act, bear, dance, cross \\ \hline
Hermione & belong, fade, earn, rub, handle, happen, attempt, welcome, cut, transform \\ \hline
\end{tabular}}
\caption{}
\label{tab:compare_actions}
\end{table}

Table \ref{tab:compare_actions} contains lists of verbs that are statistically over-represented in the Harry Potter fan fiction for specific characters. Interestingly, characters such as Voldemort and Draco who are villains in the canon seem to have a softer side to them in the fan fiction. Voldemort in the fan fiction is associated with verbs such as `love', `feel', `help', and `smile'. Likewise, Draco is associated with `marry', and `apologize'. Notably, since verbs are being compared within the fan fiction corpus, these results imply that Voldemort and Draco are statistically `kinder' than other characters in the fan fiction. In addition, the results suggest that authors of fan fiction offer a more nuanced depiction of the canonical `bad guys' than is available in the original seven books. Finally, we note that Harry is associated with the verb `flirt'. In contrast, the canonical Harry is a shy and introverted character unlikely to overtly flirt with other characters. 

\end{document}