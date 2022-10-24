# UFO Sightings

## Overview
In this project we used JavaScript, HTML, and Bootstrap to create a website that enables users to filter data about UFO sightings by date, city, state, country, and shape. 

## Results
Users can filter the site by the 5 parameters defined above. To do this, we first needed to build our filters table into our HTML document. ![HTML](https://github.com/nicole-tough/UFO/blob/main/Report%20Images/HTML%20Filter%20Table.PNG) In our code, each filter element needed to be included in the list. Now that users were able to access the filters in the filter table, it was time to add functionality to our site. We had to write a function that would filter the dataset and return the correct information based on user input. Within our function, we defined variables to save the user's input, save the input value, and save the input ID. Then, we wrote an if-else statement to apply the filter value. If no filter value was assigned, then the filter was cleared.  
![updateFilters](https://github.com/nicole-tough/UFO/blob/main/Report%20Images/updateFilters.PNG)
After the filter values were applied to data, we wrote a function that would loop through the data to build the table with the correct values. ![filterTable](https://github.com/nicole-tough/UFO/blob/main/Report%20Images/filterTable.PNG) 

Finally, we needed our site to responsive to the user's input. To do that, we used D3 to listen for all user input into the filter search table. Once input is received, our site is set to start filtering the data. ![event](https://github.com/nicole-tough/UFO/blob/main/Report%20Images/Event.PNG) 

In the example below, you can see the interface of the site and the results of a search for UFO sightings on January 10th, 2010. ![Example](https://github.com/nicole-tough/UFO/blob/main/Report%20Images/Example.PNG)

## Summary
### Drawbacks
One drawback of this new design is the lack of a button. Users will need to know that once they have entered their search criteria, they will need to either press enter or click outside of the filter table for their results to load. As many webpages with search options incorporate a button for users to click to initiate their search, this may be confusing to some users. 

### Recommendations
For further development, we recommend adding a filter for the duration of the UFO sightings. However, in order to do this, the data in the duration column would need to be formatted more homogenously. After being formatted, the duration times could be banded into spans of time depending on the spread of the data points. Then, for example, users could filter the data and find UFO sightings that were less than 1 minute long. 

We also recommend adding more data points to the site. While there are many UFO sightings documented on our current site, it would be more convincing if there were more sightings, especially more recent sightings. 
