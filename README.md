# EmailAlertsOnWhatsApp
A project to fetch emails and send them to  WhatsApp using Twilio
EmailAlertsOnWhatsapp
About
This repository contains the code which fetches recent mails from a user's gmail account and send it to his/her Whatsapp account using the Twilio environment

Prerequistics
App Passwords
You can read more about here

Setup
  1.Create Twilio Account and connect your whatsapp number to it (It's free)

  
  2.Go through the guide they provide and connect your whatsapp number such that you can send a message to the number and receive a message(Initially it would be something along the lines of "You send <your_message>")


  
  3.Navigate to the function page through the navigation bar at the left

  
  
   ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/51f6939ac590b13727fd4654428c1e556ef2c45c/Screenshot%202024-12-15%20225226.png)
  
                     
    

4.Create a new function (with any name you like) and copy the code in there.




5,Inside the functions page, go to settings->Dependencies and make sure you have all the dependencies added as shown in the figure
Dependencies


                                              
 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/66ac2beb80f0fdf041e3f1fd8d9dc0a02fb14026/Screenshot%202024-12-16%20025710.png) 






 






 


6.Now go to settings->Environment Variables and then set emailID as your GMail id and passKey as your App Password(If you don't know about app passwords please read the pre-requistic paragraph above)

   Environment variables
   
 
 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/96ef518906b8b5273cfb191f4b3c9ccb8a74d0a9/envi.jpg)

 
7.Save and select Deploy all

 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/75fa483eda19232897484b2ffe5b8514db908eba/deploy.png)
 
8.Select the 'Copy URL' present just below the code editor to copy the link of the function after deploying.


9.Now go to Programmable Messages->Settings->Whatsapp Sandbox Settings and paste the copied URL in step 8 into the 'WHEN A MESSAGE COMES IN' field in Sandbox Configuration


10.Save and you are good to go



Features/Working

The chatbot searches for keywords and replies accordingly. The followinf keyword are currently implemented.

1.Help : This gets the list of all keyword
 
 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/de5e4b1aa9539fddb23c7266d59b09f0dea77b50/Screenshot%202024-12-16%20013146.png)

2.mail/email : This gets the recent 5 emails
 
 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/53c93a12916214300f59eb5fb70cf756a2ab7482/Screenshot%202024-12-16%20013324.png)
3.mail/email + unseen : This gets the latest  unseen emails
 

 ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/0d8ecea40fe43bd103a9b019daca37eff433b990/Screenshot%202024-12-16%20013702.png)
3.Hello/Hey : This just greets you and asks if you want to get mails. If you type es then it fetches the mails.
  ![image alt](https://github.com/Monika803-ops/EmailAlertsOnWhatsApp/blob/f8a68fff3264c7f7d02a69d11179b798ca67d457/Screenshot%202024-12-16%20013809.png)
Future Plans
1.Add more functionalities/options with the email type being queried
2.Using some algorithm/AI to predict what the user is asking and reply accordingly. Currently it is hardcoded.
3.Add more features apart from email fetching (like weather, film reviews/recommendations) and turn it into a whatsapp assistant.


