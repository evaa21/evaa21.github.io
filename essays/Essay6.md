---
layout: essay
type: essay
title: Assignment 3 Checkpoint
# All dates must be YYYY-MM-DD format!
date: 2022-11-30
labels: 
  - Checkpoint 
--- 

Introduction: <BR>
Assignment 3 is almost complete with only a few more features and adjustments left to make. Working in a team of 3 has had its advantages along with a few disadvantages. 
Thus far, we have spent a lot of time planning what we would like to do, reviewing previous functions, and debugging. Before completing the project, we would like to introduce what the finished project will be.
Show what each page will look like: <BR>
The website starts at the home page. At the top we have a message welcoming the user saying, “Welcome to Betta Shop”. Down below we have a message telling the user to “Check Out Our Products!” and below showing three images that lead to 3 different pages. The first image on the left is a fish tank and when clicked it leads to the fish tanks product page, showing 6 different tanks to be sold. The second image in the middle is fish, which leads to the betta fish product page. Last but not least, we have a plants image leading to the plant’s product page. Every page has 6 different products to select from with a purchase button at the bottom of each page. 
Additionally at the top in the navigation bar from left to right we have the name of our store Betta. Then we have tabs leading to different pages starting from Homepage, Tanks, Fish, and Plants. Next, we have our search bar where the user could search for products throughout the whole store. After that, we have a user icon and when clicked it will lead to the page where users can edit their account. Following the user icon, we have a shopping cart icon which will lead users to their shopping cart when the icon is clicked here the user can add product quantities and complete the purchase. In addition, the cart will have a remove item function as well as increased validation to ensure that the user is not able to check out “zero” items. 
Lastly, on the far-right corner is the login/register button if the user is not yet logged in or registered, which will then lead to the login page once clicked. If the user is logged in then the button will turn into a log out button, which will subsequently log the user out once it is clicked. 
Currently we have an invoice, but we are planning to adapt this invoice into an invoice that will be emailed to the user upon purchase. The invoice page will be turned into a purchase confirmation page informing the user that an invoice has been emailed to them.
Furthermore, we have added an admin. It is still a work-progress as well. But we know that we will have to use sessions for adding and changing user data. 
Describe your design for your site’s shopping cart: 
The shopping cart will be a separate page. Upon clicking the shopping cart icon in the navbar it will take you to the shopping cart page. So it’s basically a get request to display the cart. Here is the code implemented so far:  
In the cart the user can add quantities for the items they selected. However, the user cannot put in negative quantities. If there is nothing in the cart, the cart page will display a message saying, “Nothing is in your shopping cart!”
Also, the user must be signed in to access their cart. If they try to press the purchase button without being logged in, they will be directed to the log in page. 
The shopping cart is still a work-in-progress, we are planning to add and remove item function. For the add function we will have a button that says update cart, and that will grab the values from the input form of the cart and replace the old session cart with the new session cart from the input form. For the remove function we will also have a column for deleting items in which we have buttons. When the button is clicked the row would delete.
Explain specifically how you will use sessions to manage your shopping cart: (In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.)
 As mentioned above, we are planning to add and remove item functions. These functions will be utilizing sessions. 
There is a cart object session and inside that object there is an array of quantities for each type of product. In other words, cart is an object and is stored in a session and the object contains arrays of quantities and product types.
 
How will you avoid access to your application when the user has not logged in or registered?: <BR>
Some security concerns involve using the clients url to get to the secure pages such as the cart, invoice, or admin page. As previously mentioned, the user must be signed in to access their cart. If they try to press the purchase button without being logged in, they will be directed to the log in page. Also if the user logs successfully then we generate a cookie, and that cookie helps keep the application secure. The cookies are associated with user and we can check which user is logged. 

Upon a successful login, how do you provide personalization in your UI?:<BR>
Upon successful login there are a few personalization’s in our UI. When logged in, the button that used to be a login/register button turns into a log out button which says “logout [user_name]”. Another example of personalization is that in the shopping cart page there is a message at the top say “Hello [name] here is what you have so far” .
We did this by using template strings and the cookies saves the username and users name then we use the cookies to display the data. 
If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?: <BR>
We split the work up as evenly as possible. Sometimes we switched tasks around if one of us had an issue that was too difficult to resolve on our own. We began with splitting up the tasks in terms of general aspects of the project. We worked simultaneously on various file versions and took turns pushing code. It was essential to pull certain code first before saving our other codes.  
Bobby worked on creating the template so the product pages would work. In other words, bringing in elements from assignment 2. Designed the layout of the application and the structure of our code. Made sure to having links to reroute tabs to pages. Also created the sessions for the shopping cart as well as cookies for usernames. 
Alex worked on all the aspects of the admin page which includes creating a whole entire admin page; creating two tabs one of which leads back to the shopping homepage. The second page leads to the functionality page for editing, adding, and changing user information and inventory.  He also helped make the search bar which will lead to products throughout the whole store.
Eva worked on front end development, further validation, assisting in debugging, making sure all comments are put in place and properly describe the codes and its purpose. Also, created the porotype map. 
How are you approaching Assignment 3 differently than Assignment 2?:<BR>
There are various ways in which we are approaching Assignment 3 differently than Assignment 2. One of the biggest differences is that we are now a team of 3 members rather than 2. This allows us to come up with a variety of ideas and break the work up even further. This time we are also making sure to comment a lot more. Also, we are being extremely careful when pushing and pulling comments since we have 3 different computers merging into one repository branch. With that being said, we are also aiming to upload code incrementally to make sure it is tested and debugged before moving forward. We trying to come up with more readable variables so when other members are looking at the code it is easier to comprehend. 
Conclusion:<BR>
This assignment has a lot of aspects and functions to consider when bringing in the finished product. We started with the home page then moved into the various product pages. Also, we brought in the user personalization functions using the login information collected from our users. We added a cart page as well as a soon to be confirmation page indicating an invoice has been emailed. The biggest change and advantage we added into this assignment was the application of sessions and cookies which helped us make the website more realistic and secure. 
![image](https://user-images.githubusercontent.com/89216883/204743034-232a0e44-4489-4f67-bab2-6d0c8486c2f9.png)
