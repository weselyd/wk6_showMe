# weather-dashboard v2.0

This web application takes input from the user in the form of a city, then calls OpenWeatherMap APIs to determine which city they are expecting and returns current weather data.  Once the weather data is displayed, there is a second button that inititates a call to OpenAI to get advice on what to wear based on the current weather.

The project's files are broken out into ES6 modules:
 - app.js: imports all necessary functionality from other modules and orchestrates all operations
 - api.js: handles API calls to OpenWeatherMap
 - ai.js: handles the API call to OpenAI
 - ui.js: performs ui updates (loading indicators, errors, display of data)
 - events.js: implements event listeners for buttons and initiates actions behind them
 - index.html: core HTML markup
 - styles.css: core styling

 To deploy this app, just clone the repo and store in root directory of webserver.  Once you have that you'll need to add your API keys, one for OpenWeatherMap (stored in api.js) and the other for OpenAI (stored in ai.js).  All there is left to do then is to start the server and open index.html.


# Week 5 Modernize Your Web App with AI & Advanced UI Techniques

This latest version of the application is functionally the same but has been significantly improved styling.  This was done using GitHub Copilot and manual changes to fine tune the desired look.  

Copilot was first prompted to change all CSS to use only Tailwind CSS classes which it did but it also changed the styling in other unexpected ways.  With a few more prompts I got it to where the page was a cleaner look better suited to common weather web sites but had to makes some manual changes when it came to specific colors, text sizing, and font selections.  Next, I added the GSAP animations and during that process I used Copilot to give some ideas about what type of animations were possible while keeping with only using GSAP and Tailwind.  