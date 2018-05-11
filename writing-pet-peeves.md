# Writing Pet Peeves

## Grammar and Style

+ Use superlatives and "hype phrases" sparingly - things like "drammatically improves the user experience" - unless it's actually warranted. If you improve precision from 0.4 to 0.8, calling the improvements _dramatic_ might be warranted. A 5% improvement is not. I would let the results speak from themselves. Overuse of superlatives potentially turns off reviewers.

+ Related, use the term _significant_ only in the technical sense of statistically significant.

+ Stay in the same tense! Some authors like to describe experiments in the past tense, e.g., "The user received a push notification and clicked on it." Others like to describe experiments in the present tense, e.g., "The user receives a push notification and clicks on it." Both are fine, but stay consistent in the same tense. Don't write, "The user receives a push notification and clicks on it. The click was then recorded by the server."

+ "Related work", **not** "related works". "Work" is a collective noun, like "staff". You don't write "research staffs". Wait, you ask: if this is indeed the case, why would you write ["DaVinci is the creator of several famous _works_ of art"](https://twitter.com/mmparker/status/991012314332545024)? Well, that's a completely different context: "work" in "related work" is intended to refer to a body of work collectively, as in "the literature". You don't write "related literatures" (well, except in a very narrow sense, something like "isolated silos of related literatures"). Note that "DaVinci's work" and "DaVinci's works" are both fine, but in different contexts. The first might refer to his body of work collectively; the second focuses on individual pieces. Also, be aware of subject-verb agreement.

+ Common noun-verb (note that in Latex this would be an en-dash, see below) agreement issue: "number of sample increases", not "increase". The verb agrees with the head noun, which is number, singular in this case.

## Latex

### Finer Points of Punctuation

+ Learn the difference between [an hyphen, en-dash, and em-dash](http://www.thepunctuationguide.com/hyphen-and-dashes.html).

  + It's `key--value` as in `key--value` store, not `key-value`.

  + It's `human--computer interaction`. Note that the [Wikipedia article](https://en.wikipedia.org/wiki/Human%E2%80%93computer_interaction) gets it right and [this incorrect URL](https://en.wikipedia.org/wiki/Human-computer_interaction) redirects to the correct article.

+ Footnotes go after the punctuation, as in `End of sentence.\footnote{...}`. Note, there is _no_ space between punctuation and the footnote.

+ There is a difference between end-of-sentence spacing and intra-sentence spacing after a period. For example, `cat vs.\ dog` but `I like cats. She likes dogs.`

### Citations

+ Cite a reference as `Lin et al.~\cite{Lin}`. Note `~` prevents ugly breaks.

+ **NEVER** *ever* begin a sentence with a citation. e.g., "[5] explored the use of..."

+ A citation is not a noun phrase, e.g., "is shown in [5]" is bad; should be "is shown by Smith et al. [5]". (Although I break this rule myself sometimes.)

+ Name your proceeding volumes consistently in the bibliography.

### Misc

+ Latex does weird hyphenation on line breaks sometimes. For example, analysis might get hyphenated as "anal-ysis", which just looks dirty. MapReduce gets hyphenated as "MapRe-duce", which bugs me. Insert in the preamble `\hyphenation{Map-Reduce}` to specify particular hyphenations you want, or use `\mbox{...}` to suppress hyphenation.