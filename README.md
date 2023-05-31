# ASMR Hub for Beginners
#### Video Demo:  <https://youtu.be/9kf8Qtmw1Yo>
#### Description:
##### *The need to find ways to relax and unwind is more important than ever, so I wanted to create a hub for people who are new to ASMR to be able to access most of the typical triggers visually and audibly. I created pages dedicated to certain basics of ASMR like SOUNDS, SIGHTS, VIDEOS, etc.*
#### Index/Home Page:
##### I wanted to create a visually pleasing and relaxing home page so I implemented a canvas elememt that simulates rainfall with splashes. The mouse movement also effects the rainfall. Point toward the bottom of the canvas and the rainfall increases. the mouse placement also effects the direction of the rainfall, to simulate wind. I also modified a codepen to use as a visual navbar when hovered over. I used a svg with a half circle to make my ASMR header curve on a text path and also made it change colors with a keyframe in css. I have a regular navbar at the top of my page with a google search bar. I used flexbox to create description/image boxes to recognize the most common triggers. Next I put a section with several ASMR articles they could access via links. Then I added a blurb about my personal experience with ASMR and how I came to use it. Last I put the footer section that has several go-to links for different parts of my website for quick access and links to all the pages. I debated and changed the layout of this page several times. I first used a hero image, but I felt it looked too crowded. I also changed the background several times until I found a color scheme I liked. Blue is considered the most relaxing ASMR type color, so I wanted my website to have a blue theme.
#### Layout Template:
##### I did not include my index/home page with my layout template because I wanted to create a different visual for all my other content pages. I used the same ASMR header and keyframe but I used another modified codepen for the navbar. One that creates an animation when hovering.
#### Videos Page:
##### For the videos page I wanted to gather a collection of videos that I thought captured a good blend of popular ASMR videos. First I start with a blurd with links to keyword searches for ASMR on YouTube. Then I include a few videos from popular ASMRtists and also popular Mukbang/Eating ASMR content creaters. Then I created a small collection of other content in an unordered list in link form.
#### Sights Page:
##### On my Sights page I wanted to have another interactive visual canvas element. When you hover over the colored circles it creates a relaxing visual effect. I then created a slideshow gallery with different relaxing images. Then I let the user choose which background color they find most relaxing/calming and when they click the button the background changes to that color. I also made the button have an animation. In the next section I display different background images that when clicked on creates an expanded image to view.
#### Sounds Page:
##### On the Sounds page I use converted sound files by transposing sounds from YouTube videos and converting them to wav files and clipping them to make them shorter. I used 2 different sound files for each trigger and add the link to the original video/sound. I then discribe musical frisson in a little more detail and give several examples the user can try for themselves.
#### Misc Page:
##### For this page the content doesn't fall into one specific category so hence the misc header. First I start off with some videos and text of popular ASMR food recipes. Food that is commonly consumed on ASMR/Mukbang videos. Then I have a section dedicated to unintentional ASMR. Things that are not classified as solely/stricktly ASMR but often create the same response in our minds/bodies. I touch on musical frisson here but go into a bit more detail on the sounds page.
#### Survey Page:
##### On my Survey page I have a small blurb and then a short 8 question survey the users can participate in. The basic questions are about the users personal experience with ASMR. Then the user can select a 2 part unique user name from 2 python lists. Then they can submit the form and it will redirect them to a results page.
#### Results Page:
##### The results page consists of a table with all the questions, all the offered answers, all the users answers, and a calculated percentage of their answers in comparison to the most popular answers.
#### app.py Page:
##### On my app.py file I configure flask and sqlite3. I created a asmr-survey database to hold my tables for the survey. I then created several tables to hold the information. I next created routes to all my pages. In the survey route I created several variables to hold the survey answer information as well as their individual 2 part user name, with a random number between 1-90000000000000. I also capitolize each user name and then put them together in a seperate variable. I then have all my SQL submissions put into my database and use python to average out the most frequently answered answers from the survey and find the percentage. I put the percentages into variables and use them to fill out the table on my results page. I then made 2 list that hold random words for the user to select for thie user names.
#### asmr-survey.db:
##### In my ASMR survey SQL database I created several tables. I created a submissions table to store the user name, a unique submission id, and the date the survey was taken. One table for each question was implemented to store the users answers and all possible answers for that particular question, and a foreign key that hold the submission id that links the tables together.
#### Game Page:
##### I created a viually stimulating Javascript game to play where you hit colored circles and they decrease in size with the effects of a firework exploding with particles. I wanted the game to be challenging but not so challenging that it would be stressful or anxiety inducing for the user. The game does tally the users score and ends when a circle touches the player in the center of the screen. Then a modal appears with the users score and the option to start over.