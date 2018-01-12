# Station - vSend for Desktop
# Plan
Email marketing is a useful way for businesses and individuals to keep in contact with one another. 
Businesses may join our platform and cost-effectively broadcast newsletters to their network.
Some tools we will offer marketers are:
## Campaigns

```
	|_______Distribute Mass Email (Q1)	
			|_______Upload your contacts list (free)
			|_______Verify your contacts list for Bounces and or Non-existent addresses (Paid)
			|_______Create Responsive Newsletter Templates (freemium)
			|_______Create Responsive Landing Page Templates (freemium)
			|_______Send Mass Email on Schedule (freemium)
			|_______Manage/Add contacts with API (Paid)
```


## Integrations

```
	|_______Web (Q2)
		|_______Zapier App
				|_______Zapier integrates API to API automation with ease, using Zapier our platform will be nearly cross-compatible with all browsers, and most public web platforms and business applications such as Gmail, Hubspot, Google Sheets and much more.

	|_______API (Q1)
		|_______Users (protected)
				|_______Hooks
				|_______Updates
		|_______Contacts (public)
				|_______Hooks
				|_______Updates
		|_______Campaigns (public)
				|_______Hooks
				|_______Updates
		|_______Automations (public)
				|_______Hooks
				|_______Updates
		|_______Custom Integration (public)
				|_______Agency can add custom routes (Q3)


	|_______CLI (Q1)
		|_______Initiate the project (SAAS)
		|_______Integrate API or Forms in your Web App
		|_______Manage Agency or Team

	|_______Mobile (Q2)
		|_______Manage, and Schedule Campaigns
		|_______Manage Contacts
		|_______Review Campaigns and Automations
```

## Social Media

```
 |_______Authenticate with Social Networks (Q2)
				|_______Upload your Contacts List, compare to see who follows you on Facebook, Instagram, or Twitter
				|_______Broadcast a link to a Campaign on your Social Channels as soon as it's published. 
				|_______Message Users on your behalf 
				|_______Message Group on your behalf
```

## SMS

```
 |_______Authenticate with Cell Phone (Q3)
 		 |_______Deliver Mass Text Messages 
 		 |_______Deliver Mass MMS Messages
 		 |_______Use Twilio (or competitive PAAS)
```

## Automations

```
	|_______Configure Automated Marketing Campaigns (Q1)
			|_______Schedule CRON for future campaign distributions 
			|_______Mainly UI, as most of the functionality will be present
			|_______Append multiple newsletters to one chain/trail/thread
			|_______Delivery proceeds in preferred order by: 
					|_______Maybe another option to base off of Open/Clicked on Timestamp 
					   (I.E, Email is opened... Then wait 10 mins, and continue delivery with next message. 
					   Or Email is clicked.. Then wait 24 hours, and deliver next scheduled message.)
						-Opened or Has Not Opened
						-Clicked or Has Not Clicked
```


# Structure
Laravel 5.1 backend with Laravel Spark for SAAS
Researching multiple views at the moment.
View will be encapsulated in Electron, with multiple frameworks carried in through Node integrations. 
View is based in VueJS and Handlebars. With a flexible and reusable code-base of Laravel we may integrate nearly any view within our application.

## Design
SAAS memberships offered to business owners and agencies who will create teams of users with different usage limitations.
Core users will look like this:

```
Agency Manager
or
Team Manager ______
				  |___Team Members(s)
			  		  |___Per User Usage Limitations
			  		  |___Per User Profile
			  		  |___Per User Storage
			  		  		|___Per User Campaigns
			  		  		|___Per User Automations
			  		  		|___Per User Templates
			  		  		|___Per User Contacts
```

## Research
Statistics, extrapolations and counting by Radicati Group from February 2015 estimate the number of emails sent per day (in 2015) to be around 205 billion. 205 billion email messages per day means almost 2.4 million emails are sent every second and some 74 trillion emails are sent per year. 

## Revenue indicators : https://blog.mailchimp.com/going-freemium-one-year-later/
### Paying Customers in Sep 2010
 Sept 2009 - 85,000 customers
 Sept 2010 - 212,500 customer {stated in blog that 'the number of paying customers has increased over 150%'}

### Ben Chestnut states that '20% of our users have lists greater than 10k subscribers'
 20% * 212,500 = 45,500 customers with >10K subscribers
 ARPU of those customers = $195 / month*

### Cost analysis in the PAAS market proves multiple competing services are offered to SAAS providers. 
### Some of the most well known providers on the PAAS level are:
Amazon SES
Sendgrid
Elastic Email


### Legality: https://www.ftc.gov/tips-advice/business-center/guidance/can-spam-act-compliance-guide-business
The CAN-SPAM Act, a law that sets the rules for commercial email, establishes requirements for commercial messages, gives recipients the right to have you stop emailing them, and spells out tough penalties for violations. ... The law makes no exception for business-to-business email. 

Each separate email in violation of the CAN-SPAM Act is subject to penalties of up to $40,654, so non-compliance can be costly. But following the law isn’t complicated. Here’s a rundown of CAN-SPAM’s main requirements:

Don’t use false or misleading header information. Your “From,” “To,” “Reply-To,” and routing information – including the originating domain name and email address – must be accurate and identify the person or business who initiated the message.
Don’t use deceptive subject lines. The subject line must accurately reflect the content of the message.
Identify the message as an ad. The law gives you a lot of leeway in how to do this, but you must disclose clearly and conspicuously that your message is an advertisement.
Tell recipients where you’re located. Your message must include your valid physical postal address. This can be your current street address, a post office box you’ve registered with the U.S. Postal Service, or a private mailbox you’ve registered with a commercial mail receiving agency established under Postal Service regulations.
Tell recipients how to opt out of receiving future email from you. Your message must include a clear and conspicuous explanation of how the recipient can opt out of getting email from you in the future. Craft the notice in a way that’s easy for an ordinary person to recognize, read, and understand. Creative use of type size, color, and location can improve clarity. Give a return email address or another easy Internet-based way to allow people to communicate their choice to you. You may create a menu to allow a recipient to opt out of certain types of messages, but you must include the option to stop all commercial messages from you. Make sure your spam filter doesn’t block these opt-out requests.
Honor opt-out requests promptly. Any opt-out mechanism you offer must be able to process opt-out requests for at least 30 days after you send your message. You must honor a recipient’s opt-out request within 10 business days. You can’t charge a fee, require the recipient to give you any personally identifying information beyond an email address, or make the recipient take any step other than sending a reply email or visiting a single page on an Internet website as a condition for honoring an opt-out request. Once people have told you they don’t want to receive more messages from you, you can’t sell or transfer their email addresses, even in the form of a mailing list. The only exception is that you may transfer the addresses to a company you’ve hired to help you comply with the CAN-SPAM Act.
Monitor what others are doing on your behalf. The law makes clear that even if you hire another company to handle your email marketing, you can’t contract away your legal responsibility to comply with the law. Both the company whose product is promoted in the message and the company that actually sends the message may be held legally responsible.
