# Planning Process
1. Idea
Community Library. People can list books to make them available to be shared with others. A borrowed book stays with the borrower until someone else wants it.

2. Write User Stories
As a user
- I can register for an account
    with name, contact information, password
- I can login

- I can browse a catalog of resources (without logging in)
- I can search the catalog (without logging in)
- I can view the details of a resource, including it's location (without logging in)

- I can request to borrow a resource (logged in)
- I can mark a request transaction completed when another user has picked up a resource that resided with me (logged in)
- I can make a resource available to the library by listing it in the catalogue (logged in)
- I can mark a resource that I have borrowed as available to the library again after reading it (logged in)

- I can message another user

3. User story nouns identify resources
- users
- resources
- request

4. Resources need tables -> ERD
- users: firstname, lastname, email, street address, how to contact me, password
- resources: isbn, title, author, description, cover-image, genre, current_possessor (userid), owner (userid), status (available/requested/in-use)
- requests: requester (userid), current_possessor (userid), resource, status (active/complete)

6. Routes

- GET  /        (home)
- GET  /login   (login form)
- POST /login
- POST /logout

- GET  /users/new          (show registration form)
- POST /users              (create user record)
- GET  /users/:id          (show profile)
- GET  /users/:id/requests (pull all requests for user)

- GET  /resources     (catalog)
- GET  /resources/:id (resource details)
- GET  /resources/new (show form to create resource/list book)
- POST /resources     (create resource record)
- PUT  /resources/:id (update / set status)

- GET  /requests/:id  (pull request by ID) 
- POST /requests      (create request record)
- PUT  /requests/:id  (update / mark completed)

7. Wireframes


================
- Meeting Times
- Tuesday:     5p/    8p/ 9:30p video
- Wed/Thur/Fri 5p/    8p/ 9:30p slack as needed
- Saturday: 1:30p/ 4:30p/ 6:00p video

- ERD (Johannes)
- Wireframes (Cherie/Merwyn)
- Git Repos (Merwyn)
  - Front end with planning directory
  - Database/API

- Think of name ideas
- Canva -> Logo?

