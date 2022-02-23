# Security Table - Action vs Roles
This table defines the security access each roll has on the platform.  
  
### Legend
| Full Access | Partial Access |
| :---: | :---: |
| :heavy_check_mark: | :white_check_mark: |

Actions:
- things you can do (actions to take) in the platform  
  
Roles:
- User: General user of the platform (Actions the user can do while not inside communities)
- Member: User of the platform in a community
- Moderator: control and moderate users in specific communities
- System Admin: Responsible for upkeep of the platform
  
### Security Table

| Actions |  User  | Member | Moderator | System Admin |
| --- | :---: | :---: | :---: | :---: |
| U1T1 - Sign up | :heavy_check_mark: | | | |
| U1T4 - Log In/Off | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| U1T4 - Create Profile | :heavy_check_mark: |  | :heavy_check_mark: | |
| U1T3 - Edit Profile | :heavy_check_mark: |  | :heavy_check_mark: | |
| S1T9 - See List of All Users | | | :heavy_check_mark: | :heavy_check_mark: |
| U2T1 - See All Communities | :white_check_mark: | :white_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| U2T2 - Join Community | :heavy_check_mark: | | | |
| M1T9 - List All Community Members |  | | :heavy_check_mark: | :heavy_check_mark: |
| U2T4 - Search Communities | :heavy_check_mark: | :heavy_check_mark: | | |
| U2T13 - Propose Communities | :heavy_check_mark: | :heavy_check_mark: | | |
| S1T6 - Remove Community| | | | :heavy_check_mark: |
| S1T1 - Create Community| | | | :heavy_check_mark: |
| U2T5 - Post | | :heavy_check_mark: | :heavy_check_mark: | |
| U2T6 - Comment | | :heavy_check_mark: | :heavy_check_mark: | |
| U2T7 - Vote | | :heavy_check_mark: | :heavy_check_mark: | |
| M1T1 - Approve Posting | | | :heavy_check_mark: |  |
| M1T2 - Reject Posting| | | :heavy_check_mark: | |
| U2T8 - Set Notification Preference | :white_check_mark: | :heavy_check_mark: | :heavy_check_mark: | |
| U2T9 - Leave Community| | :heavy_check_mark: | | |
| U2T10 - Flag Posts | :heavy_check_mark: | :heavy_check_mark: | | |
| M1T5 - See All Flagged Posts| | | :heavy_check_mark: | :heavy_check_mark: |
| U2T11 - Edit post | :white_check_mark: | :white_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| U2T12 - Delete post | :white_check_mark: | :white_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| M1T3 - Approve Members to community | | | :heavy_check_mark: | :heavy_check_mark: |
| M1T4 - Remove Members from community | | | :heavy_check_mark: | :heavy_check_mark: |
| S1T2 - Assign  Moderators to community | | | | :heavy_check_mark: |
| S1T3 - Remove  Moderators from community | | | | :heavy_check_mark: |
| S1T4 - Approve Users| | | | :heavy_check_mark: |
| S1T5 - Remove Users| | | | :heavy_check_mark: |


## User Stories in relation to security
  
### User
**U1** - As a **user** I need to **register & login** to use the tool
1)	Sign up to create account
2)	Log in to create profile
3)	Log in to edit my profile
4)	Log in to see a list of all users  
  
  
**U2** - As a **user** I wish to participate in a **community**
1) Must be logged in to access communities
&nbsp; a. log in token
2)	See a list of communities  
&nbsp; b.       see list on homepage   
&nbsp; c.       tab or section listing all communities that can access any time
3) Search for community  
&nbsp; a. search by community name
4)	Join a community  
&nbsp; a. Approved by moderators  
&nbsp; b. Gain access to post comment and vote inside the community
5)	Propose a community  
&nbsp; a. Assured community doesn't already exist
&nbsp; b. Approved by moderator
6)	Leave a community  
&nbsp; a.	Existing posts are maintained because they have a thread associated with other users
7)	Make a posting as part of a community  
&nbsp; a. Notifies moderator so they can approve
&nbsp; b. part of a thread or standalone post
8)	Make comments on other people’s community postings
9)	Flag a posting as potentially inappropriate  
&nbsp; a.	Notifies the community moderator
10)	List all users in the community  
&nbsp; a. only seen by community members or only moderators
11)	Vote on a posting
12)	Vote on a comment
13) Choose notification preference  

### Moderator
 
**M1** - As a **community leader** I am required to provide **moderation** 
1)	Approve New users to a community
2)	Reject membership
3) Approve membership
4)	Reject postings  
5) Approve postings
6) Able to see list of all flagged posts
7) Delete posts once already been approved
  
### System Admin 
**S1** - As a **system admin** I provide **management** of the tool/system
1)	Approve creation of new communities
2)	Able to put a community on hold
3)	Able to remove communities
4)	Able to remove users
5)	Able to approve new users
6)	Able to back up the database
7)	Able to change profiles
8) Able to assign moderators
9) Able to remove moderators

