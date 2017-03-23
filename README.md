# Working-with-FactsBox-API
The project FactsBox (deployed on Heroku) exposes its data in the form of API. This README gives an insight about different API exposed and how to work with them.

To see the Live Demo of project <a href="https://factsbox.herokuapp.com/" target="_blank">Click here</a> <br>
To Learn more about the project <a href="https://github.com/SumeetKumarBarua/FactsBox-Heroku-Edition" target="_blank">Visit here</a>
<br>
<h3><b>FactsBox API</b></h3>

I wouldn't feel my app [FactsBox] to be complete if it doesn't have an API for you.

You can just request the JSON feed for all facts or some particular facts of your choice.

To get all the facts:
<pre>      GET http://quotes.stormconsultancy.co.uk/quotes.json</pre>

  https://factsbox.herokuapp.com/api/FactAPI/allFacts
	 That will give the array something like this:
	 **************

To get a single fact based on ID:
  https://factsbox.herokuapp.com/api/FactAPI/factId/1001
	That will give the array something like this:
	 ***********	

To get the list of categories:
  https://factsbox.herokuapp.com/api/FactAPI/distinctCategory
 That will give an array of distinct categories like:
 ["BIOLOGY","CHEMISTRY","MATHS","PHYSICS","SCIENTIST","WWII"]
 

To get a list of facts based on Category:
  https://factsbox.herokuapp.com/api/FactAPI/category/PHYSICS
  	That will give the array something like this:
	 ***********

