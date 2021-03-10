# Rumi-Jawi

A list of Malay words in both the [Rumi] and [Jawi] (جاوي)
scripts. [Mohd Zamri Murah] compiled and expanded the original list
from various sources (see [here][rumi2jawi] for an older version of
the file). Michael Wayne Goodman performed some automatic corrections
and error detection (see the [commit history] for details), for which
Faizah Binte Zakaria verified or provided corrections.

[Rumi]: https://en.wikipedia.org/wiki/Malay_orthography
[Jawi]: https://en.wikipedia.org/wiki/Jawi_alphabet
[Mohd Zamri Murah]: https://github.com/mohdzamrimurah/
[rumi2jawi]: https://github.com/mohdzamrimurah/rumi2jawi
[commit history]: https://github.com/goodmami/rumi-jawi/commits/main

This dataset is free to use, but the license is not yet
decided. Hopefully CC-BY 4.0.

## Data Description

The dataset provides words in Standard Malay written in both the Latin
script Rumi and the Arabic script Jawi. The
[BCP-47](https://en.wikipedia.org/wiki/IETF_language_tag) language
tags are therefore:

* `zsm-Latn` (for Rumi)
* `zsm-Arab` (for Jawi)

The dataset contains modern spellings derived from dictionary sources,
and are suitable for tasks such as automatic transcription or spelling
correction. Historical spellings are not included, so it may have
reduced utility for transcribing older documents, but it may be useful
for other languages in the region, such as the Malay used in Brunei,
where Jawi has official status.

## Data Format

The [rumi-jawi.tsv](rumi-jawi.tsv) file is a [tab-separated values
file][TSV] with two columns: one for the Rumi spelling and one
for the Jawi. Here are the first 4 lines (with the header line):

    rumi	jawi
    aba	اب
    aba-aba	اب٢
    aba-daba	اب-داب
    abad	ابد

[TSV]: https://en.wikipedia.org/wiki/Tab-separated_values

## Other Details

Transcription between the two is not one-to-one; sometimes multiple
Rumi forms have the same form in Jawi, and sometimes multiple Jawi
forms have the same form in Rumi. In one case, reduplication can be
written in Jawi with the Arabic numeral 2 (`٢`) following the
reduplicated portion, as shown above for *aba-aba*, or it can be
spelled out with a hyphen. Thus, the distribution of pairs, unique
Rumi words, and unique Jawi words is shown in the following table:

| Type              | Count  |
| ----------------- | ------ |
| Pairs             | 66,321 |
| Unique Rumi words | 65,952 |
| Unique Jawi words | 64,237 |
