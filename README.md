# mvp

USERS CAN SEARCH FOR EVENTS

USERS CAN SAVE EVENTS THEY ARE INTERESTED IN

USERS CAN VIEW THEIR SAVED EVENTS

USERS CAN VIEW WHO ELSE IS INTERESTED IN THEIR SAVED EVENTS

    to do:
       1. create db with test users
            user = username 
                   password - hashed
                   email
                   myEvents
        2. everything else
         
                   
                   
                    



function render sign up page() 

function render sign up form()

(user enters username - on.click())
      function validate un()
		possible outcomes: (tests)
			password taken
			password invalid format      
			password null
			password not trimmed
			
		username valid
		function create user(id, username)  CREATE - api post call to db
		function create id()
		function store id, username()
		
		
     (user enters password) 
	   function validate pass()
        possible outcomes: (tests)
            password too long
            password too short
            password null
	    
            password valid
	            auth password 
                    create token - return - create secret hash - return
                    password authorized -
		    
		    function update user()      GET/UPDATE
		    function fetch user()
		    function add hashed password to user()
		    function save user()
		    function store user info in db()
		    
		    function render main page()

(user selects i already have an account  on.click())
    
       function render sign-in form()  
       
 (user enters username - on.click())
       function make api call to db()
       function validate un() 
		possible outcomes: (tests)
			username not found
			username null
			username valid
     (user enters password) 
	   function validate pass()
        possible outcomes: (tests)
            password not found
			password null
			password valid
	            
            if valid input - function auth password() (test)
                    create token - return - create secret hash - return
                         if auth - function render main page()

(user selects continue as guest)
        function render main page()


function show/hide() (show main page/hide sign up/sign in)

    function render form()
        (user selects event search and enters event name on.click)
            function handle event search()
                function validate entry() (tests)
                    possible outcomes:
                        entry null
                        entry not found
                        entry valid
                     
                    function clear input() 
                    
                    function make get request to eventful api()
                    function return data()
                    function show results(event)
		  
                   
                   function save event() mark user as interested in event
                        function create variable myEvents()
                        function save myEvents to db()
	                function reset event listener()


	(user selects artist search and enters artist name on.click)
           function handle artist search()
            function validate entry() (tests)
                    possible outcomes:
                        entry null
                        entry not found
                        entry valid 
                        
                        function clear input() 
                        
                        function make get request to eventful api()                           
                        function return data()
                        function render results(event)
			
                   
	                function reset event listener()
                        
            
     (user selects location search and enters event name on.click)
            function handle location search()
            function validate entry() (tests)
                    possible outcomes:
                        entry null
                        entry not found
                        entry valid 
                        
                        function clear input() 
                        
                        function make get request to eventful api()                           
                        function return data()
                        function show results(event page)
			function render event page()
                   
	                function reset event listener()
                        

       (user selects user search and enters user name on.click)
            function handle user search()
                function validate entry() (tests)
                    possible outcomes:
                        entry null
                        entry not found
                        entry valid 
                        
                        function clear input() 
                        function reset event listener()
                        function make get request to db()
                        
                            function seed db()
                            function return user data()
                            function dispaly user data()
			    
			    
			    
		
		
		


       
