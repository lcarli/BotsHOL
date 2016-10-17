# Microsoft Bot Framework Demos #

<a name="Overview"></a>
## Overview ##
This is a set of demos showing how to interact with [Microsft Bot Framework](https://dev.botframework.com) creating your first bot.

<a id="goals" />
### Goals ###
In these demos, you will see how to:

1. Create your first bit using Visual Studio and [Bot Framework Template]("site")
2. Create a webapp on Azure to host your bot and how to deploy it.
3. Register your bot and publish it.

<a name="setup"></a>
### Setup and Configuration ###
Follow these steps to setup your environment for the demo.

1. Download the (Bot Framework]()
2. Download the [template]() for Visual Studio

<a name="Demo1"></a>
## Demo 1) Ceating your first bot using Visual Studio ##

1. Open Visual Studio 2015
2. Create a new project choose Bot Framework Template and click on it.

> **Speaking Points:** Explaint this project it is a WebAPI. It is build using ASP.NET.
>- Take time to explain the basic methods such as POST (receive message)
>- Also explain about libraries:
       
 * **POST** - The method receive a message from the channel where the client was chating
        * **Tip:** This method alredy cames with a countCaracters method and a response. Explore it with your audience.


<a name="Demo2"></a>
## Demo 2) Ceating a webapp to host your bot

1. Browse to the [Azure Portal](https://portal.azure.com)

2. Click New / Web + Mobile / Web App.

3. Enter a unique name in the URL field and click the Create button. This will be the url of your bot.

> **Speaking Points:** While the site is being created, explain that Azure is provisioning a new Web App for you with supporting services, monitoring, support for continuous deployment, etc.

>- Note: This generally takes 30 - 60 seconds.

4. When the site comes up, scroll through the various features (Monitoring, Usage, Operations, Deployment, Networking) explaining that these are all live and have been provisioned with the Web App. You can click on the _settings_ option to bring up the _settings_ blade.

> Note: If these tiles are not visible, you can add them by clicking on 'Add tiles' button and add Deployment, Operations, Usage etc.

5. Click on the Browse button. When the default landing page loads, point out that the page illustrates the different options for publishing to the new site, including Git, FTP, Visual Studio, etc.

6.  Back in the portal, Under 'General' option select 'Application settings'. Show that .NET, PHP, Python and Java are all show.


<a name="Demo3"></a>
## Demo 3) Registering your bot at Bot Framework Portal

1. Browse to the [Bot Framework Portal](https://dev.botframework.com/)

2. Click sign in at the top right

> Note: If you already logged in, you can skip this step.

3. Log with you LiveID (outlook, hotmail, live, msn, etc.)

4. Click in *Register a bot* to register a new bot

5. fulfill all data about your bot.
* Name: Displayed in Bot Directory. 35 character limit.
* Bot Handle: Used in the URL for your bot. *Alphanumeric and underscore only*. Cannot be changed once registered.
* Description: First 46 characters displayed on your bot card in Bot Directory. Full description displayed in bot details.

* Messaging endpoint: HTTPS Rest endpoint that the bot implements to send and receive messages.
- It will be your webapp previously created plus the route */api/messages/*
* Microsoft App ID: Get your Microsoft App ID and password from the Microsoft Application registration portal. Paste the password in your bot configuration file.
> *Note* - You have only one chance to see your Microsoft App Password. Save it in a safety place.

* Publisher name - Your name or your company name
* Publisher Email - Your Email or your commpany email
* Privacy statement - If you have one, paste url here. If don't, you can use that -> http://go.microsoft.com/fwlink/?linkid=521839
* Terms of Use - If you have one, paste url here. If don't, you can use tour website url
* Bot website - Url of your bot previously created
* Hashtags - Comma delimited.
* Languages - ISO 639-1 format, comma delimited.
* Default Conversation Language - The default language to use for new users.(in ISO 639-1 format)

6.  Accept Privacy statement, Terms of use, and Code of conduct. and click _Register_