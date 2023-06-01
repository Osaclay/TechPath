TECHPATH
TechPath, a roadmap for the tech ecosystem, offers professional and specialized guidance for individuals looking to advance or venture into any tech related career discipline. 
Our minimum viable product includes the following features:
Information Content: High quality and up-to-date information content on tech careers and how to break into them.
Job Listings: Job board that aggregate current job listings from various tech related sources.
Career Guidance: Offer personalized career guidance to visitors through chatbot and live chat.
Networking Opportunities: Networking opportunity for both experts in the field and newcomers. 


ALX FOUNDATIONS PROTFOLIO PROJECT

Author
Osamede Osunde - Github / Email
 

Architecture

In the diagram below, the user’s web browser communicates with the load balancer (acting as reverse proxy server) that distributes incoming requests to two web servers. The load balancer also communicates with the firewall to ensure the security of the system. The web servers communicate with the application servers, which runs the portfolio application. The application server communicates with the database servers that store user data. 
Additionally, the cloud storage is used to store files and other data related to portfolio entries, such as images or videos.

APIs

APIs and Methods:

API routes for web client to communicate with the web server:

/api/user
GET: Returns the user’s information based on session id.
PUT: Updates the user’s information based on session id.
/api/job_search
POST: Returns jobs matching the parameters through a third-party job search API like Indeed, Monster, Zipcruiter or Greenhouse.
/api/chatbot
POST: Sends user input to a machine learning chatbot API like Dialiogflow and returns a response.


API endpoints or functions/methods to allow other clients to use:

searchJobs(location, keywords)
Returns a list of job results based on location and keywords. 
getUserProfile(userId)
Returns the user’s profile information based on their user id.
getChatbotResponse(inputText)
Sends input text to a chatbot API and returns the chatbot’s response.

3rd party APIs that will be used:
Google Maps API
Provides geocoding and reverse geocoding services to determine locations based on addresses or vice versa.
Indeed Job Search API
Provides job search and listing services for employers and job seekers.


Data Modelling


User Stories
As a newcomer to the tech industry, I want to be able to browse a variety of topics related to tech and learn from experts in the field.
As an industry expert, I want to be able to share my knowledge and expertise with others in the tech community and engage in discussions on the latest trends and advancements.
As a registered user, I want to be able to create and edit my own profile, including adding a profile picture and bio, to better connect with other members of the community.
As a forum member, I want to be able to post questions and receive answers from other members of the community, as well as search for answers to questions that have already been asked.
As a regular user of the site, I want to be able to receive notifications when new content is added to topics I'm interested in or when someone replies to a thread I've participated in.
As a newcomer to the tech industry, I want to be able to browse a list of recommended resources, including books, courses, and tools, to help me learn and grow in my field.
As an industry expert, I want to be able to post articles and tutorials on the site to share my knowledge and experience with others in the community.
As a forum member, I want to be able to upvote or downvote posts and replies to help identify the most helpful or relevant content.
As a user, I want to be able to report inappropriate content or behavior to the site moderators to help maintain a safe and respectful community.
As a regular user, I want to be able to easily navigate the site and find the information I need, including search functionality and clear categorization of content.

