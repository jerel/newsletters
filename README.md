
## Newsletters

The PyroCMS Newsletter module allows you to create email "blasts" to send to your email newsletter subscribers.

#### What does it do?

Add a subscribe form (widget included) to your website and start an email newsletter! Comes with 4 email templates 
to get you started and has extremely flexible send options. Administrators can send emails using a browser or schedule 
a cron job to make it automatic at a specified time each hour/day/week. Generates email open statistics and allows 
you to track the number of clicks on links embedded in the newsletter. Edit the newsletters and insert images using 
the familiar WYSIWYG editor.

#### History and License

This module was included in PyroCMS Professional until version 2.1 and sold on the PyroCMS add-on store. I've now 
pulled it out of the core of PyroCMS and licensed it under the Apache 2 license.

#### Development and Support

Your pull requests, translations, and updates for new PyroCMS versions are all welcome! If you find a problem 
with the module please create a new Issue here on Github.

#### Subscribers
To collect email addresses use the Newsletter Subscribe widget or create a Navigation link to http://example.com/newsletters/subscribe

#### Creating the Newsletter
###### Templates
Select a predefined template from the dropdown box. If you would like to edit a default template you may do so in the Template Manager. Note: the template cannot be changed when editing an existing newsletter. Choose the template carefully when creating a new newsletter.

###### Newsletter Subject
The Newsletter Subject will show in the recipient's email subject line and will have the site name + Newsletter appended to it. Example subject line: v2.0 will be released on 01/01/2015! | Acme Software Newsletter

###### Tracking Newsletter Opens
If this option is selected the newsletter module will add an invisible tracking image to the email. This is used in combination with Tracked URLs to generate statistics. This will not work if you are sending plain text emails.

###### Tracking URLs
If you want to place links in the email and track the recipient's clicks simply put the web address in the Target URL box and a unique link will be generated. Copy & Paste the generated link into the email body and it will be tracked. This works in html emails & plain text emails. You can test your links from the View page after the newsletter has been saved.

###### The Email Body
Creating a newsletter is very similar to creating page content. Use the WYSIWYG editor to generate the html that will be used in the email. You may insert images into the email like you would in page content. When the newsletter is sent the image links will be changed to absolute links so they can be read from any email client. The images are not actually sent in the email, the email just links to your server. Consequently you must not delete the images until you believe that all recipients have finished reading the email.

#### Sending the Newsletter
###### Send All
The way you send the newsletter depends on the Settings for this module. If the Email Limit is set to 0 the link will display as "Send All" and the Newsletter Module will send 50 emails at a time until all emails are successfully sent or the page is closed.

###### Send Batch
If you set the Email Limit to a number greater than 0 the link will display as "Send Batch" and only that number of emails will send. You will have to click the link again to send the next batch. This feature allows you to send newsletters (slowly) even if your host limits the number of emails you can send per day or per hour.

###### Send Cron
If you select Enable Cron in Settings the link will display as "Send Cron". When you click the link it will simply mark the newsletter as "ready" and it will be sent with the next cron job. The Email limit can be set or you may leave it as 0 to send all emails at once. If have a cron job that runs at midnight and the limit is less than your number of subscribers it may take a couple nights to send all emails. To send newsletters with cron load http://yoursite.com/newsletters/cron/gy84kn


#### Translators

* [Marco Grüter](https://github.com/marcogrueter)
* [Christian Giupponi](https://github.com/ChristianGiupponi)
