# HW1-report.md

Quellas Lin 
Due: September 6, 2023
this is a change

## Git, GitHub

*What is the URL of the GitHub repo that you created in your personal account?*
<br>https://github.com/Quellas/CS625ODU

*In which direction does the 'pull' command work (send local changes to remote OR send remote changes to local)?*
<br><br>Send remote changes to local<br><br>
*If you have committed a change on your local machine, but do not see the update on GitHub.com, what step might have you forgotten?*
<br><br>The push step is forgotten if we can not see the update on Github.<br>
## Markdown

*Create a bulleted list with at least 3 items*
<ul>
    <li>First item</li>
    <li>Second item</li>
    <li>Third item</li>
    <li>Fourth item</li>
</ul>

*Write a single paragraph that demonstrates the use of italics, bold, bold italics, code, and includes a link. The paragraph does not have to make sense.*
<br><br>This is <strong>bold text </strong> , This is <em>Italicized text</em>, This is <em><strong>bold italics</strong></em><br><br> This is java code sample:<br><br>
```java
//This is a comment

public class HelloWorld{

   public static void main(String[] args){

      System.out.println("hello world");

   }

}
```
This is a link : www.google.com<br><br>
*Create a level 3 heading*
### This is a Level 3 Heading
*Insert an image of an animal, sized appropriately*
<br>
<img src="https://github.com/Quellas/CS625ODU/blob/main/mydogSage.jpg" alt="alt text" width="250" height="300">


## Tableau

*Insert your the image of your final bar chart here. Reminder, this should show data from a region other than the South.*
<img src="https://github.com/Quellas/CS625ODU/blob/main/SalesIntheEast-Quellas.jpg" alt="alt text" width="800" height="600">
## Google Colab

*What is the URL of your Google Colab notebook?*
<br>https://colab.research.google.com/drive/1lNOkPkRMErzlCq0kigax66CVXj7497yK?usp=sharing

## Python/Seaborn

*Insert the first penguin chart here*
<img src="https://github.com/Quellas/CS625ODU/blob/main/penguinplot1.png" alt="alt text" width="800" height="600"><br>
*Describe what the figure is showing.*
<p>This plot illustrates the distribution and quantity of penguins based on their bill length and bill depth. Within the plot, three intervals stand out where a higher number of penguins are concentrated. The first interval ranges from a bill length of 35 to 42.5 mm and a bill depth of 16 to 20 mm. The second interval falls between a bill length of 42.5 to 50 mm and a bill depth of 13 to 16.2 mm. The third interval spans a bill length of 50 to 53 mm and a bill depth of 18 to 20 mm.</p>
*Insert the second penguin chart here*
<img src="https://github.com/Quellas/CS625ODU/blob/main/penguinplot2.png" alt="alt text" width="800" height="600"><br>
*Describe what the figure is showing.*
<br><br><p>This plot illustrates the distribution of penguins by species and their respective quantities. The species with the highest count is the Gentoo species, while the Adelie and Chinstrap species have nearly equal numbers, with Chinstrap slightly outnumbering Adelie.</p>
*What happened when you removed the outer parentheses from the code? Why?*
<br><br><p>The code raised a syntax error. Because the parentheses are necessary to properly group the operations performed on the Seaborn Plot object.</p>

## Observable and Vega-Lite

*What happens when you replace `markCircle()` with `markSquare()`?*
<p>The points on the plot have changed from solid circles to solid squares.</p>

*What happens when you replace `markCircle()` with `markPoint()`?*

<p>The points on the plot have changed from solid circles to hollow circles.</p>

*What change do you need to make to swap the x and y axes on the scatterplot?*
<br><br>Just switch the encoding for x and y :
```javascript
vl.markSquare()                        // Make a scatter chart
  .data(cars)                          // Using the cars data (below)
  .encode(
     vl.x().fieldQ("Miles_per_Gallon"), // For x, use the Miles_per_Gallon field
    vl.y().fieldQ("Horsepower"),       // For y, use the Horsepower field
    vl.tooltip().fieldN("Name")        // For tooltips, show the Name field
  )
  .render()                            // Draw the chart
```

*Insert the bar chart image here*

<img src="https://github.com/Quellas/CS625ODU/blob/main/CountOfRecords.png" alt="alt text" ><br>
*Why do you think this chart is the result of this code change?*
<p>Because commenting out the line `vl.y().fieldN("Origin")` removes the distribution of data based on the category of the country of origin.</p>
## References

*Every report must list the references (including the URL) that you consulted while completing the assignment. Replace the items below with the references you consulted*

* Reference 1, <https://seaborn.pydata.org/>
* Reference 2, <https://www.pythonmorsels.com/breaking-long-lines-code-python/?watch/>
