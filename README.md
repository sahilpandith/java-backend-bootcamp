# java-backend-bootcamp

# how rest API Flow


                                Broswer
                                    |
                                    |
                                -----------
                                |          |
                                |          |
                               CDN       Backend
                                           |
                                           |
                                         Database


When we load an url in a browser, Browers makes a call to DNS with url, DNS has the IP mapping for the URL. DNS identifes the edge server and makes the resquest for the static assests.

Now, if edge server has the requested reosurces caches, it will sens the resources to the browser. But , In case the cache is expired or invalid for some resason, Edge server will make a request to the origin server and the get the valid resource and send it back to the browser.

Browser loads those resources, Now the browser will make API call to the backend to get the dynamic content.

The API request will contain some information as follows

1. protocol
2. header
3. data
4. cookies
5. and some other data

Upon recieving the request, backend will process the request as follows

1. parse data
2. based on data make a DB call and get the relevant data
3. structure that data in JSON format
4. send that as a response

Browser will get that response and load the data

# git workflow

In order to contribute to an open source repo

1. First fork the repo
2. Make a local copy
3. Make changes
4. push changes
5. Make a pull request







