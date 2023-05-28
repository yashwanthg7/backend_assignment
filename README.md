# backend_assignment
Assignment Instructions:
Backend Setup:
        a. Install the required dependencies, including bcrypt, MongoDB, cookie-parser ,dotenv and the jwt module.
 2.  Route Implementation:
       a. Create three routes: login, register, and /me.
      b. Implement the login route to handle user authentication. Use bcrypt to compare the password provided by the user during login.
      c. Develop the register route to handle user registration. Again, use bcrypt to hash the user's password before storing it in the database.
       d. Set up the /me route. This route will retrieve and display the details of the authenticated user.
3.  Middleware Implementation:
      a. Create a middleware function that checks for a token in the cookies section of the request(USE Cookie-parser first in the APP.js for using req.cookies).
      b. If a token is found, verify its authenticity using the jwt module.
      c. Once the token is successfully validated, store the user ID in the request object.
      d. Use the user ID to fetch all the user details from the MongoDB database.
4  Token Generation and Verification:
     a. When creating a token for a user, pass the user ID as a parameter to generate the token.
     b. During the verification process, the bcrypt module will return the user ID as the result.
      c. Save the user ID in the request object for further use in fetching user details from the database
