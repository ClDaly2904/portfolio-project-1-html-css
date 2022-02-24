# Release

##  About
Release is a website that hopes to introduce users to two powerful self-improvement techniques; meditation and yoga. The target users for this site will be beginners searching for information about what the benefits of meditation and yoga are, how they can perform these practices at home and prepare them for what equipment they might need. 

Release will also provide a great starting point for those that wish to go on and adopt meditation and/or yoga by providing them with useful links and materials that can be accessed by users in their own local areas. Users will also have the option of contacting a member of the Release team, or recieving monthly self-improvement and mindfulness tips through the monthly newsletter.

[//]: # screenshots

![alt text](image-file-path.png)


## Features

- Nav bar - the navigation bar is a consistent feature across all pages of the site. It includes links to the Home Page, Meditation page, Yoga page and the Signup page. It is located at the top of each page and is 'sticky' so that the user can intuitively locate and use to easily navigate between pages across all devices no matter how far down their current page they are.
- Footer - the footer is also a feature on all pages, allowing the user to access Release's Facebook, Twitter and Instagram social media platforms. It also contains an email address for Release, providing an alternate route for users to access contact information without having to navigate to a different page, along with providing copyright information.

- Home page
    - Landing page image- the large hero image serves to grab the user's attention and to set the tone of the site. It demonstrates the type of tranquility and peacefulness that can be found when practicing meditation and yoga and inspires the user to attain the same.
    - Connect section - this section serves to pique the user's curiosity, introduce the user to the two self-improvement techniques focused on in the site and highlight what information they can expect to find in the relevant pages.
    - Newsletter and fig section - this section compliments the rest of the homepage by including a data graph to reassure users that the site is a reliable source of information and there are real proven benefits to the self-improvement menthods included. The image demonstrates the state of mindfulness the user may be hoping to achieve. This section also promotes Release's monthly newsletter and what they can expect from it.

- Meditation and Yoga pages
    - Intro section - gives the user an understanding of what each method entails and how it can be beneficial to them. This is presented first on the page as they are more likely to carry on reading once they have seen the positive effects both meditation and yoga give.
    - How to section - gives the user a basic understanding how to undertake the practice and provides resources for further information
    - Equipment section - allows the user to see what equipment they might need. Links to buy equipment which may make the user excited to have a go at one or both of the practices. Also provides 'at home' alternatives for those who want to try meditation or yoga out before investing. Also has a call to action button to entice the user to find a meditation/yoga group near them, as many people like the social aspect of exercise or are more committed when part of a group.

- Contact and Sign-up page
    - Contains varied contact information for Release for users seeking more help or information.
    - The sign-up form not only allows the user to sign up to the monthly newsletter but lets them set preferences for what kind of information they would like to recieve (meditation, yoga or general mindfulness tips), in turn giving feedback to Release to see what area is the most popular. The user will be asked to submit their full name and email address.

- Future features
    - Would like to add inspirational quotes layered over existing layout to encourage users
    - Would like to add carousel made up of yoga poses to give users more inspiration, and encourage users to return to the site
    - Would like to add a 30-Day Meditation and (or) Yoga tracker/ challenge to enagage users and help them track their progress, as it can take some time for habits to form. People who have committed to something for 30 days are more likely to continue it. 

## Testing

[//]: #fixed bugs

- Header content overflowing
    - At one point the header content was overflowing the header element horizontally, resulting in some of it getting cut off. I used git to compare to earlier versions of code where this had not been happening and I found the extra style in style.css for the header- the insertion of width: 100%;.
- Overlapping header 
    - After applying media queries to change the layout of the header at 950px and down, the header then overlapped and covered some of the body content beneath it. I tried altering the positioning of the header to see if any of those styles was causing the bug, but after a little research realised I needed to add a margin to the top of the hero image to 'push' that content further down the page to sit under the header.
- Hover pseudo class on nav bar
    - Another interesting bug I encountered with the header was when applying the hover effect of an orange background over for the nav links. When clicking back onto the Release home page, part of the orange highlight had overflowed onto a new line. I tried lowering the amount of padding, changing the line height and commented out code to confirm it was the :hover pseudo class causing it. In the end I solved it by changing the h1 element in the header and using a ul and li elements nested inside the nav.
- Content overflowing div on different screen sizes
    - Whilst testing the Release site on different screen sizes, I noticed that on smaller screen sizes around 800px wide and lower, the content of the sections/divs began to overflow. I used Google Chrome's dev tools to analyze the styles applied and found that it due to the fact that I had fixed the height of the divs. I came across the fix for this whilst experimenting with different values for the height attribute, where the shortcut for 'height: fit-content' appeared. Once I had applied this style all the sections/divs, I added padding to keep the desired layout and now I have responsive sections that transform for all screen sizes.


[//]: #W3C validator- HTML
[//]: #Jigsaw validator- CSS
[//]: #Lighthouse
[//]: #Unfixed bugs

## Deployment

## Credits

- Content
    - colourscheme- Shutterstock website https://www.shutterstock.com/blog/color-palettes-for-websites?kw=&c3apidt=71700000083936683&gclsrc=aw.ds&gclid=EAIaIQobChMIp-mb39H19QIVCL_tCh1txAjJEAAYAyAAEgIlwfD_BwE
    - Definitions- formed using Wikipedia.com- https://en.wikipedia.org/wiki/Yoga for yoga, https://en.wikipedia.org/wiki/Meditation for meditation
    - Benefits of meditation- https://www.mayoclinic.org/tests-procedures/meditation/in-depth/meditation/art-20045858
    - How to meditate steps https://www.mindful.org/how-to-meditate/
    - Benefits of yoga https://www.hopkinsmedicine.org/health/wellness-and-prevention/9-benefits-of-yoga
    - Some inspiration taken form The Code Institute 'Love Running' project, so there may be some code similarites. In particular, I used this as a base for my hero image sections and form.
- Media
    - Correlation-graph made using Canva
    - Images found on Unsplash and Pixabay
    - How to meditate video from Goodful https://www.youtube.com/channel/UCEMArgthHuEtX-04qL_8puQ
    - Introduction to yoga video from Yoga with Adrienne Youtube https://www.youtube.com/watch?v=v7AYKMP6rOE&ab_channel=YogaWithAdriene
