# URL_Shortener

URLs are the uniform resource locator and the URL shortener is the tool that converts the long and complex URLs into the shorter and more manageable link. These shortened URLs redirect the users to primary URLs when they access them. Short links save a lot of space when exhibited as they are small and clear. Also, it is difficult for users to mistype shorter links primary purpose of a URL shortener is to make links more concise, shareable, and easier to remember or type.
## 

This project uses the various npm packages from the npm registry which include 

express-backend web application framework for Node.js used for building web applications

mongoose-it is an asynchronous database driver, responsible for connecting to the database and performing query operations

short-id-this module creates user-friendly and unique ids for our URLs

nodemon-this package installed as a development dependency. It will constantly monitor our applications by automatically restarting the server when any file changes.

# Prerequisites

Installed node.js for the backend part of project 

generated the initial package : npm init

installed express mongoose ejs shortid: npm i express mongoose ejs shortid

Install nodemon as a dev dependency: npm i --save-dev nodemon

some large files are here-

# Getting Started 

To start the server we can go to package file and add script : "devStart": "nodemon server.js"

then to start the server command is: npm run devStart

# Internal Working 

Once the server is started, the backend starts working on the HTML main outline file using Bootstrap for the overall UI, including fonts, spacing, and colors. When a user inputs a URL to be shortened along with a corresponding note, a POST request is sent to the backend. The backend utilizes the shortid functionality to generate a shortened URL. It then adds the original URL, note, shortened URL, and the number of clicks to the MongoDB database. The updated data is displayed on the main webpage.

The number of clicks for each URL is also displayed on the homepage, and upon refreshing the page, any changes are reflected. The MongoDB database is properly set up and linked. To enable database functionality, a Schema object is created to define the structure of the data to be stored. Using mongoose.model(), a model is created based on the Schema object. This model allows for various database operations on the corresponding collection.

For implementing the search functionality, when text is entered in the search bar, the search request is processed. The find() function is then used to retrieve filtered data from the database. This function helps fetch the relevant data based on the provided search criteria. The search feature is applied to the fullurl, note, and shortUrl fields to provide user convenience.

By utilizing these components and functionalities, the backend efficiently handles URL shortening, data storage, retrieval, and search operations, providing a seamless user experience on the frontend.

# Lesson Learned 

Learned basics about HTML, Javascript, MongoDB, EJS, and most importantly Node.js and became familiar with Working with Bootstrap to implement the UI of the website. also know about Search functionality ,By learning to work with $regex operator of MongoDb and the find function.

# Resouces and Refrences Used

1.)HTML and CSStutorial :

(https://youtube.com/playlist?list=PL4cUxeGkcC9ivBf_eKCPIAYXWzLlPAm6G)

2.)JavaScript tutorial :

(https://youtu.be/W6NZfCO5SIk)

3.)Node.js and Express.js tutorial :

https://youtu.be/Oe421EPjeBE

4.)EJS tutorial :

https://www.youtube.com/watch?v=VM-2xSaDxJc

5.)MongoDB tutorial :

https://youtu.be/oSIv-E60NiU
