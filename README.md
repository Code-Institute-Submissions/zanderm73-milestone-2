# Glasgow Treasures

The purpose of the project is to allow people that are currently in Glasgow or people who are looking to visit to be able to find attractions and
things to do when they in the area. It is designed in a way that they can interact with the website and leave comments and recommendations for other
people to try when they are visiting Glasgow. We have also gave a few of what we think the best places in Glasgow are to visit to help people get 
started when organising their days.

The thing that makes the website different from others is the way that users go about finding locations. For example there is not a tab or link that 
will show all of the bars in the area although this can be done using the search bar in the Google Maps API. Users have to find places either using 
the search bar, following our recommendations or trusting others that have visited the site and left their own recommendation.

## UX

The project is essentially a single page application that allows users to search, find and recommend things to do within the Glasgow area. With our
recommendations, users recommendations and the search bar within the Google Maps API we are able to create a page that users will want to hunt for 
the best places to visit, hence the name Glasgow treasures.

The single page application has been designed on a mobile first approach but is fully responsive. This has been achieved by using Bootstrap in the 
design. Due to the nature of the application users will navigate the site in a number of different of ways, below are a few examples;
- User 1 is currently in Glasgow and has decided to try one of our recommended restaurants Yiamas but doesn’t know where it is. They are then able to 
  type Yiamas into the Google Maps search bar and the restaurant will appear in the search results. Once selected the restaurant location will be 
  highlighted on the map by a fork and knife symbol
- User 2 will be visiting Glasgow at the weekend with friends but has not been to the area before. They are looking to find out where the bars are in 
  and around Glasgow. They then use the Google Maps search bar by typing in ‘bars’. All bars in the Glasgow area are then highlighted by a martini glass
  symbol
- User 3 is a Glasgow local and knows the area but is looking for somewhere new to try as they always go to the same place. They check other peoples 
  recommendations on Glasgow Treasures. They see Jamies Italian has been mentioned as being very good. They know where the restaurant and decide to try
  it

## Features

	Existing Features
- The Google Maps API search bar allows users to search for specific places around Glasgow and also more generic terms can be used such as ‘Chinese 
  restaurants’. These will then be highlighted with a symbol appropriate to the establishment for example martini glass symbol for a bar
- The comments section allows users to leave feedback on places that they have visited in Glasgow and would like to share with other people. This same
  feature also allows users new to Glasgow to quickly find recommendations from people who have already been
- Social media links within the footer allow the user to experience Glasgow on a number of media platforms to give them a more in depth of Glasgow prior
  to visiting

	Future Features
- Create a way of reading reviews for the places that are searched for within the application so they do not have to leave the site
- Set up affiliate links that allows local business owners in Glasgow to offer special discounts exclusive to Glasgow Treasures on the page for the users
  to benefit from when visiting

Technologies Used
For this singles page application there was a number of programming languages, frameworks and libraries that were used. These are stated below with an 
explanation as to why they were used;
- HTML - The markup language was used as the building blocks allowing us to create the rest of the application
- CSS - This was used to style the website making the HTML more appealing to the user
- Javascript - This was used to allow the browser to display the interactive google maps API with a number of functions. Javascript was also used to
  allow the comment section to be interactive (https://www.javascript.com)

- Bootstrap - The framework was used to allow the layout of the application to be responsive depending on the users device. Bootstrap was also used to 
  display the social media icons. (http://getbootstrap.com/).

- jQuery - This was used to manipulate the DOM and reduce the amount if code required, shortening the development time (https://jquery.com/)

- Google APIs - This was used as a means of displaying a map and interactively search for locations 
                (https://developers.google.com/maps/documentation/javascript/)
- Htmlcommentbox - This was used as a means of allowing the user to interact with the application and other users (https://www.htmlcommentbox.com/)

## Testing

1. Accessing and navigating the site
    1. Accessing the site on different browsers to make sure that it works. This has been tested on chrome, safari and internet explorer browsers
    2. Scrolling up and down the site on both desktop and mobile to make sure that it works on different devices. This has been tested on a MacBook, 
       iPad and Galaxy Samsung S9+

2. Finding a location using the search bar
    1. Searching for one of our recommended locations by typing in Miller & Carter into the search box
    2. Selecting the correct location on the drop down list, the geolocation function worked as it showed the Miller & Carter restaurant in the centre
       of Glasgow rather than the one just outside or the Edinburgh restaurant 
    3. Crosschecking with the google maps page that the location highlighted with a knife and fork was in-fact the correct restaurant
3. Posting a comment in the hidden treasures section
    1. Posted a recommendation under the name of Jamie Oliver stating that Jamies Italian on George square served good food
    2. Refreshed the browser to make sure that t the comment was still there. 
    3. Opened an incognito tab and visited the application to see that the comment was still there
4. Visiting the social media links
    1. Visited the linked Facebook, Instagram and Youtube social media links on several devices and browsers to make sure that they were accessble 
       across devices and browsers. 
    2. Making sure that on all devices a new tab is opened to display the links as the sites are external to website and do not have links back to the
       Glasgow Treasures application

While creating the single page application there was a few problems where the solution had to be researched. Embedding the Google Maps API into the
application and having it be responsive and appealing at the same time was difficult. The way that the code was initially written led to the maps API
window unable to scale when using anything with a lower pixel width than desktop which led to the maps sticking out of the application width. Multiple
solutions were looked at to try and fix this problem, one of them was implemented but it resulted in the maps window only having 50% width when viewing
on desktop and it did not suit the design of the overall website. A solution was eventually found by inserting the Map API into its own container div.
Another problem with the Map API was that it was only loading 50% of the time. When inspecting this in Google Chrome there was an error message stating
that the function was not defined but then the page could be refreshed and it would work. This was solved by changing the order that the scripts we 
placed in on the index page.

Another issue was trying to make the ‘our treasures and ‘comment box’ columns equal in height at all times. The fact that they had different background
colors emphasised the difference. Many of the solutions that were tried after searching online did not work, I am still unsure if Bootstrap was 
overriding the attempted solutions that were implemented. This problem was resolved by inserting a media query declaring the comment box column had a 
minimum height of 630px while viewing on any device higher than 768px. 

## Deployment

This project has been hosted on GitHub Pages. This site was deployed after using GitHub as a code repository.

## Credits

The image (glasgow.jpg) in the header was taken from https://www.digitalimpact.co.uk/seo-guide-for-glasgow/
The maps Api and some of the functions were taken from https://developers.google.com/maps/documentation/javascript/
The hidden treasures comment box script was taken from https://www.htmlcommentbox.com/

## Acknowledgements

The inspiration for this application was taken from the city of Glasgow itself
The inspiration for the structure of the website was taken from previous work that I have done with Code Institute 



