# pq-challenge-star-wars

In this challenge you will create a simple website displaying a datatable list of Star Wars characters allowing you to click on each character name which will navigate you to another page where detailed biographical information on the selected character is presented.

The time allowed for this project is **36 hours**, upon delivery of the Challenge scope to the candidate. 

If you wish to have more time, please send an email to [hartley@palqee.com](hartley@palqee.com) detailing the reason, what is missing, as well as your current progress in the form of a repository link or zip file of the project.

## Requirements

-	This must be built on NextJS
-	The endpoint you will use to get the character information is a GraphQL endpoint, and as the client you must use Apollo Client
-	For styling no frameworks or libraries can be used to bootstrap, just CSS-in-JS and from scratch CSS. Note: You can use libraries for CSS-in-JS like @emotion
-	Only use React Hooks for state management
-	You will be required to use Typescript

## Definition of Done

The following is a list of features and requirements that will mark the challenge as completed or Done 

1.	Website must load without errors when running locally. Note: If you wish you can deploy this using Vercel, Heroku, Netlify or whatever platform you prefer. This is however not required as long as the site can be run locally.
2.	Built on NextJS using Apollo Client. This can be statically built, SSG, or server side rendered SSR. You can also use any start boilerplates as long as they do not contain any libraries or tools that is not part of the requirements list.
3.	User be able to use the navigation menu to go to the Star Wars – Characters page
4.	The data table must have sorting, filtering and pagination all working as expected
5.	The Star War description quotes must provide a new quote on each page refresh or navigation
6.	Clicking on a specific Star War characters from the Datatable will navigate the user to the Individual Character Page with all of the required information.
7.	The cards gallery must be responsive stacking as required based on page size.

Aside from these requirements above any other frameworks, libraries, or tools you see fit are fair game

## Resources

- Rest API endpoint for random quoest API: [https://wolfgang-ziegler.com/blog/starwars-quotes-web-api](https://wolfgang-ziegler.com/blog/starwars-quotes-web-api) | [http://swquotesapi.digitaljedi.dk/api/SWQuote/RandomStarWarsQuote](http://swquotesapi.digitaljedi.dk/api/SWQuote/RandomStarWarsQuote)
- GraphQL endpoint for Star wars api: [https://graphql.org/swapi-graphql](https://graphql.org/swapi-graphql). If this does not work you can use the following [https://github.com/graphql/swapi-graphql](https://github.com/graphql/swapi-graphql) to setup a local server instance to be run with the frontend

## Layout

Site will maintain a 2-column page layout (dashboard feel).  That will consist of:

*	Sidebar (column 1): Here you will create an accordion like Navigation which for this challenge will have 2 menu items
  *	Menu Item 1: Home
    * This will link does not need to work, or if you wish it can take them to a blank home page
  *	Menu Item 2: Star Wars
    * This item will have a submenu item called Characters
*	Main Area (column 2)
  *	This will be comprised of 2 main parts
    *	Header
      *	The header will just have today’s date 
    *	Section
      *	This is the main section which will render the content passed on each page

**Note**: The sidebar and header will remain consistent on each page

## Pages

The site will consist of 2 main pages:

### Characters List page

On this page in the main section area, you will implement the following:

1.	Breadcrumb of the page and subpage
2.	Section Title – This will hold the value of Characters
3.	Section Description 
  * This will contain display various Star Wards quotes on each page refresh
  *	API: https://wolfgang-ziegler.com/blog/starwars-quotes-web-api  
    *	Alternatively you can use any public free Quote API available which you prefer
4.	A Data Table 

The main of this page will be the data table component. Here you will provide the list of Star Wars characters available using this GraphQL API [https://graphql.org/swapi-graphql](https://graphql.org/swapi-graphql) . You can also use the following [https://github.com/graphql/swapi-graphql](https://github.com/graphql/swapi-graphql) to setup a local server instance to be run with the frontend.

The table will have the following Columns

*	Name
*	Hair Color 
*	Skin Color
*	Eye Color
*	Gender
*	Home world Name

The name will be a clickable link navigating the user to the Individual Character Page. The table will also have the following features

*	Sorting. All columns
*	Filtering. Only the following columns will allow filtering
  *	Hair Color
  *	Eye Color
  *	Home world Name
*	Pagination
  *	Max Items Per Page: 5
    *	This can be adjusted to 10 or 20

**Note**:

*	Design of the table is not important as long as the functionality works, and it is clean
*	You only need to support Tablets and Desktop devices as Responsive design. This does not need to be perfect

### Individual Character page 

Detailed view of selected Star Wars character

Here you will provide the following

1.	Breadcrumb of the page and subpage
2.	Section Title – Name of the selected Character
3.	Section Description 
  *	This will contain display various Star Wards quotes on each page refresh
  *	API: https://wolfgang-ziegler.com/blog/starwars-quotes-web-api  
4.	A list of cards related to the films the Character is a part of
  *	The card will be responsive and contain the following information. Note: The layout and design of the card and the contents of the card is up to you however it should be a gallery of cards displaying the list of films and related content inside.
    *	Title
    *	Episode
    *	Director
    *	Producer
    *	Release Date


## General Notes 

-	Again great, perfect design / UI is not required but is accepted should the time allow. You will not be able to use any CSS frameworks like Bootstrap, Tailwind, Foundation, etc. All CSS layouts, designs and implementations must be done from scratch this is why amazing design is not necessary, but gladly welcomed.
-	All of the 7 items in the Definition of Done will be graded
-	There is no exact or perfect way of implementing the challenge. The purpose here is to test you on various React techniques, and implementations, as well as NextJS and Apollo Client experience.
-	Any conventions you wish to implement are acceptable 
-	Any additional tools, plugins, rules you wish to implement in the project are acceptable as you see fit
