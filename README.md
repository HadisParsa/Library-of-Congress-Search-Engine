# <Library-of-Congress-Search-Engine>

# Library of Congress Search Tool

## Summery
This project is about an application that searches and displays results from the Library of Congress API.

## Built with

 HTML , CSS , JavaScript , Web APIs

## Instructions

This application has following criteria:

* User can submit a search query from the application to request data and receive a response from the Library of Congress.

* User can select a format in the form to help filter results.

* All of the results of my search displayed on a separate page.

* User can conduct additional searches from the results page as well.

To use this API, check out the Requests section of the [Library of Congress API documentation](https://libraryofcongress.github.io/data-exploration/).



## Link
You can experience the deployed project here: [Library of Congress Search Tool URL ](https://hadisparsa.github.io/Library-of-Congress-Search-Engine/).


### The Homepage

The homepage (`index.html`) have the following:

* A simple, well thought-out UI.

* A form with a text input field to capture a search query and an option select dropdown to capture the format of the search query. The options in the dropdown has a list of the possible format values listed in the [Library of Congress API documentation on requests](https://libraryofcongress.github.io/data-exploration/requests.html#format).

* A browser event listener attached to the form to execute a function on submission, which will capture both form values and redirect the user to a search results page with those values included in the URL as query parameters. This will use the browser's `location.replace()` method.

## The following demo shows the web application's appearance and functionality:

![The Homepage](./assets/images/ScreenShot1.jpg)


![The Homepage](./assets/images/ScreenShot2.jpg)

### The Search Results Page

The search results page (`search-results.html`) have and do the following:

* On page load, if there are query parameters, immediately parse them and use them in a request URL to fetch data from the Library of Congress API.

* If there is a value for the format query parameter, the format will endpoint to search for something based on the chosen format. For more information, see the [Library of Congress API documentation on the format endpoint](https://libraryofcongress.github.io/data-exploration/requests.html#format).

* If there is no value for the format query parameter, the search will endpoint to search for all types of data. For more information, see the [Library of Congress API documentation on the search endpoint](https://libraryofcongress.github.io/data-exploration/requests.html#search).

* The response from the API request will then be displayed on the page. For more information, see the [Library of Congress API documentation on responses](https://libraryofcongress.github.io/data-exploration/responses.html).


## The following demo shows the web application's appearance and functionality:

![The Search Results Page](./assets/images/ScreenShot3.jpg)
