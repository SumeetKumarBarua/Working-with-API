# Working-with-FactsBox-API
The project FactsBox (deployed on Heroku) exposes its data in the form of API. This README gives an insight about different API exposed and how to work with them.

To see the Live Demo of project <a href="https://factsbox.herokuapp.com/" target="_blank">Click here</a> 
<br>
To Learn more about the project <a href="https://github.com/SumeetKumarBarua/FactsBox-Heroku-Edition" target="_blank">Visit here</a>
<br>
<h3><b>FactsBox API</b></h3>

I wouldn't feel my app [FactsBox] to be complete if it doesn't have an API for you.
You can just request the JSON feed for all facts or some particular facts of your choice.
<br>
<br>
1. To get all the facts:
<pre> GET https://factsbox.herokuapp.com/api/FactAPI/allFacts </pre>
That will give the array something like this: 
<pre> [{"factId":1,"factCategory":"PHYSICS","factDesc":"BLACK HOLES ARE VERY DARK, BUT THEY GLOW, SLIGHTLY, GIVING OFF LIGHT ACROSS THE WHOLE SPECTRUM"},{"factId":2,"factCategory":"PHYSICS","factDesc":"IT IS ESTIMATED THAT SUN BURNS AROUND 620 MILLION METRIC TONS OF HYDROGEN PER SECOND INTO 616 MILLION METRIC TONS OF HELIUM."},{"factId":3,"factCategory":"PHYSICS","factDesc":"LIGHTNING STRIKES ABOUT 6,000 TIMES PER MINUTE ON OUR PLANET."}] </pre> 
<br>
2. To get a single fact based on ID:
<pre> GET https://factsbox.herokuapp.com/api/FactAPI/factId/10 </pre>
That will give the array something like this: 
<pre> [{"factCategory":"MATHS","factDesc":"ZERO IS THE ONLY NUMBER WHICH IS KNOWN WITH SO MANY NAMES INCLUDING NOUGHT, NAUGHT, NIL, ZILCH AND ZIP."}] </pre> 		
<br>
3. To get the list of categories:
<pre> GET https://factsbox.herokuapp.com/api/FactAPI/distinctCategory </pre>
That will give an array of distinct categories like:
<pre> ["BIOLOGY","CHEMISTRY","MATHS","PHYSICS","SCIENTIST","WWII"] </pre> 
<br>

4. To get a list of facts based on Category:
<pre>GET https://factsbox.herokuapp.com/api/FactAPI/category/PHYSICS</pre>
That will give the array something like this:
<pre> [{"factId":7,"factDesc":"THE HIGHEST TEMPERATURE EVER REACHED ON EARTH WAS 4 TRILLION DEGREES CELSIUS. THIS WAS IN QUARK-GLUON PLASMA AT BROOKHAVEN RHIC. "},{"factId":8,"factDesc":"THE YOUNGEST PERSON TO RECEIVE THE NOBEL PRIZE IN PHYSICS WAS WILLIAM L. BRAGG AT AGE 25. I WONDER IF HE BRAGGED ABOUT IT. "}]</pre>

