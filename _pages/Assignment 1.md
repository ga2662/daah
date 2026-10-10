
---
title: "Assignment 1 - Science Fiction Explorer"
permalink: /assignment1/
layout: single
---

**## INTRODUCTION**

When my partner and I think of science fiction, we usually imagine space, aliens, and futuristic technology. But we started wondering whether science fiction is really about the future or if these imaginary worlds reflect problems that already exist in our own world, like fear, power, destruction, and survival.

For this assignment, we used the Science Fiction Explorer notebook to analyze around 1,000 science fiction texts from Project Gutenberg through distant reading. We focused on five words: fear, destruction, survival, power, and humanity.

We were especially interested in the war and society categories because we thought they might reveal more about human behavior and control. We expected "fear" and "destruction" to appear frequently in war stories, while "survival" might be more common in space travel or Mars stories. However, our results were not always what we expected, especially when it came to the word "power."

**## What Surprised Us**

When we first started experimenting with the custom word frequency section, we chose five words: "cosmos," "desolation," "dystopia," "detonation," and "armistice." We thought these words would be interesting because they seemed connected to science fiction, especially the themes of space, war, and destruction in the 1880s–1990s and we actually got this list from ChatGPT. However, when we looked at the results, we realized that some of these words barely appeared, and "dystopia" did not appear at all. This surprised us because dystopian worlds are something we usually associate with science fiction. We realized that just because a theme is common in a genre doesn't mean the exact word describing it will appear in the stories.

![Figure 1](/daah/assets/images/figure1.png)

*Figure 1: Heatmap showing the frequency of our original five words across the science fiction categories.*

Because of this, we decided to change our words to "fear," "destruction," "survival," "power," and "humanity." We felt these words would give us a better understanding of the human struggles we were interested in exploring.

![Figure 2]({{ '/assets/images/figure2.png' | relative_url }})

*Figure 2: Heatmap showing the total number of appearances of our revised five words across each category.*

Looking at our relative frequency heatmap, the word that stood out the most was "power." It had the highest relative frequency across all five categories, appearing around 0.60 times per 1,000 words in both space travel and war stories. We originally expected words like "fear" and "destruction" to be more common in war stories, so this was interesting to see. Fear was still relatively common, especially in Mars stories, where it appeared 0.29 times per 1,000 words. On the other hand, "survival" appeared surprisingly rarely, even in space travel stories, where we expected it to be more important.

![Figure 3]({{ '/assets/images/figure3.png' | relative_url }})

*Figure 3: Heatmap showing the relative frequency of our five words per 1,000 words.*

Another thing we noticed was the difference between the raw word counts and relative frequencies. For example, "power" appeared 10,206 times in society stories, which was the highest raw count. However, when we accounted for the number of words in each category, space travel and war had higher relative frequencies. This showed us why looking at raw counts alone could be misleading.

**## How Does Language Change Over Time?**

After looking at how often our words appeared across different categories, we wanted to see if the time period made a difference. We decided to compare two periods, 1880–1913 and 1900–1930, using the same five words. We chose these periods because we were interested in how World War I (1914–1918) might have influenced the language used in science fiction. The war introduced new forms of warfare and destruction, including tanks, chemical weapons, and more advanced military technology. We wondered whether experiencing such a major conflict might have changed how writers imagined the future, especially when it came to themes like fear, destruction, and power.

![Figure 4]({{ '/assets/images/figure4.png' | relative_url }})

*Figure 4: Heatmap showing the relative frequency of our five words between 1880 and 1913.*

One of the biggest differences we noticed was the word "power." In space travel stories, its relative frequency was 0.22 per 1,000 words in the 1880–1913 selection, compared to 0.57 in the 1900–1930 selection. We noticed something similar in war stories, where it went from 0.32 to 0.51. This made us wonder whether World War I and the growing importance of technology influenced how science fiction writers thought about power. After all, the war showed how technological developments could be used for destruction and control. However, we couldn't tell from the heatmaps whether writers were actually discussing military or technological power or something different.

![Figure 5]({{ '/assets/images/figure5.png' | relative_url }})

