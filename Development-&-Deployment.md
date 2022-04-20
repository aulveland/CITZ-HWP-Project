# OpenShift Deployment
Follow the 2021 Capstone groups' deployment to the BC Governments PaaS platform based on RHEL OpenShift strategy.  
[How to Build and Deploy on Openshift](https://github.com/bcgov/citz-dst-capstone-2021/tree/main/openshift). Refer to the [challenges](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/Challenges#issue----how-to-learn-and-onboard-to-the-bcgov-paas-openshift-platform) page for more info.

## OpenShift Provisioning
Follow the request steps on the  BCDevExchange lab web site [here](https://developer.gov.bc.ca/Getting-Started-on-the-DevOps-Platform/How-to-Request-a-New-OpenShift-Project)


# Local Deployment

Before running this code make sure to clone the latest version of this repository to your local machine. 
Clone the main branch to local computer using git clone (you may need to download git to your computer for this to work. )  

First Install NodeJS on local computer https://nodejs.org/en/  
Then install mondoDB onto local computer https://www.mongodb.com/try/download/community  
once both are installed, you can start the steps to install. 

### Backend
once in the CITZ-HybridWorkplace repository cloned on your local machine, navigate to the server directory in your terminal.  
  
`cd app/server`  
  
Install all the server side dependencies  
  
`npm install`  
  
Wait for the dependencies to install then start the server.  
  
`nodemon index.js` 
  

  
### Frontend

Open another terminal in the CITZ-HybridWorkplace repository.   
Navigate to the client directory. 
  
`cd app/client`
  
Install client side dependencies.  
  
`npm install`  
  
Start running the client end  
  
`npm start`  
  
Open up a **Chrome** Browser to [http://localhost:3000/](http://localhost:3000/ )  
The website should now be running on this port.  
To debug redux, a google chrome extension has been added to the store.js file. To run on browsers that aren't google chrome, comment out line 36 of the store.js file.
  

# Other Deployment
### Netlify *Blocked* 
  
To deploy to Netlify we would either need to deploy to Heroku for the backend or add new library and code implementation. For our project scope, this is too complicated and will take too much time away from our development build so this step is currently blocked. Few [articles](https://stephencook.dev/blog/netlify-mongodb/) are available to describe this process.