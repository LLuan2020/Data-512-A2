# Bias in Data

## Goal 

The goal of this assignment is to explore the concept of bias through data on Wikipedia articles - specifically, articles on political figures from a variety of countries.

## Data Sources 

Data from the following sources were used for this analysis:

The Wikipedia politicians by country dataset can be found on [Figshare](https://figshare.com/articles/dataset/Untitled_Item/5513449). This dataset contains a subset of metadata info of articles on politicians published in the English version of Wikipedia.

World Population Datasheet by Population Research Bureau. This dataset is drawn from the [world population data sheet](https://www.prb.org/international/indicator/population/table/) published by the Population Reference
Bureau.

## API Documentation

To get the predicted quality scores for each article in the Wikipedia dataset. We're using a machine learning system called ORES. This was originally an acronym for
"Objective Revision Evaluation Service" but was simply renamed “ORES”. ORES is a machine learning tool that can provide estimates of Wikipedia article quality. The article quality estimates are, from best to worst:

- FA - Featured article
- GA - Good article
- B - B-class article
- C - C-class article
- Start - Start-class article
- Stub - Stub-class article

## Dataset

| Column Name  | Description |
| ------------- | ------------- |
| country  | This is the country which the article belongs to  |
| article_name  | The name/title of the article  |
| revision_id  | A unique number that identifies the article  |
| article_quality_est  | The ORES prediction of the quality of the article  |
| population  | 	The population of the country  |

## Results

There are six tables showing the following results.

1. Top 10 countries by coverage: 10 highest-ranked countries in terms of number of
politician articles as a proportion of country population
2. Bottom 10 countries by coverage: 10 lowest-ranked countries in terms of number of
politician articles as a proportion of country population
3. Top 10 countries by relative quality: 10 highest-ranked countries in terms of the
relative proportion of politician articles that are of GA and FA-quality
4. Bottom 10 countries by relative quality: 10 lowest-ranked countries in terms of the
relative proportion of politician articles that are of GA and FA-quality
5. Geographic regions by coverage: Ranking of geographic regions (in descending
order) in terms of the total count of politician articles from countries in each region
as a proportion of total regional population
6. Geographic regions by coverage: Ranking of geographic regions (in descending
order) in terms of the relative proportion of politician articles from countries in each
region that are of GA and FA-quality
