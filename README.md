# Net Worth Calculator
This app will be created to calculate my net worth and will include a way to essentially manage my finances better.

# This app will be created with help from
 `https://www.schwabmoneywise.com/public/file/P-4038856/Net-Worth-Worksheet.pdf`


 # Step 1: Update Index.js 
 
After following advice from the developers.facebook.com forum, I will be creating and deploying a webhook in heroku. 

The Heroku App will be deployed at:
https://secure-hamlet-18311.herokuapp.com/

To test the GET request:
`curl -X GET "secure-hamlet-18311.herokuapp.com/webhook?hub.verify_token=networthverify&hub.challenge=CHALLENGE_ACCEPTED&hub.mode=subscribe"`

To test the POST request:
`curl -H "Content-Type: application/json" -X POST "secure-hamlet-18311.herokuapp.com/webhook" -d '{"object": "page", "entry": [{"messaging": [{"message": "TEST_MESSAGE"}]}]}'`

