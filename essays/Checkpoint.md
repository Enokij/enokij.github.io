---
layout: essay
type: essay
title: "Checkpoint Assignment 3"
# All dates must be YYYY-MM-DD format!
date: 2022-11-30
published: true
labels:
  - MIS
---

<h4>Show what each page will look like. The pages do not have to be “functional” but the design should clear.</h4>![Assignment 3 layout](https://user-images.githubusercontent.com/112168487/205006729-bf6040ec-bae3-4e6f-ba57-37573c4509ec.png)
[Click here to watch screencast.](https://youtu.be/BfcynrnXhEM)

<h4>Describe your design for your site’s shopping cart. That is, will it be a separate page that the user can view and edit, or will it be integrated into the product pages? If so, describe in detail how this will work on your site. Provide several examples of using the cart.</h4>
<p>My design for the shopping cart will be similar to Amazon's shopping cart, where the user will be taken to a separate webpage to view all their items and the quantities. The shopping cart will work by checking first to see if they are logged in. Then, by having that user information in the session, it will remember what the user has put into their shopping cart so that if they leave the site and come back, their products will still be in there. Then, from whatever quantities they decide to purchase from each item, it will show up in the shopping cart, where the user will be able to change the quantity by putting in a different number. Once they are ready to check out, they just click checkout and they will be redirected to the invoice page where they will be shown what they purchased and their total. <br> One example of using the shopping cart will be if the user decides to purchase a specific keyboard, they will be able to view it in their shopping cart. Then say they want to buy a certain amount of switches for that keyboard, they can go to the switches page and add the amount of switches they want. Then if they realized they need more switches, they can go into their cart and change the amount of switches they want to buy to the correct amount. Another example would be if they realized they wanted to purchase a different keyboard, they can go into their cart and remove the previously selected keyboard and select the keyboard they actually want to purchase and put it in the cart. </p>

<h4>Explain specifically how you will use sessions to manage your shopping cart. In particular, what shopping cart data will be stored in the session, what data format will be used (NOT what data type, but the format like with the data format used for your registration data). Use code examples showing what data structures (such as arrays and their objects) you will use to manage the shopping cart data and how they will be used in a session.</h4>
<p>I would create an object, and in that object would include different arrays for each product, so that the cart will be able to recognize what product will be purchased and how many products will be purchased. An example of the array code would be: "Keyboard":[ { "name": "Tofu65", "price": 150, “quantity_purchased”: 0}. To request data from the session, I would use something like “request.session”.</p>

<h4>How will you avoid access to your application when the user has not logged in or registered? What are the particular security concerns you must address?</h4>
<p>By using cookies, the server can check to see if that user has cookies. If the user logged in, they would have a cookie for that session, if not, they wouldn’t. Then, by running validations on the check out button, we can check to see if the user has cookies or not, if they do then they will have access to purchasing the items in their cart, and if not then they will be prompted to log in. Some security concerns I must address will be if the user has left the website inactive for too long. This could be a security reason as if they forgot to log out, someone could go on the same computer and use their account to purchase things. To fix this, I would set a timer on the cookie by giving it an age, in milliseconds, so that when the timer is up the cookie will expire, which would then log the user out.</p>

<h4>Upon a successful login, how do you provide personalization in your UI? Explain how you did or will do this (paste code if necessary)</h4>
<p>Upon a successful login, I would personalize my site by giving them a welcome page with their name right after they log in. I would also put their name in a thank you message after they have purchased their products and send them an email with their invoice.</p>

<h4>If you are working with partners, how will you split up the work in your team so that you are working in parallel as effectively as possible? That is, who is doing what and when?</h4>
<p>I am working alone.</p>

<h4>How are you approaching Assignment 3 differently than Assignment 2?</h4>
<p>I am definitely starting the assignment earlier and thinking more about what to do and planning it out better, step by step. This allows me to work more efficiently as I have a dedicated plan that I can follow. I will also restart from the ground so that my site looks cleaner, and just pull certain code from assignment 2 and use it in assignment 3. This way I can make the changes I need easily and not get stuck just trying to modify assignment 2.</p>
