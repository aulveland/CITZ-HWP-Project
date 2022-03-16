**# CHALLENGE -  Users can subscribe for email digests of community posts that interest them**
## ISSUE -  How to trigger the Update Notification Frequency?

The user profile is stored in the Mongodb server. One setting is "**Update Notification Frequency**".  
We need to create some logic that polls the current time and checks the database in regular intervals for a match which triggers a buildEmailDigest function which tallies up how many posts were created in that time interval and packages them up and sends out a link to the subscriber letting them know
they then click that link to see their '**MyNewPosts**' page.

### investigate these links and topics
*  [Send and Schedule emails from a node.js app](https://blog.greenroots.info/send-and-schedule-e-mails-from-a-nodejs-app)
*  long polling in MERN
*  callbacks
*  socket.io 

**# CHALLENGE -  Hosting on OpenShift**
## ISSUE -  How to learn and onboard to the BCGov PaaS openShift Platform?

Currently for our solution we are developing on local machine and testing on Netlify. Our intended deployment path is to rehost on the BC Gov OpenShift platform.

### What will help us solve this challenge?
1. leverage the knowledge of in house staff (Poornima).

### investigate these links and topics

* [OpenShift Adoption](https://developer.gov.bc.ca/topic/featured/Service-Overview-for-BC-Government-Private-Cloud-as-a-ServiceOpenshift-4-Platform)
* [Developing for OpenShift](https://github.com/bcgov/CITZ-IMB-Capstone2020/blob/master/docs/Solution%20Readme.md#deploying-to-openshift)

**# CHALLENGE -  Using IDIR authentication**
## ISSUE -  How to integrate KeyCloak?

Currently in our solution we have a user sign on page that asks users for their user credentials which are stored in the user table of our mongodb . The password is bcrypt'd and we use JWTs for token based authorization. In our preferred Identity management system we wish to incorporate the BCGov KeyCloak standard.

### What will help us solve this challenge?

### investigate these links and topics
*  [developer.bcgov resources](https://developer.gov.bc.ca/Authentication-and-Authorization/Request-SSO-Client-Creation)
*  [Realm-o-matic](https://github.com/bcgov/realm-o-matic)