# Spotify Accounts Authentication Examples

Auth examples :

https://developer.spotify.com/web-api/authorization-guide/

* Authorization Code flow
* Client Credentials flow
* Implicit Grant flow

## Installation

Clone this repository and install its dependencies running:

    $ npm install

### Using your own credentials
You will need to register your app and get your own credentials from the Spotify for Developers Dashboard.

To do so, go to [your Spotify for Developers Dashboard](https://beta.developer.spotify.com/dashboard) and create your application. For the examples, we registered these Redirect URIs:

* http://localhost:8888 (needed for the implicit grant flow)
* http://localhost:8888/callback

Once you have created your app, replace the `client_id`, `redirect_uri` and `client_secret` in the examples with the ones you get from My Applications.

### Using `.env`
1) Install and import the dotenv package.
2) Save the Client_ID, Client_Secret, and Redirect_URI in to the `.env` file. 
3) Once save you can use the `process.env.{variable_name}` to access the variable
4) add `.env` to your `.gitignore` file.

## Running the examples
In order to run the different examples, open the folder with the name of the flow you want to try out, and run its `app.js` file. For instance, to run the Authorization Code example do:

    $ cd authorization_code
    $ node app.js

Then, open `http://localhost:8888` in a browser.
