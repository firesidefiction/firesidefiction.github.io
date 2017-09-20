---
layout: blackspecfic
title: "Antiblack Racism in Speculative Fiction"
author: Cecily Kane
date: 2016-07-26 00:01:00 -0500
category: "#Blackspecfic"
permalink: /blackspecfic-2015
teaser: "#BlackSpecFic: A Fireside Fiction Company special report"
published: true
---

For many science fiction and fantasy writers, the value of a solid bibliography of short fiction cannot be understated. While sales often aren’t lucrative enough to be an independent income stream, it can lead to novel solicitations, columns, editorial positions, and other work that can lead to a higher profile and more opportunities. [Having published short fiction helps a writer expose their ideas to the wider community and build an audience, a brand, and a foundation from which to grow their careers](http://www.sfwa.org/2015/02/ten-reasons-write-short-stories-even-though-pay-peanuts/).

> The field of short science fiction and fantasy — at least U.S. publications, which make up the bulk of the field — is essentially not publishing black writers. This locks them out of this valuable process.

I first noticed this in the anthology market. Several anthologies that I looked at, that I read, and even that I initially reviewed positively looked pretty diverse until I took a closer look at their table of contents, which appeared to have zero stories written by black people. I knew of several other anthologies with missions of publishing black authors specifically or people of color generally, so I was pretty sure that this pattern wasn’t in alignment with the actual demographics of the field. At the same time, someone I know, Ethan Robinson, was noticing the same thing about the magazine markets.

[And he began to count](https://docs.google.com/spreadsheets/d/1Humm9VHch7bFvJvCFxH8KkH9C1OpUkeHaSTM0xVBo94/edit?usp=sharing).

## Initial Analysis

The methodology is flawed, as it’s based in self-reported data whenever possible, but such data was not always findable or clear. I consulted an actuary, Weston Allen. He and I assumed that there may have been a few false positives and false negatives, but not in such numbers as to unduly dilute the study.

And the numbers are very damning. Out of 2,039 original stories published in 63 magazines in 2015, only 38 stories could be found that were written by black authors.

![](/images/graphics/blackspecfic2015-1.png)

That’s just under 2%. The median number of stories by black authors in these magazines is zero, which means that more than half of all speculative fiction publications measured did not publish a single original story by a black author in the year of 2015.

To adjust for the methodological flaws, as well as the fact that we don’t have access to submission-rate data concerning race and ethnicity either overall or by individual magazine, we used binomial distributions. The purpose of this was to find the probability that such numbers could be random — the chances that numbers like that could exist without biases in play (which could extend to biases that are literary in nature, such as story structure), systemic problems, and/or structural gaps. In the first binomial distribution we ran the data assuming that submission rates of black authors are equal to the proportion of the black population in the United States, which was 13.2% in 2015 ([according to Census projections](http://www.census.gov/population/projections/files/summary/NP2012-T6.xls)).

Under this assumption, the probability of the 1.9% average occurring by random chance is 3.21x 10^-76, or **0.000000000000000000000000000000000000000000000000000<br/>00000000000000000000000000321%**. For comparison’s sake, the odds of winning the New Jersey Pick Six lottery are 7.15x 10^-08, or 0.00000714%

## Alternate analysis

In order to provide more useful analytics for authors’ submission, we created a second binomial distribution assuming that the submission rates of black authors are actually equal to the sample average of 1.9%. Under this assumption, which is the most charitable to whiteness as possible, some magazines still have a very unlikely proportion of black authors represented in the sample.

This latter assumption’s yieldings are most useful for comparing individual magazines. It is theoretically possible that only 1.9% of submitted stories are written by black authors. But even under that assumption, 0 of 5 stories in a magazine is a far more likely result than 0 of 150, and is far less likely to imply bias. (Caveat: due to the limitations of the methodology and the tiny numbers, individual comparisons per magazine are less reliable than the overall data set; one false positive or negative can change a given single magazine’s numbers greatly, especially if it’s a relatively low-volume magazine, but will exhibit only a tiny fractional change on the mean as a whole or the first probability distribution.)

A more detailed breakdown of all these numbers, including ones for individual publications, can be found in [this spreadsheet](https://docs.google.com/spreadsheets/d/1Humm9VHch7bFvJvCFxH8KkH9C1OpUkeHaSTM0xVBo94/edit?usp=sharing).

## Conclusions

For this report, we focused on black authors specifically rather than authors of color generally because, while all are important, we noticed several patterns — not limited to the short fiction field — in which “diversity” initiatives excluded black people and hid antiblackness. The terms “people of color” and “PoC” can have a flattening effect, so we took a closer look than the white/not-white binary.

We still don’t know submission rates, and gathering data on them would be enormously difficult. But the fact that [Terraform](http://motherboard.vice.com/terraform)—which exists further on the outskirts of the historical and sociocultural speculative short fiction field than likely any other publication in this data set and is not going out of its way to publish stories by black authors—appears to have published 8–9% black authors suggests that the number of stories by black writers within the average submission rate is greater than 2% and likely closer to Terraform’s average. (For more about that, see note at end.)

Furthermore, even in the unlikely event that only around 2% of all stories in all submission piles across the field are written by black authors, given that the chances of that possibility being random is likewise 0%, we need to examine the real problem: systemic racism. Speculative short fiction publishing is rife with antiblackness, and white speculative fiction writers and publishers need to stop pretending otherwise.

## About This Report

The underlying data was gathered by Ethan Robinson. The statistical analysis of the data was provided by Cecily Kane, who has an accounting background, and Weston Allen, an actuary by profession. The report was written by Cecily in consultation with several authors of color, and it was edited by Fireside publisher Brian White.

- The initial dataset included two magazines that are not included in this study. [Omenana](https://omenana.com/) is headquartered in Nigeria, and its principal intended audience is African, as are its published authors. [Truancy](http://www.delinquentspice.com/) is headquartered in Malaysia, and similarly occupies another literary center. Both are part of the field, but are distant enough from the center of the system we are critiquing that we felt inclusion of any measurements to be unnecessary and perhaps distorting.

- When Terraform was asked if it was intentionally going out of its way to publish black authors, its editors said this: “To answer your question, to be perfectly honest, we don’t have any particular directive to specifically publish black authors, no. We do have an interest in publishing diverse voices generally. If a submission about the dystopian future of online dating in China comes across our desk, or about how Botswana’s virtual world may suffocate citizens in times of climate change, we will gravitate towards those stories naturally because they help paint a fuller portrait of speculation than we’d otherwise get. If you’re publishing speculative fiction, you can’t get a complete picture of how humans are thinking about the future unless you’re inclusive of as many voices as possible. Our interest in science/speculative fiction has always been rooted, in part, in an appreciation for its power as a tool of social criticism.”
