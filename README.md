# mvp

sign up / sign on page:
----------------------

    sign up:
      short description of the site and instructions to sign up/sign in below
     
      user enters username ------- valid  -------- user enters password ------- valid --------- home page
                          
                          
          user enters username   ------- username no entry ------ error and show message to enter a username
          user enters username  ------- username does not meet criteria ------- error and show message to enter a username
                          
          user enters password ------- password no entry ------- error and show message to enter password
          user enters password ------- password does not meet criteria -------- error and show message to enter password
          
          
    sign on: 
          user enters username ------- valid  -------- user enters password ------- valid --------- home page
          
          user enters username   ------- username no entry ------ error and show message to enter a username
          user enters username  ------- username not found ------- error and show message to enter a username
                          
          user enters password ------- password no entry ------- error and show message to enter password
          user enters password ------- password not found -------- error and show message to enter password
          
          
          
          
home page:  
---------
                 find shows:
                      http://eventful.com/events?q=music
                     search events by artist  http://eventful.com/events?q=music&
                     search events by date  http://eventful.com/events?q=music&l=San+Diego&t=9+December+2006
                     search events by location (zip code or city)  http://eventful.com/events?q=music&l=San+Diego
                     search similar events
                     
                  want to connect to other people?
                  
                   search users by name, saved events, groups user is a member of
                      keyword:  http://api.eventful.com/rest/users/search?...&keywords=eventor
                      username: http://api.eventful.com/rest/users/get?...&id=mruser
                      event attending:  
                        matches any user marked as "I'm going" to the event. For instance, going:chris_radcliff 
                        will find events attended by the user chris_radcliff.
                     
                     
                  click here to see/edit your events, groups, and profile --------- profile page
                     
                     
                     
profile page:
-----------         
                using oAuth key (which i have) users to see their eventful calendar and
                           edit their eventful profile through my app 

        1.    see calendar of events user plans on attending/has attended  
                http://api.eventful.com/rest/users/calendars/list?app_key=...&owner=eventor
        2.    see user's groups
                http://api.eventful.com/rest/users/groups/list?...&id=
                  
        3.       edit profile:  
                      edit name
                      add/remove location
                          http://api.eventful.com/rest/users/locales/add?...&id=eventor&locale=
                      add/remove evens user plans on attending 
                           http://api.eventful.com/rest/users/going/add?...&event_id=
                      
                      
          
                   
       Eventful supports oAuth 1.0 for Eventful API clients to access API resources on behalf of Eventful users.
Your application must first register as an oAuth consumer. To register an application, select [get oAuth consumer] for the 
application's key at API Application Keys. Your consumer key and consumer secret should be listed under your application 
key. You will need all three in order to use oAuth.

To access a user's protected resources, that user must first authorize your application. A "User" may be just your App 
trying to create events, upload images etc that needs authentication. In this case you'll just have to go through the 
process once and then you'll have your access token. In the case of your app wanting to login with real Eventful users 
you'll have to do the following once for every user that wants to be authenticated. The process of authorizing an 
application has three separate steps,

The application gets a request token.
The user authorizes the request token by logging into Eventful.
The application exchanges the request token for an access token.

The access token is all your application needs in order to access protected API resources. The access token will 
not automatically expire, but access can be revoked at any time by the user or Eventful. If the access token is 
revoked you may repeat the authorization steps to acquire a new access token.

        These endpoints handle the authorization process,

                Request Token
                POST http://eventful.com/oauth/request_token
                Authorize Request Token
                GET http://eventful.com/oauth/authorize
                Access Token
                POST http://eventful.com/oauth/access_token
                   
                   
                   
                

    
