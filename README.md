auto-phrase-tokenfilter
=======================

Lucene Auto Phrase TokenFilter implementation


Performs "auto phrasing" on a token stream. Auto phrases refer to sequences of tokens that
are meant to describe a single thing and should be searched for as such. When these phrases
are detected in the token stream, a single token representing the phrase is emitted rather than
the individual tokens that make up the phrase. The filter supports overlapping phrases.

The Autophrasing filter can be combined with a synonym filter to handle cases in which prefix or
suffix terms in a phrase are synonymous with the phrase, but where other parts of the phrase are
not. This enables searching within the phrase to occur selectively, rather than randomly.

##Overview
Forked from https://github.com/LucidWorks/auto-phrase-tokenfilter and updated to work for Solr5. The usage of it is same as explained in the forked project. 
