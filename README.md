# Datathon-IISc, Session-based Fashion Recommendation System.


Problem Statement and Dataset:
We have been given 16K images of apparel from an ecommerce website. We've to design a fashion recommendation system for window shopping. At every time instant, a user is shown 4 images and he has to like 0 or more images. Based on his selection and the previously collected data, we have to show him next 4 images. The aforesaid is repeated, till the user chooses to quit.

Methodology used-
Exploration and Exploitation Strategy: A parameter alpha to give some weightage to exploration and partly to exploitation.
For exploitation, we used Mobilnet V2 embeddings for each of the image and used them for finding the most similar images to the selected image.
Used epsilon smoothing strategy for exploitation which allowed to factor in the previous likes of the user in the same session.
For exploration, we showed images randomly from the least exploited images.
And the parameter alpha keeps on decreasing implying that we give more importance to exploitation as time goes by.


Run Instructions
Run the cell with the main function.
Select the images which you like. Get the corresponding outputs. 
Repeat the last line.


#


