---
title: Google Analytics Pt.1
layout: post
---
# How Google Analytics Works (1.2)
In order to get data from a website, you need to create a Google Analytics account, and then insert a JS tracker into the HTML code. The code gets anonymous information about the user actions, as well as Lanuage, Type of broswer, device, OS, and traffic source (what brought them here.). 
GA tracks the user based on 'sessions' where you have GA not tracking after 30 minutes of inactivity. Of course you can have filters for geographic location, mobile vs. other users, etc. 
# The Analytics Account Structure (1.3)
Google accounts are (optionally) grouped under 'Organization'. Account creation then creates 'Property' which then has 'View'. You may have multiple properties per account ofc.
The multiple properties allow you to seperate your data. Ex: seperate properites for each state, or area. Since each account can have multiple properties, you can also have multiple views per property.
- For example if Google wanted to view All Data vs. NA vs. EU vs. Asia vs. internal data based on ID.
There's also something called goals, which will be talked about later on.

**Important** You can only recover views in 35 days if you delete them. Must be done by an admin of the account.

**_Note to reader_**  Here there's a demo section, where you can set up a Google Analytics account and install a code all in the tutorial

Under the Admin section, you can add more views, in order to test things. We created a Test View and filtered out bot traffic (under bot filtering). 
Creating another view is as simple as just saying "Copy View."
At this point it's important to note that the tutorial has made us create "Test View," "Raw Data," and "Master View." Raw data is what it sounds like: unfiltered, no bot traffic taken out. Test view has the bot traffic taken out. Then we copy Test view and call it Master View. 

If you have filters that you're using in the Test View (for example excluding internal traffic), you can apply it to Master View by actually just going to Filters ~> Apply Existing Filter. Remember **order of filters matter**.

[Link to the tutorial!](https://analytics.google.com/analytics/academy/)
