# Notes

For my project, I am planning to create a classifier that uses visual (movie poster) and textual (title, plot summary) features to predict the potential genres of movies.

I am planning to use this as a lab log.

16.12.20: 
- Loaded the movie data that was given in a csv file.
- Filtered out the columns I did not need and only kept the title, the overview, the movie id and the genre column.
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
- Used pickle module to save the tensors.
