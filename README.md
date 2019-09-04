# Assignment 1 3813ICT
### Developed by Taylor Hannan

## Angular Architecture
### Components
There are four components, as follows:

#### Home Component

This component is responsible for the user's login.

#### Nav Component
The navigation component is a static component that controls the routing of home, chat, and admin components.

#### Chat Component
Chat page but not necessary

#### Admin Component

This component hosts the management dashboard. Superadmin users can add and delete users on this page, and can also add and delete groups.


## User Routes
#### /api/auth
"Auth" routing is used to authorize users at login time. It is achieved by obtaining the parameter * username * & password * from the login form on the home page. 

#### /api/reg
This route is used to manage user registration. It does so by taking the following parameters entered on the user registration form on the AdminComponent: *username*,  *email*, and *role*. 

#### /api/del
This route is used to delete the user's data in the check form. It exists in userdata.json. If it matches, it can be deleted.

#### /api/users
This route is for the past user to be from userdata.jason. This route does not require special parameters. It only needs to send a request to return user data.

## Group Routes
#### /api/groupreg
This routing user adds a user group. Enter the name of the input in the form into groupdata.jason and save it.

#### /api/groupdel
This routing user deletes the user group. Whether the input in the check form matches, if it matches, it can be deleted.

#### /api/groups
This route user reads the data in groupdata.
This route requires no special parameters, only a request to be sent to it for it to return the user data.
