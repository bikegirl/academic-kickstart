Preliminary Results
===================

The following is an example of an event chain extracted from a story
from the fan fiction:

1.  ('CLUSTER 0', 'nsubj'), ('walked', 'root')

2.  ('CLUSTER 0', 'nsubj'), ('looked', 'root')

3.  ('CLUSTER 0', 'nsubj'), ('changed', 'root')

4.  ('CLUSTER 0', 'nsubj'), ('asked', 'root')

In the example above, the character in Harry Potter referred to as
'CLUSTER 0' first walks, then looks, changes, and finally asks. The
first element in every tuple is the word in the document with its
replaced coreference-resolution tag and the second element is its first
order dependency parse that was used to extract the event chain of every
noun subject of a story.

Results
=======

Pointwise Mutual Information (PMI) Analysis
-------------------------------------------

The most probable bigrams and the bigrams with the highest PMI were ran
over all words, verbs, and events of the two corporas: Harry Potter
Fanfiction and Harry Potter Canons. PMI analysis reveals the unique
co-occuring concepts in each of the corporas and highlights other
stylistic writing differences on average from the authors. Most probable
bigrams are shown along side the highest PMI bigrams in each of the
tables to show that the magnitude of the frequency count of each bigram
over total bigrams does not entail importance or significance in a
document and underscoring the value of PMI analysis.

