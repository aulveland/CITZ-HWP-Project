**# CHALLENGE -  Users can subscribe for email digests of community posts that interest them**
## ISSUE -  How to trigger the call back event?

The user profile is stored in the Mongodb server. One setting is "**Update Notification Frequency**".  
We need to create some logic that polls the current time and checks the database in regular intervals for a match which triggers a buildEmailDigest function which tallies up how many posts were created in that time interval and packages them up and sends out a link to the subscriber letting them know
they then click that link to see their '**MyNewPosts**' page.

### What will help us solve this challenge?

### investigate these links and topics
*  [Send and Schedule emails from a node.js app](https://blog.greenroots.info/send-and-schedule-e-mails-from-a-nodejs-app)
*  long polling in MERN
*  callbacks
*  socket.io 

**# CHALLENGE -  Using IDIR authentication**
## ISSUE -  How to integrate KeyCloak?

Currently in our solution we have a user sign on page that asks users for their user credentials which are stored in the user table of our mongodb . The password is bcrypt'd and we use JWTs for token based authorization. In our preferred Identity management system we wish to incorporate the BCGov KeyCloak standard.

### What will help us solve this challenge?

### investigate these links and topics
*  [developer.bcgov resources](https://developer.gov.bc.ca/Authentication-and-Authorization/Request-SSO-Client-Creation)
*  [Realm-o-matic](https://github.com/bcgov/realm-o-matic)