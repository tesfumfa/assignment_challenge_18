# assignment_challenge_18
<h1>Table of Contents:</h1>
<ul>
 <li> <a href="">User Story </a></li>
<li><a href="">Acceptance Criteria</a></li>
<li><a href="">Description</a></li>
<li><a href="">Mock-Up</a></li>
<li><a href="">API Tests</a></li>
 <li><a href="">Submission</a></li>
</ul>
<h2> User Story</h2>
<p>AS A social media startup<br/>
I WANT an API for my social network that uses a NoSQL database<br/>
SO THAT my website can handle large amounts of unstructured data</p>
<h2>Acceptance Criteria</h2>
<p>GIVEN a social network API<br/>
WHEN I enter the command to invoke the application<br/>
THEN my server is started and the Mongoose models are synced to the MongoDB database<br/>
WHEN I open API GET routes in Insomnia for users and thoughts<br/>
THEN the data for each of these routes is displayed in a formatted JSON<br/>
WHEN I test API POST, PUT, and DELETE routes in Insomnia<br/>
THEN I am able to successfully create, update, and delete users and thoughts in my database<br/>
WHEN I test API POST and DELETE routes in Insomnia<br/>
THEN I am able to successfully create and delete reactions to thoughts and add and remove friends to a user’s <br/>friend list</p>
<h2>Description:</h2>
<p>This is a set of API for a social network that uses a MongoDB database so that the website can handle large amounts of unstructured data, Express.js for routing, Mongoose ODM, and the moment package to format time stamps.</p>
<h2>Mock-Up</h2>
<ul>
  <li><a href=""> User Routes</a></li>
  <li><a href=""> Thought Routes</a></li>
  <li><a href=""> Friend Routes</a></li>
  <li><a href=""> Reaction Routes</a></li>
  <li><a href="https://youtu.be/5efi7Sq9iQU"> Walkthrough Videos All in One:</a>&nbsp;https://youtu.be/5efi7Sq9iQU</li> 
</ul>
<h2>API Tests</h2>
<h3>Testing restful API calls with Insomnia Core and Rest client</h3>
<p>/api/users</p>
<ul><li>GET all users</li>
<li>POST a new user: <br/>
         
         {
 
           "username": "daniel",</br>
	          "email": "daniel@yahoo.com"
            
         }

 </li></ul>
 <p>/api/users/:userid</p>
 <ul><li>GET a single user by its _id</li>
<li>PUT to update a user by its _id</li>
<li>DELETE to remove user by its _id</li></ul>
<p>/api/users/:userId/friends/:friendId</p>
<ul><li>POST to add a new friend to a user's friend list</li>
<li>DELETE to remove a friend from a user's friend list</li></ul>
<p>/api/thoughts</p>
<ul><li>GET to get all thoughts</li>
<li>POST to create a new thought</li><br>

 {  
     "thoughtText": "how are you  dawit",<br>
	  	"username": "dawit",<br>
		  "userId":  "61c691144046d926ef0e3c46"
	  
 }
</ul>
<p>/api/thoughts/:thoughtId</p>
 <ul><li>GET to get a single thought by its _id</li>
<li>PUT to update a thought by its _id</li>
<li>DELETE to remove a thought by its _id</li></ul>
<p>/api/thoughts/:thoughtId/reactions</p>
<ul><li>POST to create a reaction</li><br>
 // Example json data<br>
    {
    
     "reactionBody":"hallow  alexander!!",<br>
     "username":"alexander"
 
    }

</ul>
<p>/api/thoughts/:thoughtId/reactions/:reactionId</p>
<ul><li>DELETE remove a reaction by the reactionId</li></ul>
<h2>Submission:</h2>
<a href="https://github.com/tesfumfa/assignment_challenge_18">Github repository</a>





 

