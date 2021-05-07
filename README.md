# Humanitarian-Data-Classification

## Last Updated: March 2021

## Objective

The objective of this framework is to detect, classify, and recommend a category of data in the context of natural disasters and humanitarian emergencies. The categories of humanitarian data collected during an onset of a crisis is usually limited to the most immediate needs of a population. By identifying these categories and classifying incoming data, humanitarians and information managers can focus on collecting, cleaning, and utilizing information while automatically classified data is analyzed and mapped.

The notebook may change as I try new methodologies, datasets, and models.

## Methodology

Over 2,000 datasets were scraped from the Humanitarian Data Exchange (HDX). The datasets pulled had Humanitarian Exchange Language (HXL) tags, which identify the type of data. This data was processed and distilled down to a certain number of tags that are only relevant to rapid needs assessments. These tags were then turned into categories for a training set for our model.

Word embeddings were created using fastText, an NLP library created by Facebook. An MLP model is then trained using these word embeddings.

Assorted rapid needs assessment datasets are then tested to see the model's accuracy.
