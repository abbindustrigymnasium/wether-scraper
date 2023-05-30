# Weather Scraper
This project scrapes temperature from two different websites and compares them side by side for the user to see if they agree with each other and therefore can trust the weather forecast. It specificaly scrapes the temperatures from any city in Sweden.

# Setup
<ol>
 <li>Clone the repository</li>
 <li>Run "npm install" in the main porject folder to install all dependencies required</li>
 <li>Enter the "server" folder and open it's terminal. In the terminal run "npm start" to start the server</li>
  <li>In the main project folder enter the "website" folder and open it's terminal. In the terminal run "quasar dev" to start the website</li>
   <li>You will be redirected to the website and when that happens you can start to use the application. Just type in any swedish city in the search bar and wait for the data to be scraped</li>
 </ol>
 
 # Bugs
 <ul> 
 <li>Loading Time - The program that scrapes from smhi.se is bugged and works fine sometimes while it dosen't work at all other times. The code automatically re-runs the program if the data that is being sent back is empty and it therfore the loading time can sometimes be longer than other.</li>
 <li>No data - The application scrapes a 10-14 day weather forecast and both websites being scraped start to update the temperature on a different TIME scale meaning that the data for the 4th day is only being recorded during hours 00:00, 04:00, 12:00 and 16:00 from the klart.se website while on the smhi.se website the data is being recorded in the hours 00:00, 05:00, 09:00 and 14:00. This makes the data not properly alligned on the website and results in no temperature being shown on the klart.se side.</li>
 <li>Server not working - The server dosen't work properly unless you start it in the terminal using "npm start". It dosen't work if you try to start it in visual studio code</li>
</ul>
