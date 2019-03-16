# Google's Neural Machine Translation with Attention from Arabic to English

## Background on Neural Machine Translation

Back in the old days, traditional phrase-based translation systems performed
their task by breaking up source sentences into multiple chunks and then
translated them phrase-by-phrase. This led to disfluency in the translation
outputs and was not quite like how we, humans, translate. We read the entire
source sentence, understand its meaning, and then produce a translation. Neural
Machine Translation (NMT) mimics that!

![](assets/encdec.jpg)

<p align="center">
Figure 1. <b>Encoder-decoder architecture</b> – example of a general approach for
NMT. An encoder converts a source sentence into a "meaning" vector which is
passed through a <i>decoder</i> to produce a translation.
</p>

Specifically, an NMT system first reads the source sentence using an *encoder*
to build
a
["thought" vector](https://www.theguardian.com/science/2015/may/21/google-a-step-closer-to-developing-machines-with-human-like-intelligence),
a sequence of numbers that represents the sentence meaning; a *decoder*, then,
processes the sentence vector to emit a translation, as illustrated in
Figure 1. This is often referred to as the *encoder-decoder architecture*. In
this manner, NMT addresses the local translation problem in the traditional
phrase-based approach: it can capture *long-range dependencies* in languages,
e.g., gender agreements; syntax structures; etc., and produce much more fluent
translations as demonstrated
by
[Google Neural Machine Translation systems](https://research.googleblog.com/2016/09/a-neural-network-for-machine.html).


## Output Example
![](assets/example.png)