*Figure 5: Heatmap showing the relative frequency of our five words between 1900 and 1930.*

We also expected "fear" and "destruction" to become more common in the later period because of the war. Surprisingly, this wasn't always the case. In Mars stories, fear was actually slightly more frequent in the earlier selection, appearing 0.42 times per 1,000 words compared to 0.38 in the later one. In society stories, however, it was slightly higher in the later selection, going from 0.21 to 0.24. The relationship between historical events and the language used in science fiction might be more complicated than we originally expected.

One limitation of our comparison is that the periods overlap between 1900 and 1913, so some stories could be included in both results. Also, the 1900–1930 selection includes stories published before, during, and after World War I. Because of this, we cannot confidently say that the war caused these differences. To explore this properly, we would need to compare separate periods before and after 1918.

**## TF-IDF**

![Figure 6]({{ '/assets/images/figure6.png' | relative_url }})

*Figure 6: Bar graphs showing the top 15 most distinctive words in each category using TF-IDF.*

When we analyzed the TF-IDF section of the notebook, we looked at the five main tags: space travel, war, society, action, and Mars. The graph displayed the top fifteen distinctive words per category based on their TF-IDF scores, and what we found was that many of these words were character names. Even after filtering out several names, more continued to appear. This section was not exactly as helpful, unlike the earlier frequency heatmaps, the TF-IDF graph focused on words that stood out compared to the other categories, rather than how frequently our chosen words appeared.

**## KWIC**

![Figure 7]({{ '/assets/images/figure7.png' | relative_url }})

*Figure 7: Our KWIC settings for searching the word "power" with ten surrounding words on each side.*

![Figure 8]({{ '/assets/images/figure8.png' | relative_url }})

*Figure 8: KWIC results displaying the word "power" within sentences from different science fiction texts.*

After analyzing the TFIDF data results, we moved on to the keyword in context (KWIC) section of the notebook. Our focus was on the word “power”, as it appeared the most frequently used. We wanted to see how the word was actually being used in the context of the stories rather than the amount of times it appeared. For example, in the book Failure on Titan, we noticed that the word was used to describe both the ability of oneself to command others and gain obedience as well as the energy required to use weapons. Similarly, in Hostage of Tomorrow, the word was used to refer to atomic energy, but also to the authority held by leaders.

Some references were related to technology and energy, while others focused more on authority and human control. Unlike the earlier heatmaps, which only showed us how often certain words appeared, KWIC allowed us to look at the actual context in which they were being used.

**## What we learned and what we’d do differently**

One thing we found useful about computational analysis was being able to compare so many stories at once. Reading all 1,000 texts individually would have been impossible in the time we had, and even if we could, it would have been difficult to notice patterns across so many different stories. The notebook made it easier to compare words across categories and see which ones appeared more frequently. Although, it was a little frustrating because our first word choices didn't give us the results we expected and we had to keep experimenting to find something useful. The words we choose can completely change what we notice about a collection of stories.

This also made us think about the risks of distant reading discussed by Ted Underwood. Throughout our analysis we realized that although computational tools can help us identify patterns across a large number of texts these patterns still require deeper interpretation. It’s important to question the results we are given rather than assuming that the data tells us everything about the stories being analyzed.

What we would do differently if given more advanced technical skills would definitely have to be expanding on the different time periods of the metadata and how they affected the data and its abundance. We would also want to investigate how the meanings of certain words changed over time. Since we found that the word “power” could refer to both technology and human authority, it would be interesting to see whether one meaning became more common than the other during certain periods.

**## Collaboration Statement**

We both contributed to the research, analysis, and development of our essay. Aljazei focused on the introduction, frequency heatmaps, and comparisons between different time periods (Sections 1–3), while Ghaliah focused on analyzing the TF-IDF and KWIC results, as well as writing the final reflection and conclusion (Sections 4–6). We worked together to develop our research questions and interpret the overall findings.

**## AI Statement**

We used ChatGPT to help us brainstorm our initial list of words to analyze and to improve the clarity and structure of our writing. However, all the data analysis, interpretations, and conclusions were from the notebook.

**READY FOR GRADING**
