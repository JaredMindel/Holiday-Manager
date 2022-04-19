# Holiday-Manager ReadMe

---

## Importing Libraries

Truth be told, only a few of these are absolutely necessary, but some of those libraries are there for the sake of future editing.

Primarily, we need to use the datetime library, the json library, the bs4 library, and the requests library. The others aren't as important, but in future editions they may be of value.

## Holiday Class

Alright, so this is where we begin. The Holiday class is effectively the object that we want to be using throughout this entire program. The Holiday class is the bread 
and butter of our operation. To create a holiday, we need the name and date of the holiday. It's important that the date be set in the following format: yyyy-mm-dd; if the date is not set this way, it will not work. To add this in our main run - which we'll get to later - we'll use the addHoliday function. 

## HolidayList

This is the large, library class in our program. We want to take many objects of the Holiday class and put them into a library. The library itself has it's primary list, 
the innerHolidays list, which is very important for tracking the holidays; it will serve as the list that holds the various holidays, which are formatted as dictionaries there.

## Main Run

This is where the magic happens. The main run is really the testing sight, where we run the entire program. The menu will appear and ask the user what they want to do, and they have 12 options:

  1. Add a holiday
  2. Remove a holiday
  3. Count the holidays
  4. View the holidays
  5. Scrape holidays from online
  6. Get the Weather for the current week
  7. Read in a json file with holidays
  8. Save the holidays as a json file
  9. View the current week
  10. See each holiday and what week it's in
  11. Exit the program
  12. Go back to the main menu

Let's go through each option:

  1. Add a holiday: To add a holiday, give a holiday name and the date in the following format: name, yyyy-mm-dd; note that in between the name and the date, there is a          comma and a space. It won't work if not used correctly. 
  2. Remove a holiday: To remove a holiday, use the same format as when adding a holiday, but now the holiday will be removed.
  3. Count the holidays: This is simple; it just counts the total amount of items in the innerHolidays list and returns that value as an integer.
  4. View holidays: This will show the holidays in total alongside their date.
  5. Grab holidays from online: This is effectively the scraper; this one should be used before anything, but it's not absolutely necessary. 
  6. Get the Weather for the current week. Unfortunately this one doesn't work anymore because the API won't let me run it with this API key, but it used to work very well.      The API website is (WeatherAPI.com) and the rapidAPI website for this API is (https://rapidapi.com/weatherapi/api/weatherapi-com/). 
  7. Read a json file: This command lets you read in an API file with holidays. Simply give the file name - without the json file type at the end - and it'll work. Of          course, this file has to be in the same folder as the program itself and needs to be in json. 
  8. Save the file: Basically this saves the innerHolidays list as Holiday_List_Output.json. No inputs required!
  9. View the current week: This will let you view the current week; it will ask if you want to see the weather, but unfortunately that doesn't work.
  10. View the holidays in a week: this shows each holiday and what week it is in, given a week between 1 and 53 (this is odd, yes, but this is how these dates work.             Sometimes the week will carry over into what we consider to be the next year). The user is prompted for a week number and a year between 2020 and 2024, and it will         print any holidays that fall in that range in the United States.
  11. Exit. If the user has not saved the file, it will ask if they want to leave with a warning that the file is unsaved. If the file is saved, that warning won't appear,       but they'll still be asked if they want to leave. 
  12. See the main menu again. This should be self-explanatory.
