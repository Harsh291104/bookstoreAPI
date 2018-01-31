## Bookstore - Simple bookstore API exposing GET, PUT, POST, DELETE Operations using NodeJS, ExpressJS and MongoDB##

##Prerequisite
1.) Download code from repository.
2.) Install node JS - Configure Paths - Verify via running npm install app command on terminal.
3.) npm install express --save
4.) Install and configure MongoDB
   - create directories /data/db in your root folder and provides full executable permissions.
   - ./mongond - RUN Mongo daemon in one terminal
   - ./mongo   - RUN Mongo server in other terminal
   - mongoimport -d bookstore -c books books.json - Import books collection
   - mongoimport -d bookstore -c books genreSchema.json - Import genres collections

5.) node app - This will run the nodejs server on port 9090, ready to listen to request.
6.) Use any REST client Postman or RESTeasy  to issue GET, PUT, POST, DELETE requests on
   http://localhost:9090/api/books
   http://localhost:9090/api/genres
   http://localhost:9090/api/books/5a71b8866a2f4a334b0c7873 - Use id in the json object to delete and update books, genre collection


##DB commands used
use bookstore
db.createCollection('books')
db.createCollection('genres')
db.books.find()
