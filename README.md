In this exercise, you will be automating the process of entering search text and verifying the presence of certain elements after they are loaded.

### Prerequisites

- Install IntelliJ IDEA Community IDE  Version 2018.3.6.
- Install OpenJDK 11 and complete the configuration.
- Install a Browser Driver(Chrome Driver).
- Setup a Selenium project with the name `WikiSearchTest`.

You can refer to this [Reading Material](https://learning.ccbp.in/qa-automation-testing/course?c_id=cf952b35-27ab-4b1e-a6de-44227f22806c&s_id=f5c19277-3889-4e63-b631-c06c088d612c&t_id=6a935df7-2c93-477c-b505-3ae0aabcf9a2#31-installing-ide) to complete the above prerequisites.

### Steps to Automate

- Create a driver instance using WebDriver interface.
- Navigate to the url `https://qawikisearch.ccbp.tech/`
- Find the input field with id `searchInput`- _use (Relative) XPath Locator_.
- Enter the text `HTML` in the input field.
- Find the 'Search' with class name `search-button`- _use (Relative) XPath Locator_.
- Click the button - _use `click()` method_.
- Wait for a maximum of 10 seconds for the search results to be loaded.

    - Wait until the search results (`<div>` elements) with class name `result-item` are loaded,
    	- _use `visibilityOfElementLocated()` method_
    	- _use (Relative) XPath Locator_
- Find all the search results with class name `result-item`- _use (Relative) XPath Locator_.
- Print "<result count> Results Found"
	
	- For example: `3 Results Found`
- Close the browser window.

<br>
<br>

**Note: Set up the project and practice this exercise in your local IDE(IntelliJ).**
