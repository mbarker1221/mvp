# mvp

SIGN UP/SIGN ON/LANDING PAGE:
----------------------

      short description of the site and instructions to sign up/sign in below

    CONTINUE AS GUEST ————————————————————————————————— direct to home page                    
                     
    SIGN UP:
  
        user enters username   ------ username no entry ------               error message enter a username
        user enters username  ------- username does not meet criteria ------- error message enter valid username																 
                      
        user enters password ------- password no entry -------                error message enter valid password
        user enters password ------- password does not meet criteria -------- error message enter valid password
                                                                                
   
    user enters username ----- valid ——--— user enters password --——— valid —--- continue to home page    
    
 
    SIGN ON:
           
      user enters username   ------ username no entry ------  error message enter valid username
      user enters username  ------- username not found ------- error message enter valid username
                      
      user enters password ------- password no entry -------   error message enter valid password
      user enters password ------- password not found -------- error message enter valid password
      
   
    user enters username ------- valid  -------- user enters password ------- valid --------- home page
        

          

HOME PAGE:
  
        event search:
              
                 search events by artist  http://eventful.com/events?q=music&
                 search events by date  http://eventful.com/events?q=music&l=&t=
                 search events by location (zip code or city)  http://eventful.com/events?q=music&l=
                
               
        click here to edit your username, password or delete your profile — redirects to profile page
	find friends --- redirects to social page


PROFILE PAGE:
                             
       edit profile:  edit username ----- username no entry ------- error and show message to enter username
       			            ----- username does not meet criteria -------- error and show message to enter 
                                                                                    a valid username
											
		      edit password ----- password no entry ------- error and show message to enter password
        			    ----- password does not meet criteria -------- error and show message to enter 
                                                                                   a valid password
											
		      delete profile  -----  profile delete
					
       		      see my events
            			http://api.eventful.com/rest/users/calendars/list?app_key=...&owner=eventor
   	
    		      add/edit my events:  
		     		http://api.eventful.com/rest/users/going/add?...&event_id=
                  		

SOCIAL PAGE:

      
      
      user search  ——  FIND FRIENDS

		1.  search by username, name or email: http://api.eventful.com/rest/users/get?...&id=mruser
		
	
 
       
                Request Token
                POST http://eventful.com/oauth/request_token
                Authorize Request Token
                GET http://eventful.com/oauth/authorize
                Access Token
                POST http://eventful.com/oauth/access_token
                   
                   
                   
                

    
