# Text to Categorical MATLAB Function

## Purpose

The intention of this function is to assist with the cleaning of text data, converting it into categorical data based on the presence of keywords. There doesn’t seem to be a built in or well-known way of completing this task. 

##Design

The function takes two inputs, a column of text data and a predefined list of categories to check for within the text data. Each entry is checked and converted to the relevant category if the associated keyword is found. It may be possible to complete this task with a better efficiency than the current implementation. Something of note is that this approach will replace NaN values with the “Other” category, which is also the default for any item not containing a substring. This may or may not be desirable depending on the data set.

##Relevance

This function is helpful when attempting to visualize general trends within text data. It was written to convert descriptive entries from an archaeological data set into categories for the purpose of visualization and analysis and accomplished this task quite well.
