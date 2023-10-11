# Report Expass 6
Link to GitHub: https://github.com/EndreSletnes/dat250expass6

All the code is written in a new repository linked here. Only change I made on code from expass4 was the CORS fix mentioned under technical issues.

## Technical Issues
* CORS blocked requests from web app to spring application so i added @CrossOrigin(origins = "http://localhost:4200") because angular apps run on localhost:4200.
* Did not use subscribe on the request that creates a new Todo so all request worked except that. It worked fine after I added .subscribe().
