# DynamoDB-Rest-Server 
Generic Pluggable DynamoDB REST API with user auth, creation, update & delete functionality.

JWT integrated.

### Development

- Clone Repo:  `git clone https://github.com/mnoster/DynamoDB-Rest-Server.git`

- Add your AWS credentials to `config/connect.config.json`
 
- Create DynamoDB table called 'Users'
 
- Add columns to your table as specified below

- Start node server: `npm start`


___

### DynamoDB schema

#### Table Name: Users

#### Table Columns: email, password, first_name, last_name, date
   - email field is the primary key

___

#### Endpoints

- /user_authentication
- /user_create
- /user_update 
- /user_get
- /user_update
- /logout

#### Request Headers
- x-access-token : 'json web token here'
- Content-Type : application/json


#### Middleware
- VerifyToken (JWT check)

#### uses jwt session
#### uses bcrypt password protection








