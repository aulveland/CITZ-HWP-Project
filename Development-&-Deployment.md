# OpenShift Deployment
Follow the 2021 Capstone groups' deployment to the BC Government PaaS platform based on the RHEL OpenShift strategy.  
[How to Build and Deploy on Openshift](https://github.com/bcgov/citz-dst-capstone-2021/tree/main/openshift). Refer to the [challenges](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/Challenges#issue----how-to-learn-and-onboard-to-the-bcgov-paas-openshift-platform) page for more info.

## OpenShift Provisioning
Follow the request steps on the  BCDevExchange lab website [here](https://developer.gov.bc.ca/Getting-Started-on-the-DevOps-Platform/How-to-Request-a-New-OpenShift-Project)


# Local Deployment

1. Before running this code make sure to [clone](https://github.com/bcgov/CITZ-HybridWorkplace/fork) the latest version of this repository to your local machine. 
2. Clone the main branch to the local computer using git clone (you may need to download git to your computer for this to work).  
3. Make sure you have at least 500 MB to install.
4. Install [Node. JS](https://nodejs.org/en/) onto the local computer.
5. Install [MongoDB](https://www.mongodb.com/try/download/community ) onto the local computer.  
6. Once both are installed, you can start the steps to install. 

### Backend
Once in the CITZ-HybridWorkplace repository cloned on your local machine, navigate to the server directory in your terminal.  
  
`cd app/server`  
  
Install all the server-side dependencies  
  
`npm install`  
  
Wait for the dependencies to install then start the server.  
  
`node index.js` 
  

  
### Frontend

Open another terminal in the CITZ-HybridWorkplace repository.   
Navigate to the client directory. 
  
`cd app/client`
  
Install client-side dependencies.  
  
`npm install`  
  
Start running the client end  
  
`npm start`  
  
Open up a **Chrome** Browser to [http://localhost:3000/](http://localhost:3000/ )  
The website should now be running on this port.  
To debug redux, a google chrome extension has been added to the store.js file. To run on browsers that aren't google chrome, comment outline 36 of the store.js file.  
   
Then set up a branch for your changes   
git checkout  

