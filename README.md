## Website Performance Optimization portfolio project

#### Instructions to Run Website

In order to start the program running follow these instructions:
1. Download the repository.
2. Extract the folder.
3. Navigate into the folder in the terminal.
4. Type the following into the terminal:
    python -m SimpleHTTPServer 8080
5. Open a browser and visit localhost:8080 to view the page.

#### Steps Taken to Optimize
###### Index.html
1. I deferred loading of the print css in order to make unnecessary css load last.
2. I put the styles in style.css into the html as a <style> tag so that it would grab all the css in one round.
3. I made the API call to Google Analytics an async script in order to have it not block the rendering of the rest of the page.

###### Main.js
1. I read the scroll.body.top before the for-loop that utilizes the data in order to use it to write all the new values into items[i].style.left.
2. Inside the changePizzaSizes function, I assigned the dx and the newwidth properties in order to change the style in the actual for loop.
