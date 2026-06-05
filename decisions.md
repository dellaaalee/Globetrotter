# Globetrotter — Decisions Log

## Milestone 0: Setup and Planning
- Destination chosen: Korea
- Primary audience: people trying to visit Korea for the first time
- One design decision that reflects the destination: 
- Wireframe format used (hand-drawn / Figma / other): the wireframe is made in figma and shown in asset/img/wirefram1.png and asset/img/wireframe2.png


## Milestone 1: HTML Structure

I use <figure> instead of <div> when wrapping around img in photo-gallery because I need to include a caption, and <figurecaption> can only be used with <figure>. <div> is a semantically meaningless container to wrap around. For a photo gallery, using <figure> would be more appropriate.

When I was making navbar, I had to change the structure to make sure that it was the same throughout all the page. Claude orginially had it made as changing based on what page you were in, so I changed it to where the navbar is the same no matter what page you are currently located. I also made sure that the page that I'm currently in is highlighted. 

My wireframe guided a specific decision because I decided that I wanted top attraction, food guide, and photo gallery to be a different page, so when I coded the html part of this project, I had a separate page for this, and linked them (or reference them) in the index.html page


## Milestone 2: CSS Styling
I choose to do a black and red color scheme. Korea's national color from the flag is red, blue, black, and white, so I decided to pick the two colors from those choices. 
I rejected some of the color choices that claude suggested because it didn't fit with the color scheme/ color that I choice for the project. 
The navbar styling didn't look right at first because claude just populated the nav in the middle of the screen whereas I wanted the navbar sections to be at the right of the screen. I changed it intentionally to be at the right of the screen. 

## Milestone 3: Flexbox Layout
One Flexbox property I chose deliberately was using `justify-content: center` on key containers like the top-attraction and food sections so the main cards stay visually centered and balanced across screen sizes. One place where Claude's generated layout did not match my plan was the top-attraction page, where nested sections were accidentally repeated and made the structure messy; I corrected it by simplifying to one clean card section and then restyling it to match my wireframe. A layout challenge that required changing HTML structure was the food guide image wrapper, where I switched between `div` and `figure` to align with semantic intent and styling needs, and I also adjusted wrappers so the card layout could stay consistent when different image sizes are used.

## Milestone 4: Responsive Design
I'm sizing for desktop, mobile, and iphone. 
320px
768px
1024px

I made the website different from desktop to mobile by changing some features rather than just shrinking the elements on the page. For example, the food card switch to a vertical flow and different gradient direction. Top attraction becomes a stacked instead of side by side and gallery goes to signle column for predictable scrolling and easier tap tagets. 

## Stretch Features
_Add entries if you implement any stretch features._