# Movie-Recommendation-System-
This is a content-based movie recommendation system which mostly suggests movies on the basis of the kind of stories users likes to see which uses cosine similarity algorithm by comparing all the movies with each other 
# Data Collection 
Collected movies and credits data from kaggle which has list of 5000 movies which are popular and highly rated on many popular websites 
# Data Prepocessing
Removed missing and duplicated values from the dataset as well empty column which ads nothing substancial to the data and the combines both movies and credits tables on the title column which was common in both of them 
Converted Geners,Keywords,Cast and Crew from dictionary form into list form and also edited out  all the unnecessary information from these columns and grouped together all the important information regarding every entry into a list and also converted the overview column into the list 
Combined all of them these 5 columns Geners,Keywords,Cast , Crew and Overview together to form tags 
# Model Building
After creating tags convert them into vectors through countvectorization in nltk library and then apply cosine similarity algorithm to detrmine the cosine distance between all the movies with each other and then comparing their cosine similarity distance with each other and then recommending movies based on their cosine simalarity distance with other movies 
