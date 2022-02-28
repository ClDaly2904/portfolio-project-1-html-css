## Testing

## Fixed Bugs

Whilst testing the live site at different stages of building the site, I encountered some unexpected results and bugs. To solve these I largely experimented with changing code and spent a lot of time researching sites such [W3Schools](https://www.w3schools.com/html/), [CSS Tricks](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) and [Stack Overflow](https://stackoverflow.com/).

- ### Header content overflowing
    - At one point the header content was overflowing the header element horizontally, resulting in some of it getting cut off. I used git to compare to earlier versions of code where this had not been happening and I found the extra style in style.css for the header- the insertion of width: 100%;

- ### Overlapping header 
    - After applying media queries to change the layout of the header at 950px and down, the header then overlapped and covered some of the body content beneath it. I tried altering the positioning of the header to see if any of those styles was causing the bug, but after a little research realised I needed to add a margin to the top of the hero image to 'push' that content further down the page to sit under the header

- ### Hover pseudo class on nav bar
    - Another interesting bug I encountered with the header was when applying the hover effect of an orange background over for the nav links. When clicking back onto the Release home page, part of the orange highlight had overflowed onto a new line. I tried lowering the amount of padding, changing the line height and commented out code to confirm it was the :hover pseudo class causing it. In the end I solved it by changing the h1 element in the header and using a ul and li elements nested inside the nav
![screenshot showing nav hover fault on header](docs-images/nav-hover.png)

- ### Content overflowing div on different screen sizes
    - Whilst testing the Release site on different screen sizes, I noticed that on smaller screen sizes around 800px wide and lower, the content of the sections/divs began to overflow. I used Google Chrome's dev tools to analyze the styles applied and found that it due to the fact that I had fixed the height of the divs. I came across the fix for this whilst experimenting with different values for the height attribute, where the shortcut for 'height: fit-content' appeared. Once I had applied this style all the sections/divs, I added padding to keep the desired layout and now I have responsive sections that transform for all screen sizes

- ### Active class on header
    - One of my aims for a user friendly navigation was to have an 'active' class on the header to show the user which page they were currently on. However, I had recurring issues with this working on the sign-up and contact page. This problem came both in design issues (the original plan of an underlined active class didn't show over the border for the sign-up page link), and code errors. After reforming my design to a having the active page be signalled by a slightly different colour background, testing showed that this had not been successfully applied for the sign-up.html page. After a few different attempts (and a brainwave), I realised my error had been to do with CSS specificity and corrected the order of my styles accordingly.


[//]: #W3C validator- HTML
[//]: #Jigsaw validator- CSS
[//]: #Lighthouse
[//]: #Unfixed bugs