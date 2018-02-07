# mvp

SIGN UP/SIGN ON/LANDING PAGE:
----------------------

      short description of the site and instructions to sign up/sign in below

    CONTINUE AS GUEST ————————————————————————————————— direct to home page                    
                     
    SIGN UP:
  
        user enters username   ------- username no entry ------ error and show message to enter a username
        user enters username  ------- username does not meet criteria ------- error and show message to enter a 																                            valid username
                      
        user enters password ------- password no entry ------- error and show message to enter password
        user enters password ------- password does not meet criteria -------- error and show message to enter 
                                                                                a valid password
    -------     -------     -------     -------     -------     -------     -------     -------
    user enters username ------- valid ——— user enters password  ——— valid —— continue to home page    
    -------     -------     -------     -------     -------     -------     -------     -------   
 
    SIGN ON:
           
      user enters username   ------- username no entry ------ error and show message to enter a username
      user enters username  ------- username not found ------- error and show message to enter a username
                      
      user enters password ------- password no entry ------- error and show message to enter password
      user enters password ------- password not found -------- error and show message to enter password
      
   -------      -------     -------         -------     -------     -------     -------     -------
    user enters username ------- valid  -------- user enters password ------- valid --------- home page
   -------      -------     -------     -------     -------     -------     -------     -------     -------             

          

HOME PAGE:
  
        event search:
              
                 search events by artist  http://eventful.com/events?q=music&
                 search events by date  http://eventful.com/events?q=music&l=San+Diego&t=9+December+2006
                 search events by location (zip code or city)  http://eventful.com/events?q=music&l=San+Diego
                 search similar events

                
        user search  ————— redirect to social page             
              
        click here to see/edit your username, password or delete your profile — redirects to profile page

        click here to edit your calendar ———— redirect to social page



PROFILE PAGE:
                             
       edit profile:  edit username ----- username no entry ------- error and show message to enter username
       			            ----- username does not meet criteria -------- error and show message to enter 
                                                                                	a valid username
											
		      edit password ----- password no entry ------- error and show message to enter password
        			    ----- password does not meet criteria -------- error and show message to enter 
                                                                                	a valid password
											
		      delete profile  -----  profile delete
					
       to edit calendar  ——— redirect to social page
       to search user    --- redirect to social page
				
                  		

SOCIAL PAGE:

      user enters eventful credentials
                    user name —— if null —- error message to enter a username
		    password ——- if null —- error message to enter a password

		    username —— if invalid  —  error message “not found. enter a valid username”
		    password —— if invalid —- error message “password incorrect.  enter a valid password”

		    username — if valid — enter password
		    password — if valid — continue to social page
       ____________________________________________________________________________________________

      user search  ——  

		1.  search by username
		2.  search by events attending
	
      edit my calendar  ———

     	1.    see my events
            http://api.eventful.com/rest/users/calendars/list?app_key=...&owner=eventor
   	2.    edit my groups
            http://api.eventful.com/rest/users/groups/list?...&id=
    	3.    edit my location: 
	     http://api.eventful.com/rest/users/locales/add?...&id=eventor&locale=
    	4.    add/edit my events:  
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
                   
                   
                   
                

    
