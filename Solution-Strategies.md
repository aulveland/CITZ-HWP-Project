# Strategies 

Strategies are narratives that describe solution concepts of how specific **[Journeys](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/5.User-Journeys)** translate into **[features](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/7.Security)** as part of our solution design. 
They are based on our **[user research](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/3.User-Research)**. To implement our intended solution the HWP team has identified six feature groupings that require strategies to be documented.

* User
* Community
* Moderator
* Admin
* Search
* Notify

## User

A user is a platform member who requires an account, [logs on](https://user-images.githubusercontent.com/82344553/157935583-ab1b70db-121b-41b4-a3fb-575e594b6a00.png) with a valid identity, has a [profile](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/9.Wireframes#u1t4---profile), and can customize user preferences (settings). 
A user can join or leave a community. A user can create a topic (ie: a Post). Users can also comment on posts from other community members.  A user can flag a post or comment if they feel it is controversial. When a user logs into 'The neighbourhood' they will initially be a member of the 'welcome' community. Their "homepage" (also referred to as their 'dashboard') will display a 'header' region that contains the BC Government branding, a 'search' bar (see description below). Their profile avatar/icon and a menu icon. below the 'header' their screen is divided into two regions.
![a](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/9.Wireframes#u1t3---home)

On the right is a list of communities they have joined, while on the left is a list of all the postings they are subscribed to see and comment on.

## Community 

A community is a collection of users who share a common interest and can post topics and comments within their community. Communities can be created by users. Only Administrators can remove Communities.

## Moderator

A community-moderator is a community member who has been approved by the (system-)Administrator and can add/remove users to a community.

The community moderator features are displayed on the [Moderator](https://github.com/bcgov/CITZ-HybridWorkplace/blob/main/docs/moderatorPanel.png) page.

## Admin

A (system-)Administrator is a 'super'-user role who has the ability to add/remove users, promote [and remove] users to the community moderators role. 
An Administrator can adjudicate 'flagged' users and posts (ie: activate or remove a 'flagged' user or post. 

The Admin features are displayed by the [Admin](https://github.com/bcgov/CITZ-HybridWorkplace/blob/main/docs/AdminPanel.png) page.

## Search

The platform includes a search facility allows users to: 
* search all posts and comments based on key-word matches, if the user is not a member of the community that is matched they will have the ability to join the community
* search for user names within a community they are a member of [limited to that scope]

Search returns results in the Search Screen.

## Notify

The platform supports a notification facility allowing users to: 
* set a notify on/off option indicating that they wish to monitor a community for updates.
* a user has three options: 
     1. turn notification on/off
           - off = default 
           - on = a user will receive either a weekly or immediate update
     2. set a user-defined interval to receive a digest (default is a 7 day weekly).

Options to be considered to implement this feature includes [gcNotify](https://notification.canada.ca/) or the BCGov [CHES](https://digital.gov.bc.ca/common-components/common-hosted-email-service) common component.


The solution 'flow' has been documented [here](https://github.com/bcgov/CITZ-HybridWorkplace/wiki/9.Wireframes#flow-diagram).