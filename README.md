WHAT IS BOTSIFY?
=======

Botsify helps you create facebook messenger chatbot for your business/page without any coding.

You can artificial intelligent chatbots with our technology with no technical knowledge require. Technical mates can go extra mile with Botsify by integrating their API with Chatbot to make it extra effective. People can do analysis on different behavior of their bots and also run marketing campaigns to the people who opted for it.

With over a billion users you can now double you conversions with messenger chatbots.

There are a lot of businesses excited with the lunch of facebook messenger because they have one more medium other than Email Marketing to start interacting with their customers and increase conversions by assisting through the process/offering different deal to their customers.

When facebook messenger API was launched every other blog including Techcrunch started bashing the AI of the chatbot but on other end they all created their own messenger bots as well. So first few businesses who shifted to use Facebook Messenger includes:
 * TechCrunch
 * Spring
 * Poncho
 * CNN
 * Wall Street Journal

GETTING STARTED
=======

Creating facebook application
---------------

In order to make your chatbot with botsify you need to first create a Facebook application. You can create one for [FREE HERE](https://www.developers.facebook.com "Facebook Developers"). One you have your application you need a Facebook page as well or it could be your existing business page.

Creating your first bot with botsify
---------------

Once you have created the application in Facebook you need to create an account with Botsify and login. In the left hand menu you should see **Create Bot**, go ahead and click it. It is a simple form to take information about your Facebook application and page which you just created. You need to know following fields before filling out this form.


### Facebook Application ID

This is the ID of your application which you just created. You can find it in your application settings.

![alt text](http://i.imgur.com/mrjbNnr.png "Facebook Application ID")

### Secret Key

It is just a connector between Facebook Application Webhook and Botsify. You can type anything for example **my_secret_key**.


![alt text](http://i.imgur.com/XAJPaf3.png "Secret Key")

### Facebook page access token

It is the access token of the page for which you want to make your chatbot.

![alt text](http://i.imgur.com/EW3dlmb.png "Facebook page access token")

Connecting your facebook application with botsify
---------------

Once you have filled this form you will see your application webhook. This webhook will allow you to connect your facebook application with Botsify.

To setup a webhook you need to go to “Your Facebook Application -> Messenger -> Setup Webhook -> Edit Events”. You will see a webhook configuration form like in the snapshot below.

![alt text](http://i.imgur.com/sQEUr83.png "Connecting your facebook application with botsify")

 * Your URL is going to be the one provided by Botsify.
 * Your Application Secret Key is going be the same which you filled while filling your form.
 * Check all options in order to enjoy full access to the messenger API. You can be selective as well about these options.


Verifying application connection
---------------

### Verification from facebook

Once you see this **Green Check mark**. It is a clear signal that you have successfully connected your application and Botsify.

![alt text](http://i.imgur.com/6BgbFkg.png "Verification from facebook")

### Verification from botsify

 * Now turn on your application in Botsify. You can also use this button to turn it off anytime to switch from **Bot mode** to **manual mode**.
 * Go to your facebook page (which you connected)
 * Send message to the page and type **Hi**.

![alt text](http://i.imgur.com/IZX1ZLz.png "Verification from botsify")


 * You should get an automated **Bot** response telling you that you have successfully configured your Bot.
 * Go back to Botsify and click “Test”. If all set you should get this screen which will help you write your chatbot?

![alt text](http://i.imgur.com/ESqam1K.png "TEST from botsify")


Write / Setup your chatbot responses
------------

Botsify let you manage your chatbot through a simple and easy interface. We currently support two type of responses.
 * Basic Responses
 * Advance Responses

### Adding Basic Responses

For basic responses we currently have **Greeting Response** which will be the first response to your customers when they start conversation with the Bot. 

 * Let’s type : **Hi welcome. Please use @list to know about all commands I support**.

Second is **Default Response** which is the response when your chatbot will fail to understand the conversation. 

 * Let’s type : **Sorry, I don’t understand what you are saying. Let’s start over with @list**.

Once you have submitted these two responses you can go back to your page and chat with your bot. You will not receive the greeting message because you have already started conversation with the bot but if you type “asasafaf3131”; some gibberish; it will respond with our default response.

![alt text](http://i.imgur.com/Qz4ZwfY.png "Adding Basic Responses")

#### Adding Advance Responses

##### Understand the UI of advance responses

For advance responses you can go extra mile and create some hard coded and dynamic API based responses. You will see “Messenger like” UI in advance responses which let you create stories with respect to your business.

![alt text](http://i.imgur.com/x7t0W8W.png "Adding Basic Responses")

Let’s understand the UI first. If you select **Your Application name** in left hand panel it means you are trying to chat as a user. And if you have user selected in the left hand panel it means you are trying to chat as a bot.

In lower of the left hand panel there are command and parameter fields. So let’s talk more about commands and parameters.


##### Commands:

Command is something which your chatbot supports and user can use it. In step 1 we asked user to type @list to know about our commands. @list itself is a command but it has no parameters. So let’s say user type @list we can responds this message in any manner we like.

##### Parameters:

Parameters are something which gives some context to a command. Let’s say “@shoes/men” gives the context that our user is interested in men shoes. So shoes can be of several different types and parameters help us understand more about @shoes.



Creating advance chatbot for a shoe store
-----------------------------------------


Let’s say we have an online shoes website and a story is user is chatting in order to know what products are available.

 * So while you have **bot** selected in the left hand panel type @list as a user. You will see the command and parameters fields are automatically filled. 

![alt text](http://i.imgur.com/K1qaQhL.png "Adding Advance Responses")


 * Now select **User** from left hand panel and respond to this command as a “Chatbot” we will write: **@shoes/men @shoes/women @sandals @slippers**
 * A confirmation pop up will appear; click **OK** to submit your response. 
 * Go back to facebook messenger and type: **@list**. You will see that you get the response of @list we just submitted.

![alt text](http://i.imgur.com/b8imNyW.png "@list")

Now assume our user is more interested in **Men shoes** and writes @shoes/men. Once you type this command as a user **command and parameter fields** will be auto filled with “shoes” and “men” respectively. Since you can have any number of parameters to give more contexts to your command you will see **param1** associated as the key of your first parameter.

![alt text](http://i.imgur.com/5gpKufP.png "Param1")

Now responds to this message as a bot and type: **Sorry, we do not have {param1} shoes in stock. Do you want me to show some slippers?**.

Now you see we can use parameters of command in our responses to make it more customized. 
So if you go back to your messenger and type: **@shoes/men** you will see that your bot says. **Sorry, we do not have men shoes in stock. Do you want me to show some slippers?**.

Since this is personalized response even if your user type **@shoes/women** your bot will say. **Sorry we do not have women shoes in stock. Do you want me to show some slippers?**.

![alt text](http://i.imgur.com/KdkyU0h.png "Param2")


Advance API based responses
---------------

Now there is clearly a problem. You can see that although you have women shoes in store you are saying that you do not have women shoes in stock. There comes the use of dynamic API based responses.

So instead of **Sorry we do not have {param1} shoes in stock** if you type your API end point, e.g:

**www.abc.com/api/v1/check/stock/{param1}**

This will call your API end point with related parameter and you can give your response to customers in string formatted, right from your API.


Conclusion
===========

So this is how you can create your messenger chatbots with Botsify. Currently your application is in development mode but you can fill in additional information and request facebook to publish your chatbot. Once it is published you can even link messenger on your website page.

We are helping businesses to increase conversions by making intelligent chatbots. If you think that you are too non-technical to write your chatbot just ping us and take quotation through the chat support available 24/7 on our website. We can help you make customized AI based chatbots for your business considering every possible user story of your business.

Currently botsify is running beta and continuously improving the website and functionalities. Let us know your feedback and queries at support@botsify.com.

Thanks.

 * [My website](http://botsify.com) (botsify.com)
 * [Github](http://github.com/usamanoman) (@usamanoman)
 * [Twitter](http://twitter.com/botsify_app) (@botsify_app)
