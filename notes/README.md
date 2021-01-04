# Notes

For my project, I am planning to create a classifier that uses visual (movie poster) and textual (title, plot summary) features to predict the potential genres of movies.

I am planning to use this as a lab log.

16.12.20: 
- Loaded the movie data that was given in a csv file.
- Filtered out the columns I did not need and only kept the title, the overview, the movie id and the genre column.
- Filtered out all genres that appeared only once and did not really make sense.
- Given the weird formatting of the genre column, I did some necessary cleaning to make accessing the genres more convenient.
- Made a plot to visualize the genre distribution.

17.12.20:
- Made a function to retrieve the movie posters using the TMDB (TheOpenMovieDatabase) API.
- Download the posters locally - it takes very long to run the get_data function on the whole dataframe.
- Added a poster column to the dataframe.

18.12.20:
- Changed the function that retrieves the posters to return the path to the local directory, which I save the images at.
- Created training, validation and test sets.
- Saved the training, validation and test sets to csv files.

19.12.20:
- Made a function that resizes images,  converts them to RGB images and then stores them to a tensor and saves them to the GPU.
- Iterated through the train, validation and test dataset and created tensors out of all posters.
- Used pickle to save the tensors of tensors for future save.

20.12.20:
- Did some cleaning up on the code.
- Documented what I have done up to now.

21.12.20:
- Realized that if I wanted to use titles as an input to my model I should have excluded non English titles, so I decided to write a function to filter them out.

31.12.20:
- Did some research on multi label classification and came across the MultiLabelBinarizer from sklearn.preprocessing, so I made a function to transform the labels for each movie into a one hot encoding.
- Had to convert the string representation of each list of labels into a regular list so that I could fit the list of lists binarizer and then tranform the label sets.

02.01.21:
- Made a bar plot to visualize the distribution of number of labels per movie in my data.

04.01.21:
- Started research on what methods to use to preprocess the textual data. I decided to use a slightly modified cleaning up function for the title string and the overview string since certain titles contain solely stop words (e.g. 'Who am I?') and removing stop words in this case would return an empty string.
