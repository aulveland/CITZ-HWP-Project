[HWP Data Models](https://github.com/bcgov/CITZ-HybridWorkplace/tree/main/app/server/models)

## User

const User = new mongoose.Schema(
	{
		name: { type: String, required: true, unique: true },
		email: { type: String, required: true, unique: true },
		password: { type: String, required: true },
		fullName: {type: String},
		title: {type: String},
		bio: {type: String},
		darkMode: {type: Boolean},
		communities: [{
			type: mongoose.Schema.Types.ObjectId,
			ref: 'Communities'}],
	},
	{ collection: 'user-data' }
)

const model = mongoose.model('UserData', User)




[data modeling ](https://www.mongodb.com/docs/manual/core/data-modeling-introduction/#:~:text=MongoDB%20documents%20make%20it%20possible,denormalized%20data%20model%20is%20optimal.).