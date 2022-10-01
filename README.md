# Flight-Delay

Anyone who has ever booked a flight ticket knows how unexpectedly the flight timing varies. Airlines use sophisticated tactics which they call "yield management".

According to a recent study, India is currently the 3rd largest civil aviation market in the world. According to IATA (International Air Transport Association) the number of flyers globally could double to 8.2 billion in 2037. 

Nowadays, in this ever advancing world time management has become a prominent factor in all business operations. We can’t afford to lose time on unnecessary delays. Using this as motivation we have developed a ML Model which predicts arrival flight delay based on various factors that include airport score, general airline trend, air traffic etc.


# Data Collection and Cleaning:

Collection of data from flightradar24.com by                                      web scraping using python package BeautifulSoup which parsing HTML and XML documents.
Overall 23 features collected were collected from the website
Weather features were also extracted in a similar way using Beautiful Soup, 21 weather features were extracted 
After categorical encoding, imputation of missing values and remove of rows with many null values, final dataset obtained had 10313 rows and 44 columns.
 
# Data Pre-processing and Model Application:

Removal of the Departure Delay feature it caused Data Leakage
Outlier Removal: We considered only delays from 3 hrs early to 3 hrs late.
Normalized the target variable so that our model generalises well in real life.
Applied Interaction features which allowed us to capture better insights about the data.
Careful feature selection based on their importance. This allowed the model to improve its performance as well as reduce training time.
Started with basic linear models but they performed poorly, hence shifted to tree based ensemble models, they performed much better than better prediction were obtained.
The evaluation metric used was Mean Squared Error,  
Finally inverse transform was applied to target variable to show predicted delays.


       
      

