---
permalink: /assignment2/
title: "Assignment 2"
---
# Mapping Occupational Diversity in Lorimer's Gazetteer of the Persian Gulf

## Introduction
For our second Digital Humanities assignment, we decided to explore the geographical distribution of occupations displayed in J. G. [Lorimer's Gazetteer of the Persian Gulf, Oman and Central Arabia](https://drive.google.com/file/d/1pg-2MlWpdAkEhf-_9UDEs0Qvmlel0w6j/view?usp=sharing). We were interested in understanding how different forms of work were represented across the region and whether specific locations had a greater variety of recorded occupations than others. Rather than focusing on one particular line of work, we wanted to analyze occupational diversity and see whether there were any geographical patterns that might not be immediately noticeable when reading the text itself.

The reason behind our choosing of Lorimer's Gazetteer is because it contains detailed descriptions of settlements, communities, and economic activities across the Gulf and surrounding regions. However, much of this information is presented through written descriptions rather than a structured dataset, which makes it increasingly difficult to compare different locations in a straightforward way. By identifying occupations and connecting them to geographical coordinates, we wanted to see how historical information could be transformed into something that was easier to analyze and visualize.

Our main research question was: How does the diversity of occupations documented in Lorimer's Gazetteer vary across different geographical locations in the Gulf region?

## Methodology and Data Collection

We began by examining Lorimer's Gazetteer to identify occupations documented across different geographical locations. We approached this process manually by reading geographical entries, using the search function to locate relevant terms, and examining screenshots of the original text. We used an LLM (ChatGPT) to help extract occupations from screenshots of the original text, but manually reviewed the results to verify the results and identify any contextual errors/inaccuracies. One of the prompts we used asked ChatGPT to identify the occupations mentioned in a paragraph and organize them into a table, with TRUE and FALSE values indicating whether each occupation was documented. We also used the following prompt to help organize geographical information. “Use this datasheet to find the latitude and longitude for the places we listed and extract the points into a list with three columns: place, latitude, and longitude.”


![Screenshot of Lorimer's Gazetteer]({{ '/assets/images/lorimer-screenshot.png' | relative_url }})
(Example of one entry)

One of the biggest challenges was collecting enough data because occupations were not always mentioned directly or consistently. Sometimes they appeared as specific professions, while other times they were included within broader descriptions of economic activities. This meant that we had to go through different sections of the text and connect the relevant occupation to a geographical location.

After collecting the information, we organized everything into an Excel spreadsheet. Each row represented a geographical location, while the columns represented different occupations. We used Y and N values to indicate whether an occupation was documented in a particular location. This allowed us to organize information that was originally scattered throughout the text into a dataset that we could compare and analyze.
Our main spreadsheet contained 261 place records and 84 occupation categories, with 646 positive occupation entries. We then used the spreadsheet to calculate the number of different occupations recorded at each location. Another challenge involved finding geographical coordinates for historical locations. Some place names were spelled differently from their modern equivalents, while others were difficult to locate using contemporary maps. To address this, we used the place name dataset provided by our professor, [Professor's Place Name Dataset](https://zenodo.org/records/20122587) A Dataset of Place Names from J. G. Lorimer's Gazetteer of the Persian Gulf, Central Arabia and Oman (1908). We also used [GeoNames](https://www.geonames.org/), the original Gazetteer, and OpenGulf to help identify and verify geographical locations.

Once we had organized the information, we prepared a CSV file containing the geographical coordinates and occupation counts so that we could import our dataset into [Kepler.gl](https://kepler.gl/)

## Data Visualization

For our visualization, we decided to use Kepler.gl because it allowed us to explore our dataset through an interactive geographical map. We wanted to create something that would make differences in occupational diversity easier to understand compared to looking at the information in Excel.

We experimented with different settings before deciding to use a 3D hexagonal map. The map groups nearby geographical locations into hexagonal areas, while the height and color of each column represent the average number of different occupations recorded within that area. Taller columns indicate higher average occupational diversity, while shorter columns represent lower averages.
We chose blue, green, and yellow to make the columns easier to distinguish and included a legend and interactive tooltips so that viewers could explore the information themselves.

One thing we found particularly interesting was how different the data looked once we transferred it from Excel into Kepler.gl. When we were working with the spreadsheet, the information mainly appeared as rows, columns, and numbers, which made it difficult to understand the geographical relationships between locations. However, once we created the map, we could see the spread and clustering of the recorded occupations much more clearly.

However, we also had to consider how the visualization settings affected the way our data was presented. Since we used hexagonal aggregation, each column represents an average across locations within an area rather than the occupation count of one specific settlement. This made us realize that the way data is visualized can influence how people interpret it.

<iframe
  src="{{ '/assets/maps/lorimer_occupation_diversity_safe.html' | relative_url }}"
  width="100%"
  height="650"
  style="border: 0;"
  title="Interactive 3D Map of Occupational Diversity">
</iframe>


## Findings and Analysis

One of the first things we noticed when examining our dataset was that certain occupations appeared much more frequently than others. Fishing was the most commonly recorded occupation, appearing in 98 place records, followed by cultivation in 82 and pearl diving in 81. Date cultivation was also frequently documented, appearing in 63 records.

These findings highlight the importance of maritime activities and agriculture's significance in our dataset. Although the numbers do not tell us how many people practiced each occupation, they show which forms of work were documented most frequently.
Other occupations appeared less frequently. For example, weaving appeared in 18 records, boat building in 11, and blacksmithing in five. However, this does not necessarily mean that these professions were uncommon in reality, since our results depend on what Lorimer chose to document.

We also noticed considerable variation in the number of occupations recorded at individual locations. Some places had only one documented occupation, while others had a much greater variety. The highest occupation count in our main spreadsheet was 20 for Anaizah, followed by another Anaizah entry with 19 and Shushtar Town with 18.

However, the two Anaizah entries also made us consider how historical place names and repeated entries could affect our analysis. This showed us why organizing and checking the dataset was just as important as creating the visualization itself.
Our 3D map also showed differences in recorded occupational diversity across geographical areas, with visible clusters and variations in column height that were harder to recognize in Excel.

At the same time, we had to be careful about how we interpreted these patterns. A location with more recorded occupations does not necessarily mean that it had a more diverse economy than another location. It could also mean that Lorimer provided a more detailed description of that particular place. Because of this, we understood our findings as patterns in documented occupational diversity rather than a complete representation of economic activities across the region.

## Limitations and Reflection

One of the main limitations of our project was the historical source itself. Lorimer's Gazetteer was not originally written to provide a complete dataset of occupations, which meant that the amount of information available varied between locations. Some settlements were described in considerable detail, while others had much shorter entries. This could affect the number of occupations we were able to identify and make comparisons between locations less straightforward.

Another limitation was the process of converting historical descriptions into Y and N values. Although this made the information easier to organize and analyze, it also simplified the original text. For example, recording that fishing was mentioned at a location did not tell us how many people worked as fishermen or how important fishing was to the local economy. Our dataset therefore focused on whether an occupation was documented rather than the scale of that occupation.

This experience also made me realize that digital humanities involves much more than simply using digital tools. The quality of a visualization depends heavily on how the information was collected, organized, and interpreted before it was uploaded. Even though the map was the most visually interesting part of our project, the research and data preparation were just as important.

## Conclusion

Overall, this assignment allowed us to explore how occupational diversity was documented across the Gulf by transforming historical descriptions into structured data and an interactive map.

More importantly, this project helped us understand that digital tools do not automatically make historical information complete or objective. The patterns we see depend on the original source, the decisions we make when collecting and organizing information, and the way we choose to visualize it. Through this assignment, I developed a better understanding of how digital humanities can make historical information more accessible while also encouraging us to question what the data actually represents.

## References

Lorimer, J. G. Gazetteer of the Persian Gulf, Oman and Central Arabia.

A Dataset of Place Names from J. G. Lorimer's Gazetteer of the Persian Gulf, Central Arabia and Oman (1908). Zenodo.

GeoNames. (https://www.geonames.org/)

OpenGulf. (https://opengulf.github.io/)

Kepler.gl. (https://kepler.gl/)

