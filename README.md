# UFOs
Objectives

The goals of this challenge are to:
    create, update, and deploy JavaScript functions to provide additional table filters.
    Update and deploy forEach (for loop) to loop through the filters and update them with user input.
    Update and populate the dynamic filters and table using JavaScript and HTML.
Resources
    JavaScript
    html
    css

Analysis

I started by adding list items for the filters that were required (city, state, country, shape). These were added to the unordered list section in the .html file that already held the user input area for the date filter we developed in the module. Once this was completed, I built the Javascript code to grab the user input from these items and append a JS object (named "filters"). The .toLowerCase() method was useful to make sure the user input was in the correct state to match up the filters. I then found code on Stack Overflow1 that helped me remove the keys and values from the object if the user did not enter data into that field (i.e. empty value). Once we have this clean object, we can loop through it by converting the object to an array (in this case an array of key/value pair arrays) to build the filtered data. We then return to the buildTable function where we pass the filteredData as the parameter. I have also added a clear filters button and function that simply reloads the page since our default is the complete table (i.e. no filters). As a recommended action, we could improve data accuracy by creating dropdown lists for the user to choose from, but the placeholder does a pretty nice job of directing the user to the correct format for data entry.
![Website screenshot](https://user-images.githubusercontent.com/92246505/153174460-ba541ce4-d81e-4934-9fdd-77785e90b3f3.png)




Summary
Drawback
One draw back is the absence of a prompt from the filters during a search. The list of sightings we have in the data is not exhuastive, therefore some of the search criteria do not brinng up any information. However, there is no prompt in the search box to show that a search criteria has not information to show from the table. The user might be unawre and there's a chance they might think the filters don't work.
Recommendations:
Include a code to show a message prompt in the filter box when there's not information for a search criteria will surely enhance user experience.
A popup to show the number for each search result will also enhance user experince.
