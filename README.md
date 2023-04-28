*Chat GTP created webpage report: 

Chat GTP, at first glance, seems to be an incredibly simple way to generate a webpage without any experience or knowledge of manual coding in HTML or CSS. With basic instructions (create a 1-page website using HTML and CSS about home brew) a very simple web page was created. Additional elements could be requested (create a footer, create a hero image), however the more complicated and in depth the additional requests became, the more difficult it was to implement them into the page code. It very quickly became apparent that at least a fundamental understanding of HTML and CSS would be required to create an interesting, fully functional web site with much more than the most basic functionality. It also requires a very good understanding of what and how to request different elements of the page from the system, some of the responses from Chat GTP around specific elements could easily confuse users with no experience or understanding of coding fundamentals. 

There were a number of interesting quirks I found when making requests from the system. Some examples are: 

-Code truncation - when code becomes significantly long, the system would stop generating at random points. I could not reliably replicate this issue (without a lot more testing), so I'm not sure if this is an underlying system issue, or something to do with infrastructure. Whatever the case it is still worth noting. My workaround for this was to request code be generated from a point before it was truncated (generate code from class XXX for example). It was then a case of copying the code to the correct area in VS code. 

-Class naming - The system also seems to drift away from its own defined class names the more requests are made about the same page. By example, a class .column__left may shift in later requests to just .left or .grid__left. The result of this was several errors and inconsistencies if you just copied and replaced code without checking or understanding how HTML calls CSS code. This may pose a hurdle for users with no experience in coding, or if you miss the changes, but it was simple to correct with a good understanding of the coding principles. 

-being specific about what you request - Chat GTP seems to only take a broad guess approach if you are not specific in your requests. By example, asking for a footer initially resulted in a single line with the web page, which while technically correct, was not what I was after. A more thorough request; create a footer with sitemap and email subscribe function, resulted in a much more interesting and modern result. The learning curve for getting the requests right was not hard, but good to keep in mind. This also indicates you would need to have a very good understanding of what you wanted from the page (lo-fi prototypes would significantly help here). 

  

** Things Chat GTP did well: 

It was incredibly easy to get started on a website using the system. The most basic functions could be created instantly without the need to cut a single line of code. 

For my topic, homebrewing, it generated some really interesting content about the hobby out of the box. This helped to get a sense of page layout and content immediately, which allows users to focus on content and coding as 2 separate, discrete jobs. 

Adding elements, when requested with enough specificity, was also a relatively easy task, however the more complex the requests, the more coding knowledge was required. I did make a few requests about "where in my code do I add this element" which occasionally returned good results, but sometimes steered me down an incorrect path. I believe the system does not maintain a good track of where the code is up to and what has previously been written. 

I did use the system to review my code as well, at several points I added the complete code package (as copy and paste) to the system and requested it clean up the code. The changes were minor, but it did seem to pick up areas where code was repeated, or out of order. This was a handy function to check code after a number of complex additions were made. 

The system would also offer different approaches if one method didn't work. For example, trying to center text did not work as required, making an additional request of "that didn't work..." and adding what didn't work (text is still right aligned) often resulted in a different approach to the problem. This included a more board approach, such as modifying more global settings or functions further up the code stack. This was a handy method to address issues, though if not careful, it could end with confusing, spaghetti code. This again reinforces the need for some level of HTML and CSS understanding. 

Chat GTP also offered great explanations as to what and why it did things. Explaining how it created code to add a hero image, for example, was good to increase coding experience and understanding. As a tool to help learn and grow experience in creating web pages, it could prove invaluable. 

**Overall thoughts: 

I think using Chat GTP as a starting point for new pages is a great idea. It can save a lot of repetitive coding and some of the complexity in creating a new page. It also does well in suggestion how to create and code new elements for the page. However, the more complex the requests you make are, the better understanding of HTML and CSS you will require. The way the system is set up, it could also be used as a teaching/learning tool to help increase coding knowledge and experience. I do feel that the more complexity that the page being created requires, the less value Chat GTP could offer at a fundamental level. The actual coding value it adds would run as diminishing returns, however the use case may shift to assist with troubleshooting or exploring different options for a solution. 

There is an incredible amount of value to be gleaned from Chat GTP as long as it is used well and with the understanding of its limitations. As it stands it would provide an additional tool for both new and experienced developers, but it is not yet at the point where coding experience is defunct. 

  

**Request lists: 

This is a sample list of the requests I made to the code. A full transcript will be added to the Git repository under the folder GTP Outputs. Please disregard the homebrew recipes i was requesting from the system. Export only seems to take the entire output. 

- build a one page website using html and css about homebrew beer

Result: Very, very simple page, but still clean and efficient. Much easier than coding from scratch. The images however had broken links, but a second request to fix this did not work. Response was:
I apologize for that. As a language model, I don't have control over external images and their links, so I used a random image from Unsplash for the sake of example. Here's an updated code with the image link updated to a different image:
The CSS coded was embedded in the HTML as a <style> element. I will request this be split into a CSS file in future iterations.

The actual information sourced for the content was actually really useful and informative about the hobby. 

- can you add colums to the page to make it more visually interesting
I asked it to add columns to make the page more visually appealing. 2 colums were added quickly, but it still remained a very basic page. Images were still not loading.
The footer has also been dropped.
It actually looks like sections of the code have been dropped froom the response. Regenerating code to see if this adds the required elements.

- can you add a subscribe button to the footer
There seems to be a limit on the length of this request. I requested the code be split into styles.CSS and index.HTML files. This worked well and allowed separation of the CSS and HTML.

- can you please split the code into a styles.css file and an index.html file
There is a limit on the response length from the system. The Index.html was fine, but the Styles.CSS truncated after a couple of lines, as shown below:.
/* CSS styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}
header {
  background-color: #333;
3.5 request	
can you regenrate the styles.css
Regenerating the Styles.CSS returned a complete CSS file. This 

Notes:
It seems to regenerate new content each time I request a change. Will need to modify my requests to just request specific changes from now.

- can you add grid element for the columns
Columns don’t seem to be working. Requested it use grid layout to generate the content mapping.
This vastly changed the page, the colour scheme has changed and the look was different. The grid elements meant the images and text looked much cleaner. This is a big improvement.

- can you suggest some images to download for the page
response:
Sure, here are some suggestions for images related to homebrewing that you could use on your webpage:

- A person pouring a homebrewed beer into a glass
- A close-up of hops or barley
- A person stirring a pot of boiling wort
- A row of filled beer bottles
- A homebrewing kit with all the necessary equipment
- A person holding a glass of beer with a homebrewing logo on it
- A group of people enjoying a homebrewed beer outdoors

You can search for these images on stock photo websites like Unsplash, Pexels, or Shutterstock, or on free image search engines like Google Images. Just make sure to check the usage rights and give proper credit to the photographer if required.

Notes:
Really good explanations when asking specific questions about code:
In this example, I've used the font-size: 4vw; property to set the font size of the hero text to 4% of the viewport width. This means that the font size will scale up or down depending on the size of the screen, allowing the text to fit within the hero image on any device. You can adjust the 4vw value to your liking.

These explanations allowed the code to be added, just need to choose the size to suit. This is much easier than custom cutting code, only need to worry about making the result look good.



