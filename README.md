# mvp

function render sign up page() 

function render sign up form()
function handle sign-up form()

	user enters username password - on.click()
function route to tests for validation()
function perform validation tests()
	if(error) - alert
	if validated -
function perform auth tests()
	if(error) - alert
	if auth - create token - return and -
function render main page()



	user selects i already have an account  on.click()
function render sign-in form()
function handle sign-in form()
	user enters username password - on.click()
function route to tests for validation()
function perform validation tests()
	if(error) - alert
	if validated -
function perform auth tests()
	if(error) - alert
	if auth - create token - return and -
function render main page()


	user selects continue as guest
function render main page()


function show/hide()
function api call return 6 events 
function render events

function render form()

	user selects event search and enters event name on.click
function handle event search
function validate entry
function api call
function return data
function render data
function clear input 
	if user enters new data on.click
function clear results, replace

	user selects artist search and enters event name on.click
function handle artist search
function validate entry
function api call
function return data
function render data
function clear input
	if user enters new data on.click
function clear results, replace

	user selects location search and enters event name on.click
function handle location search
function validate entry
function api call
function return data
function render data
function clear input
	if user enters new data on.click
function clear results, replace


	
function render sidebar()
function edit profile()
function delete profile()

function user search()
function render form()
function seed db()
function api call and return users()
function render data()
		
		
		

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
                 search events by event name  http://eventful.com/events?q=music&
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
                   
                   
                   
                

    