::: {#long}
  ------------------------- -------------------- --------------------------- --------------------
   Harry Potter Fanfiction   Harry Potter Canon    Harry Potter Fanfiction    Harry Potter Canon
           of the                  of the              bibbidi bobbidi          avada kedavra
           in the                  in the               merus lumens            felix felicis
           to the                said harry             zauberei dorf           bertha jorkins
           it was                  he was                hoity toity           whomping willow
           on the                  at the             palatino linotype        expecto patronum
           at the                  to the             magikos akademia          dressing gown
           he was                  on the             alarte ascendare          grubbly plank
            to be                  it was             inkosi inkosikazi        zacharias smith
           she was                 he had                namby pamby           law enforcement
            i was                  out of              modus operandi           auntie muriel
            and i                 said ron              cuevas gontan          bathilda bagshot
           out of                 into the              füvessy uram              goal posts
          going to                 to be          toothflossing stringmints    pansy parkinson
           with a                   in a              babbitty rabbitty        deathly hallows
           he had                 from the            higgledy piggledy        phineas nigellus
            as he              said hermione              dawh dawh              king's cross
            in a                  had been               shoop shoop             diagon alley
           for the                he said              loundon's towne          pumpkin juice
            was a                  was a               farlin flookey             st mungos
           as she                  of his              helter skelter           godrics hollow
                                                                             
  ------------------------- -------------------- --------------------------- --------------------

  : PMI Analysis on Words.[\[long\]]{#long label="long"}
:::

Two random variable X, Y are independent iff their joint distribution is
equal to the product of their marginal probabilities:
$$p( X, Y ) = p( X )p( Y )$$ That is for all outcomes x, y:
$$p( X, Y ) = p( X )p( Y )$$ So the mutual information \"I\" can be
described as: $$I(X; Y ) = 
\sum_{XY}^{}
p(X = x, Y = y) log p(X = x, Y = y)
p(X = x)p(Y = y)$$ We find pairs of words *wi, wj* that have high
pointwise mutual information, because this signifies the frequency count
of their co-occurrence is much greater than how often each word appeared
independently in the corpora, as seen in equation 4.
$$PMI(wi, wj ) = log\tfrac{p(wi, wj )}{p(wi)p(wj )}$$

In Table 1, you can see that the most probable bigrams aren't telling,
but both the Canon and the Fanfiction feature common 'spells' from the
text as their highest rated PMI bigrams. From the canon you see 'avada
kedavra' and 'expecto patronum' which were common spells from the books
and films, and from the Fanfiction we see 'merus lumens' and 'alarte
ascendare.'

::: {#long}
  ------------------------- -------------------- ------------------------- --------------------
   Harry Potter Fanfiction   Harry Potter Canon   Harry Potter Fanfiction   Harry Potter Canon
          said said              said said               oyt cafru             slammed shut
           let go               said looking            Erised oyt            starting feel
          know said               do said                born dies             looking saw
        said looking             know said                doo doo              trying sound
           was was               said know          destroyed destroyed       came striding
           go said                got said                cha cha             came hurrying
           do said                I've got               de gnome            looking puzzled
           have do                was said               drip drip           looking relieved
          get said                is said                tick tick          looking bewildered
          said know             said looked              beep beep             turned face
          have said               said was                won won              trying catch
         said looked              go said          captivate resonating        managed find
          knew was               have said              click click            supposed be
         asked said              said think              live born           stopped talking
           know is                said got              liked hated            wanted talk
          know know               see said           vested pronounce           made feel
           know do                get said             raptured ends          stood waiting
           have go               asked said            ceases amaze           expecting see
          see said                's said                bid adieu                let go
          want know              think said             loved hated             need talk
                                                                           
  ------------------------- -------------------- ------------------------- --------------------

  : PMI Analysis on Verbs.[\[long\]]{#long label="long"}
:::

The difference between unique co-occuring verbs between the fanfiction
and the canon is telling. One of the conclusions we can draw from the
results of the PMI analysis of co-occuring verbs is writing style
difference. There are 4 main writing styles: Expository, Descriptive,
Persuasive, and Narrative. The co-occuring verbs that were identified as
the highest-valued unique concepts in the fanfiction (3rd column from
the left) reveal a certain writing style that is most in common with
'Descriptive' and the Canon (last column in Table 2) is most in common
with 'Narrative.' In a descriptive writing style, the authors on average
use language that lead by the five senses (what they hear, see, smell,
taste, or touch), which is evidence by the \"drip, drip\" and \"beep,
beep\" and \"tick, tick\" ranking amongst the highest PMI bigrams for
this corpora. By contrast, narrative style of writing is concerned with
character development, constructing a story, conflict and setting, which
is evidenced by the pleasant flow of co-occurring verbs in the canon.

::: {#long}
  ------------------------- --------------------- --------------------------------- ----------------------
   Harry Potter Fanfiction   Harry Potter Canon        Harry Potter Fanfiction        Harry Potter Canon
         (was, gone)           (wanted, watch)       (acknowledged, manifested)        (woke, remember)
        (love, hear)            (watch, was)            (orgasimed, griping)            (sleep, dozed)
      (drifted, sleep)           (was, rose)             (clamp, her mouth)             (fuming, hear)
      (turned, walked)         (rose, pressed)           (streaking, ripple)            (check, chose)
        (love, know)         (pressed, blinked)             (sed, shuld)             (clambered, hurried)
        (want, know)           (rolled, fell)             (hace, xplained)             (hurried, tell)
       (walked, left)           (fell, woke)            (contunue, document)           (living, giving)
         (knew, was)          (woke, remember)          (clanged, aperating)          (squeezed, could)
       (hope, enjoyed)         (was, heaving)          (reinforced, quenched)         (crumpled, burned)
          (was, be)            (slumped, fell)     (differ, a bushy - haired girl)     (avoid, hitting)
       (turned, left)          (looking, felt)         (rejuvenated, cleansed)        (hitting, groped)
         (knew, be)              (felt, was)             (delves, submerges)          (groped, smashed)
        (would, like)          (felt, fainted)            (punishing, pine)            (fighting, keep)
          (be, was)            (lay, looking)              (oohed, ahhed)              (know, meeting)
        (like, know)          (looking, sleep)         (memorised, visualised)        (meeting, holding)
         (know, was)           (sleep, dozed)         (dk, the little blue box)         (agrees, sent)
        (try, update)         (been, realized)           (proceeds, doodle)           (throws, getting)
        (left, left)         (wrenched, leaving)      (infatuated, unbelieving)         (getting, rid)
        (hope, liked)        (leaving, standing)        (releases, vanishes)             (go, turned)
         (had, was)          (standing, staring)         (bowing, restoring)           (cleared, read)
                                                                                    
  ------------------------- --------------------- --------------------------------- ----------------------

  : PMI Analysis on Events.[\[long\]]{#long label="long"}
:::

In Table 3, an event was considered co-occuring if it occurred alongside
another event in the same story and in the same chapter. Events were
extracted first using dependency parsing and semantic role labeling in
conjunction with coreference resolution. Each event consisted of a tuple
with one verb and one argument (whether subject or object) and counted
over the whole corpora. The events here are not character dependent,
this is an analysis over all the events found in the corpora in general.
Future work will include PMI analysis over co-occuring events within
each character to delineate not only events that correspond to each
character, but which events consititute a unique concept to that
character. These general results will also be applied in the future work
as positive examples for predicitive modeling to predict an event given
a previous event and/or it's temperal order.

Log-Odds Analysis
-----------------

When comparing two corpora $A$ and $B$, it is of interest to determine
whether certain words $w$ are more common in corpus $A$ than in corpus
$B$, while controlling for their relative sizes. A simple metric that
formally quantifies this notion is the log-odds-ratio defined as
follows:
$$log \; odds \; of \; w = \frac{\frac{\# \; of \; occurences \; of \; w \; in \; A}{total \; \# \; of \; words \; in \; A}}{\frac{\# \; of \; occurences \; of \; w \; in \; B}{total \; \# \; of \; words \; in \; B}}$$

### Comparison of Corpora

. [\[corpus\_level\_odds\]]{#corpus_level_odds
label="corpus_level_odds"} We begin by performing a log-odds-ratio
analysis to compare Harry Potter literature to a generic corpus of
English language text. Table
[\[tab:compare\_corpora\]](#tab:compare_corpora){reference-type="ref"
reference="tab:compare_corpora"} contains lists of tokens that appear
out of place when specific pairs of corpora are compared.
Unsurprisingly, we find that words pertaining to the Harry Potter books
specifically, such as the names of characters, are statistically
over-represented in both the Harry Potter canon and the fan fiction,
relative to standard English.

Next, we compare the canon to the fan fiction noting that terms such as
'scorpius' and 'hugo' appear more frequently in the fan fiction.
'scorpius' likely refers to Scorpius Malfoy who is the son of Draco and
Astoria Malfoy. Similarly, 'hugo' likely refers to Hugo Granger-Weasley
who is Hermione and Ron's child. These two characters never appear in
the canonical books, and log-odds-ratio analysis is able to detect this
fact. We also note that J.K. Rowling avoids the use of swear words in
the original books, but this is not a constraint on the fan fiction as
evidenced by the more frequent use of the word 'shit'.

We note that in performing the above comparisons we randomly retained
10% of the total fan fiction corpus in order to speed up the process of
counting tokens. Future work may consider splitting the fan fiction
stories to compare works by specific authors.

### Fan Fiction - Comparison of Character Behavior {#character_odds}

We are interested in examining whether the behavior of characters in the
canon is noticeably different to their behavior in the fan fiction. We
extract all verbs associated with a particular character from the
narrative chains in which they appear as the protagonist. We then
compare the verb counts for the character of interest against the verb
counts for all the remaining protagonists using the log-odds-ratio.

Table
[\[tab:compare\_actions\]](#tab:compare_actions){reference-type="ref"
reference="tab:compare_actions"} contains lists of verbs that are
statistically over-represented in the Harry Potter fan fiction for
specific characters. Interestingly, characters such as Voldemort and
Draco who are villains in the canon seem to have a softer side to them
in the fan fiction. Voldemort in the fan fiction is associated with
verbs such as 'love', 'feel', 'help', and 'smile'. Likewise, Draco is
associated with 'marry', and 'apologize'. Notably, since verbs are being
compared within the fan fiction corpus, these results imply that
Voldemort and Draco are statistically 'kinder' than other characters in
the fan fiction. In addition, the results suggest that authors of fan
fiction offer a more nuanced depiction of the canonical 'bad guys' than
is available in the original seven books. Finally, we note that Harry is
associated with the verb 'flirt'. In contrast, the canonical Harry is a
shy and introverted character unlikely to overtly flirt with other
characters.
