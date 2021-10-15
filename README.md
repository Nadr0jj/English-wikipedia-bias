# Goals
Create a series of tables to show...

1. The countries with the greatest and least coverage of politicians on Wikipedia compared to their population.   
2. The countries with the highest and lowest proportion of high quality articles about politicians (according to ORES).
3. A ranking of geographic regions by articles-per-person and proportion of high quality articles.

# Data Descriptions

## WPDS_2020_data.csv - https://www.prb.org/international/indicator/population/table/
Offered under a CC BY 4.0 license. Contains data on countries, regions, and measured population during 2019.

## page_data.csv - https://figshare.com/articles/Untitled_Item/5513449
Unsure of license. Contains  a list of (en) wikipedia articles with a revision id and the country which the politician serves in.

## population_data_mod.csv
The same as WPDS_2020_data.csv but with sub-regions manually added to a new column.

## wp_wpds_countries-no_match.csv
A list of page_data.csv wikipedia pages which could not be identified by ORES and therefore were unable to be assigned a predicted quality.

## wp_wpds_politicians_by_country.csv
A list of page_data.csv wikipedia pages which were identified by ORES and assigned a predicted quality. 

# Reflection (questions in python notebook)
Ultimately, I feel that the bias uncovered was not very surprising. It makes a lot of sense that the data would mostly reflect the community which primarily contributes to the data. I also believe the bias uncovered is at least in part due to the measurement used. Even though I believe in the conclusion, I'm not sure that a higher density of FA/GA articles is actually due to a western bias. It could be due to information availability. It's possible that some countries do not document politician behavior as thoroughly as others. If I were to be making a claim about the existence of bias in a more rigorous setting I would want to do a much more thorough investigation.
