# Script
 
 1. Install Node [nodejs](https://nodejs.org/en/download/)
 2. `npm install swagger --global`
 3. `swagger project create --framework restify swagger_app`  
 	[swagger.io](http://swagger.io/)
 4. `swagger project start swagger_app`
 	* Or `start "Serve" /b cmd /k swagger project start swagger_app`
 4. Add the following line to `app.js`  
   
 ```js
 app.use(restify.CORS());
 ```
 5. `swagger project edit swagger_app`
 6. Edit file `api\controller\hello_world.js`  
   
	 ```js
	res.type = 'json';
	res.json({message: hello});
	 ```