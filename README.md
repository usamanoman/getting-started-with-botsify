WHAT IS BOTSIFY?
=======

Botsify helps you create facebook messenger chatbot for your business/page without any coding.

You can artificial intelligent chatbots with our technology with no technical knowledge require. Technical mates can go extra mile with Botsify by integrating their API with Chatbot to make it extra effective. People can do analysis on different behavior of their bots and also run marketing campaigns to the people who opted for it.

With over a billion user you can now double you conversions with messenger chatbot.

There are a lot of businesses excited with the lunch of facebook messenger because they have one more medium other than Email Marketing to start interacting with their customers and increase conversions by assisting through the process/offering different deal to their customers.

When facebook messenger API was launched every other blog including Techcrunch started bashing the AI of the chatbot but on other end they all created their own messenger bots as well. So first few businesses who shifted to use Facebook Messenger includes:
 * TechCrunch
 * Spring
 * Poncho
 * CNN
 * Wall Street Journal

GETTING STARTED
=======

Creating Facebook Application.
---------------

In order to make your chatbot with botsify you need to first create a Facebook application. You can create one for free here. One you have your application you need a Facebook page as well or it could be your existing business page.

*In short: just download this file and upload it somewhere.*

The main JS and CSS files are also available in [npm] and [bower].

[Default theme template >][template]

[Blank template >][blank]

[bower]: http://bower.io/search/?q=flatdoc
[npm]: https://www.npmjs.org/package/flatdoc

Registering on Botsify and 
creating your first bot:
---------------

Once you have created the application in Facebook you need to create an account with Botsify and login. In the left hand menu you should see **Create Bot**, go ahead and click it. It is a simple form to take information about your Facebook application and page which you just created. You need to know following fields before filling out this form.


### Facebook Application ID

This is the ID of your application which you just created. You can find it in your application settings.

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.github('USER/REPO')
});
```
### Secret Key

It is just a connector between Facebook Application Webhook and Botsify. You can type anything for example **my_secret_key**.


``` javascript
Flatdoc.run({
  fetcher: Flatdoc.github('USER/REPO', 'Changelog.md')
});
```

### Facebook page access token

It is the access token of the page for which you want to make your chatbot.

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.github('USER/REPO', 'Changelog.md')
});
```

Connecting your facebook application with Botsify
---------------

Once you have filled this form you will see your application webhook. This webhook will allow you to connect your facebook application with Botsify.

To setup a webhook you need to go to “Your Facebook Application -> Messenger -> Setup Webhook”. You will see a webhook configuration form like in the snapshot below.

 * Your URL is going to be the one provided by Botsify.
 * Your Application Secret Key is going be the same which you filled while filling your form.
 * Check all options in order to enjoy full access to the messenger API. You can be selective as well about these options.


Verifying Application Connection
---------------

### Verification from facebook

Once you see this **Green Check mark**. It is a clear signal that you have successfully connected your application and Botsify.

To setup a webhook you need to go to **Your Facebook Application -> Messenger -> Setup Webhook**. You will see a webhook configuration form like in the snapshot below.

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.file('http://yoursite.com/Readme.md')
});
```

### Verification from botsify

 * Now turn on your application in Botsify. You can also use this button to turn it off anytime to switch from **Bot mode** to **manual mode**.
 * Go to your facebook page (which you connected)
 * Send message to the page and type **Hi**.
 * You should get an automated **Bot** response telling you that you have successfully configured your Bot.
 * Go back to Botsify and click “Test”. If all set you should get this screen which will help you write your chatbot?

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.file('http://yoursite.com/Readme.md')
});
```

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.file('http://yoursite.com/Readme.md')
});
```

Write / Setup your chatbot responses
------------

Botsify let you manage your chatbot through a simple and easy interface. We currently support two type of responses.
 * Basic Responses
 * Advance Responses

### Adding Basic Responses

For basic responses we currently have **Greeting Response** which will be the first response to your customers when they start conversation with the Bot. 

Let’s type : **Hi welcome. Please use @list to know about all commands I support**.

Second is **Default Response** which is the response when your chatbot will fail to understand the conversation. 

Let’s type : **Sorry, I don’t understand what you are saying. Let’s start over with @list**.

Once you have submitted these two responses you can go back to your page and chat with your bot. You will not receive the greeting message because you have already started conversation with the bot but if you type “asasafaf3131”; some gibberish; it will respond with our default response.

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.file('http://yoursite.com/Readme.md')
});
```

#### Adding Advance Responses

##### Understand the UI of advance responses

For advance responses you can go extra mile and create some hard coded and dynamic API based responses. You will see “Messenger like” UI in advance responses which let you create stories with respect to your business.

``` javascript
Flatdoc.run({
  fetcher: Flatdoc.file('http://yoursite.com/Readme.md')
});
```

Let’s understand the UI first. If you select “Your Application name” in left hand panel it means you are trying to chat as a user. And if you have user selected in the left hand panel it means you are trying to chat as a bot.

