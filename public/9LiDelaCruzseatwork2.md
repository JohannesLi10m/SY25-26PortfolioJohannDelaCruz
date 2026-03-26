Seatwork #2 - Getting to know CSS Position and z-index.
This seatwork will ask you to implement the different CSS position on a given code.
short link to this .md file is: https://bit.ly/4c61P9K
Resources (also found in Khub week 5)
4 Minute Youtube Video on CSS Position
CSS Position Tutorial
Instructions:
This is individual submission in khub, but you can work with a partner. When you submit in khub please place both your names in the submission bin.

Guided Activity (30 minutes), please follow what is being required.

Make a copy of this .md file to your Q4 repository and name it as SectionLNseatwork2.md example 9LiCruzSeatwork2.md. Place it in your q4 repository vscode local computer. Committing frequently to your Github repository.
Copy the code below and paste it inside a new file (name it as SectionLNseatwork2.html). Place this file in the same location where the .md file is saved.
Change the content values of the meta tags to your names for author/s and the date today for revised.
Please do the following tasks that will ask you to reposition HTML elements then answer the guided question for each task on the .md file. Commit changes to the .md file and to the .html file as well. - This seatwork is worth 20pts and should be submitted by the end of the period The link to KHub submission bin.
Submit the links to your .md file and .html file.
<!DOCTYPE html>
<html>
<head>
  <meta name="author" content="<your names>" />
  <meta name="revised" content="<date today>" />
  <style>
    body { font-family: Arial, sans-serif; }
    .header, .footer {
      background: lightblue;
      padding: 10px;
    }
    .footer {
       opacity: 0.5;
    }
    .sidebar {
      background: lightgreen;
      width: 150px;
      height: 200px;
    }
    .content {
      background: lightyellow;
      width: 300px;
      height: 200px;
    }    
  </style>
</head>
<body>
  <div class="header">Header</div>
  <div class="sidebar">Sidebar</div>
  <div class="content">Main Content</div>
  <div class="footer">Footer</div>
</body>
</html>
Step 1 (Static vs Relative):
Add in css position: relative; top: 20px; left: 20px; to .sidebar.

Guided Question: What changed compared to the default static positioning? Try to give different values to top and left or you can change it to bottom, right.
Ans: The sidebar block moved down and to the right, this is because of the amount of pixels inputted in the code that gave a border of the same amount of pixels.

Step 2 (Fixed):
Add in css position: fixed; bottom: 0; width: 100%; to .footer.

Guided Question: What happens when you scroll the page? Why does the footer behave differently from position relative?
Ans: The footer is still and fixed in place even when trying to scroll the webpage, compared to the position relative, it is fixed in place and can only be moved if the bottom factor is set to a number that is not equal to 0.

Step 3 (Absolute):
Add in css position: absolute; top: 66px; left: 200px; to .content.

Guided Question: What is the effect of position: absolute on an element? How is it different from fixed?
Ans: Absolute position effects the element's position relative as it positions it next to its nearest ancestor. Its different from fixed because you can still choose the amount of border or input where you want to put the element.

Step 4 : (Absolute)
Add in html <div class="notice">Notice!</div> and include the css below:
.notice {
    position: absolute;
    top: 60px;
    left: 400px;
    background: orange;
    padding: 10px;
    z-index: 2;
}
Give .content a z-index: 1.

Guided Question: Why does the notice appear on top of the content? What happens if you swap the z‑index values?
Ans: Notice! appears on top of the content because it has a higher z-index value, if their z-index values are switched, Notice! goes behind content and only a portion of it can be seen. 

Challenge:

What changes that you have to do on the code that will position .notice box on the top right corner of the .content box? Please write the code on paper as well (both html and css on the part of .notice and .content).
Ans: To position the .notice box on the top right side of the .content box, you must add a value of pixels to the left: ;, I added 50 pixels and the .notice box moved to the right by about 50 pixels.

Try to change the position of .content to relative then to fixed. What do you observed each time?
Ans: When changing the position to relative, the Main Content box moved to the middle, when changed to fixed, it stays in its original position before being moved to relative.

What do you observe on about the effect of z-index on .notice and .content boxes?
Ans: The z-index value determines if the .notice and .content boxes if they are behind each other, or infront of one another.

Please answer the following reflection questions (15 minutes)

a. Could you summarize the differences between the CSS position values (static, relative, absolute, fixed)?
static: Doesn't move with an animation, can be moved by pixels
relative: Moves relative to its nearest ancestor block
absolute: Block is able to be moved in whatever position
fixed: Block is fixed, can never be moved

b. How does absolute positioning depend on its parent element?

c. How do you differentiate sticky from fixed (you can research on sticky)?

d. If you were designing a webpage for a school event, how might you use positioning to highlight important information? Please give concrete examples.