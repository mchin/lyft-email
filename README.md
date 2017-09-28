![Lyft Logo](https://github.com/mchin/lyft-email/blob/master/img/logo_pink.png?raw=true "Lyft Logo")

## Summary

#### Process for completing the project

I started with taking a look at the design and getting a general idea of the layout. I also took a look at the style guide to see the colors and fonts that would be needed. Then I made sure to get all the image urls and assets I needed. Since it’s an email, using tables would be necessary, and there would be some nesting of tables involved. 

I looked up general best practices for responsive email templates by making sure to accommodate for Outlook spacing issues and font sizing issues. I created a basic wireframe of the layout for desktop and then started filling the content in. I started with the level 1 design, and made sure I had desktop and mobile versions done along with QA-ing, then i started the level 2 design, desktop and mobile, and then finally level 3 design. Then QA-ing on different browsers, as well as phone types using simulators. 

#### Any snags you ran into, and how you resolved (interested in seeing how you learn!)

I encountered a snag early on when centering content in the table wrapper, and it took me some time to realize that I forgot to close some <tr> and <td> tags.  I used a program to clean up and format my code, and I realized I was missing those tags because there were unmatched pairs. 

Another issue I ran into was adding the level 3 design code into my current code, for some reason the code I added broke the responsiveness of the page, so I had to backtrack and undo some code line by line. I got to the point right before I broke the code, and then just changed some of the level 3 design code to nest differently and it wasn’t broken anymore. 

Additionally, I had an issue with the stacking order for the mobile responsiveness of the <td> elements in the level 3 design. The image and the description text were not stacking in the correct order. I tried changing the css and adding a direction attribute and used “direction: rtl” but the layout stacking was not changing like it should, and nothing was happening , so I decided to try coding “dir=“rtl” inline in the table tag. I then decided to manually swap the <td> elements , but I feared it would break the desktop version, but it didn’t and the stacking worked as expected on the mobile version. 

#### Approach to QA

I QA while I code, so it’s a constant process of coding and then checking periodically to make sure I’m heading in the right direction. 

Testing tools are important so one knows what specifics to test for which include the top email clients. Also, one needs to make sure to have a checklist of things to check for before an email gets sent out. Make sure the links work when you click on them, and all the text is readable in different email clients. Also, making sure data is going into your email program to track opens and clicks, etc. by analyzing metrics and data. 

A final QA is done on different email clients, browsers, and mobile devices as well as on sites like putsmail.com. or litmus software. 

#### Any thoughts on optimizations, how you might improve the template

There’s a good balance of images and text  but there’s a lot of whitespace. (in the first and second designs)

Maybe add small icons or another color to the designs to give a little pop and maybe more personalization. 

## Question - Level 4: Dynamic content
### You’ve been asked to send an email to a national audience. One section of the email needs to be different depending on which region the subscriber has been approved to drive; there are 50 different regions that could fall into this audience. How would you approach this task?

I would try and see if I could break down the 50 different regions to smaller less concentrated regions, but there would be less specific personalization. Additionally, if on a time sensitive campaign, I would just filter out and send to the regions that have the most subscribers.  So it’s a matter of speed vs quality personalization. 

If the above is not feasible, then you would need to have 50 different segments representing each region, and then filter all the people who belong to each region to target them in the email. The dynamic content in the email would show based on the person’s region segment or geolocation, depending on how the data was gathered. This could be time consuming, so works best if there’s no rush and would result in greater quality personalization. 
