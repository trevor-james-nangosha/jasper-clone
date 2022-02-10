***Design/ implement a web based system for sharing files and chat messages***

#### KEY AREAS BEING TESTED
status codes
serving static files using express
handle download functionality
using the CRUD operations in a mongoDB app
sessions and cookies
realtime chats using sockets

#### IMPORTANT EXPRESSJS LIBRARIES TO INSTALL
mongoose for mongDB
nodemon for instant server restart
redis
postman is used for building APIs
multer is used for handling the file uploads and downloads
socket.io for real time communication betweeen the server and client
uuid for the user IDs
express-session for handling the user sessions
express-validate for handling the user validation
moment.js for date and time formatting
jquery, for some common vanillaJS functionality

#### THE SYSTEM SHOULD HAVE (BUT NOT LIMITED TO) THESE FEATURES
the users of the system must have user accounts in the system
the users must login to the system before they can begin sharing files
after logging in with their credentials, they must be on something like a dashboard
the users can select the files from their hard drive or other devices connected to the computer they are currently 
working with
obviously the user accounts call for something like mongDB to store user credentials
i will prefer to use a minimalist design for my applications which for the start will have only
two pages the login page and the dashboard page
each user must have their own dashboard
for now we shall consider a connection between only two users
we shall consider that the two users run on a single server instance
use sessions and cookies for identifying users across sessions and storing user data

#### THE FOLLLOWING ARE THE DIFFERENT FOLDERS AND WHAT THEY DO
config, is where we have our database connection configurations hence the name
routes, is where we have the different routes
controllers, the routing  logic
public, is where we have our static assets
index.js, that is our main file
models, is where we have our database structure like defining the schemas
views, this folder has our JADE templates for our web views

#### IMPORTANT NOTES
in case the page is taking forever to long. use res.send instead of console.log
you should always use sessions and cookies
i finally found out what "redis" and "memcache" for - it uses memory cache because it provides a better way of storing user data and sessions
redis is seperated from your application server and hence reduces dependency

websites do not store the user data and hence they use session cookies to store the data
 
#### NOTES FROM THE BOOK CLEAN CODE BY ROBERT C. MARTIN
good code should have complete error handling
i think java and its class design principles make a good way f defining good APIs, through its use of private and public methods
good code should be minimal
