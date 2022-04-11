[HWP Data Models](https://github.com/bcgov/CITZ-HybridWorkplace/tree/main/app/server/models)

## User


const model = mongoose.model('UserData', User)

## Community

 const Community = new mongoose.Schema(

     {
         title: { type: String, required: true, unique: true},

         description: { type: String},

         creator: { type: String},

         members: [{ 

             type: mongoose.Schema.Types.ObjectId,

            ref: 'User'

            }],
     },
     { collection: 'community-data' }
 )
 
 const model = mongoose.model('CommunityData', Community)


[data modeling ](https://www.mongodb.com/docs/manual/core/data-modeling-introduction/#:~:text=MongoDB%20documents%20make%20it%20possible,denormalized%20data%20model%20is%20optimal.).