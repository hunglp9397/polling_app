#  An Overview of the security mechanism

* Build an API that registers new users with their name, username, email and password.

* Build an API to let users log in using their username/email and password. After validating user’s credentials, the API should generate a JWT authentication token and return the token in the response.

* The clients will send this JWT token in the Authorization header of all the requests to access any protected resources.

* Configure Spring security to restrict access to protected resources. For example,

* APIs for login, signup, and any static resources like images, scripts and stylesheets should be accessible to everyone.

* APIs to create a poll, vote to a poll etc, should be accessible to authenticated users only.

* Configure Spring security to throw a 401 unauthorized error if a client tries to access a protected resource without a valid JWT token.

* Configure Role-based Authorization to protect resources on the server. For example -

* Only users with role ADMIN can create a Poll (Note that, The demo project that is available on Github doesn’t require ADMIN role for creating a Poll, but you can easily change this behavior).
* Only users with role USER can vote in a Poll.
