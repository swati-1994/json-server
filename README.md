The Node module, json-server, provides a very simple way to set up a web server that supports a full-fledged REST API server.

json-server is a node module, and hence can be installed globally by typing the following at the command prompt
#  npm install json-server -g

create a folder named json-server and add the json files with .json extension.

Type the following at the command prompt to start the server(-d is used for delay, here delay is of 2secs)
# json-server --watch db.json -p 3001 -d 2000

This should start up a server at port number 3001 on your machine. The data from this server can be accessed by typing the following addresses into your browser address bar:

# http://localhost:3001/dishes
# http://localhost:3001/promotions
# http://localhost:3001/leaders
# http://localhost:3001/feedback

The json-server also provides a static web server. Any resources that you put in a folder named public in the json-server folder above, will be served by the server at the following address:

# http://localhost:3001/
