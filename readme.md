This project provides a simple web application that allows users to search for National Registration Card (NRC) information based on NRC code, NRC name, or city name. The application retrieves data specific to Myanmar NRC from a JSON file and dynamically updates the search results based on the user's input.


## **Data**

The provided data in the `data.json` file represents Myanmar NRC information. Here is an example structure of the JSON data:

```
{
  "data": [
    {
      "name_mm": "(အဂယ)",
      "nrc_code": "1",
      "city_name": "အင်ဂျန်းယန်"
    },
    {
      "name_mm": "(ဗမန)",
      "nrc_code": "1",
      "city_name": "ဗန်းမော်"
    },
    ...
  ]
}
```


The `data` array contains objects representing individual NRC entries. Each entry consists of the following properties:



* `name_mm`: The NRC name written in Myanmar language, enclosed in parentheses.
* `nrc_code`: The NRC code.
* `city_name`: The name of the city associated with the NRC.


## **Usage**

To use the NRC Code Search application, follow these steps:



1. Clone or download the project files to your local machine.
2. Open the `index.html` file in a web browser.
3. Enter the NRC code, NRC name, or city name in the search input field.
4. As you type, the application will filter the data and display the matching results in a scrollable table.
5. The table will show the NRC code, NRC name, and city name for each matching entry.
6. If no matching entry is found, a message will be displayed indicating that no results were found.
7. You can continue to refine your search by modifying the input in the search field.


## **Code Overview**

The project consists of two main files: `script.js` and `index.html`. Here is an overview of the code:


### **script.js**

The `script.js` file contains the JavaScript code that handles the search functionality and data retrieval. The main functions are:



* `searchNRC()`: This function is called whenever the user inputs text in the search field. It retrieves the input value, fetches the data from the `data.json` file, filters the entries based on the input, and dynamically updates the search results.
* `extractTextWithinParentheses(text)`: This helper function extracts the text within parentheses from a given string. It is used to extract the NRC name from the data entries, which are stored in parentheses.


### **index.html**

The `index.html` file provides the structure and layout for the web page. It includes an input field for the user to enter their search query and a div element to display the search results. The relevant JavaScript file (`script.js`) is imported at the end of the body section.


## **Styling**

The project includes a separate CSS file (`style.css`) for styling the web page. You can customize the styling in this file to suit your preferences.

Please note that the provided code and data are specific to Myanmar NRC and may not be applicable for other countries' identification systems.