In lower of the left hand panel there are command and parameter fields. So let’s talk more about commands and parameters.


#### Lightning-fast parsing

Next, it uses [marked], an extremely fast Markdown parser that has support for
GitHub flavored Markdown.

Flatdoc then simply renders *menu* and *content* DOM elements to your HTML
document. Flatdoc also comes with a default theme to style your page for you, or
you may opt to create your own styles.

Markdown extras
---------------

Flatdoc offers a few harmless, unobtrusive extras that come in handy in building
documentation sites.

#### Code highlighting

You can use Markdown code fences to make syntax-highlighted text. Simply
surround your text with three backticks. This works in GitHub as well.
See [GitHub Syntax Highlighting][fences] for more info.

    ``` html
    <strong>Hola, mundo</strong>
    ```

#### Blockquotes

Blockquotes show up as side figures. This is useful for providing side
information or non-code examples.

> Blockquotes are blocks that begin with `>`.

#### Smart quotes

Single quotes, double quotes, and double-hyphens are automatically replaced to
their typographically-accurate equivalent. This, of course, does not apply to
`<code>` and `<pre>` blocks to leave code alone.

> "From a certain point onward there is no longer any turning back. That is the
> point that must be reached."  
> --Franz Kafka

#### Buttons

If your link text has a `>` at the end (for instance: `Continue >`), they show
up as buttons.

> [View in GitHub >][project]

Customizing
===========

Basic
-----

### Theme options

For the default theme (*theme-white*), You can set theme options by adding
classes to the `<body>` element. The available options are:

#### big-h3
Makes 3rd-level headings bigger.

``` html
<body class='big-h3'>
```

#### no-literate
Disables "literate" mode, where code appears on the right and content text
appear on the left.

``` html
<body class='no-literate'>
```

#### large-brief
Makes the opening paragraph large.

``` html
<body class='large-brief'>
```

### Adding more markup

You have full control over the HTML file, just add markup wherever you see fit.
As long as you leave `role='flatdoc-content'` and `role='flatdoc-menu'` empty as
they are, you'll be fine.

Here are some ideas to get you started.

 * Add a CSS file to make your own CSS adjustments.
 * Add a 'Tweet' button on top.
 * Add Google Analytics.
 * Use CSS to style the IDs in menus (`#acknowledgements + p`).

### JavaScript hooks

Flatdoc emits the events `flatdoc:loading` and `flatdoc:ready` to help you make
custom behavior when the document loads.

``` js
$(document).on('flatdoc:ready', function() {
  // I don't like this section to appear
  $("#acknowledgements").remove();
});
```

Full customization
------------------

You don't have to be restricted to the given theme. Flatdoc is just really one
`.js` file that expects 2 HTML elements (for *menu* and *content*). Start with
the blank template and customize as you see fit.

[Get blank template >][template]

Misc
====

Inspirations
------------

The following projects have inspired Flatdoc.

 * [Backbone.js] - Jeremy's projects have always adopted this "one page
 documentation" approach which I really love.

 * [Docco] - Jeremy's Docco introduced me to the world of literate programming,
 and side-by-side documentation in general.

 * [Stripe] - Flatdoc took inspiration on the look of their API documentation.

 * [DocumentUp] - This service has the same idea but does a hosted readme 
 parsing approach.

Attributions
------------

[Photo](http://www.flickr.com/photos/doug88888/2953428679/) taken from Flickr,
licensed under Creative Commons.

Acknowledgements
----------------

© 2013, 2014, Rico Sta. Cruz. Released under the [MIT 
License](http://www.opensource.org/licenses/mit-license.php).

**Flatdoc** is authored and maintained by [Rico Sta. Cruz][rsc] with help from its 
[contributors][c].

 * [My website](http://ricostacruz.com) (ricostacruz.com)
 * [Github](http://github.com/rstacruz) (@rstacruz)
 * [Twitter](http://twitter.com/rstacruz) (@rstacruz)

[rsc]: http://ricostacruz.com
[c]:   http://github.com/rstacruz/flatdoc/contributors

[GitHub API]: http://github.com/api
[marked]: https://github.com/chjj/marked
[Backbone.js]: http://backbonejs.org
[dox]: https://github.com/visionmedia/dox
[Stripe]: https://stripe.com/docs/api
[Docco]: http://jashkenas.github.com/docco
[GitHub pages]: https://pages.github.com
[fences]:https://help.github.com/articles/github-flavored-markdown#syntax-highlighting
[DocumentUp]: http://documentup.com

[project]: https://github.com/rstacruz/flatdoc
[template]: https://github.com/rstacruz/flatdoc/raw/gh-pages/templates/template.html
[blank]: https://github.com/rstacruz/flatdoc/raw/gh-pages/templates/blank.html
[dist]: https://github.com/rstacruz/flatdoc/tree/gh-pages/v/0.9.0
