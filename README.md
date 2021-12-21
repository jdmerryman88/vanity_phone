Vanity Phone Number Creation

Overview

This project takes the phone number of a caller from Amazon Connect and reports back to the caller the three best vanity phone numbers for their number. An additional two numbers are saved into a Dynamodb database paired with the callers phone number. This application uses an Amazon Connect contact flow with a dynamodb database and lamda functions to process the data. Python is used in the lambda functions to handle all of the computing of the data and to return the values. 

Development Languages

This project utilizes Python, Amazon Lambda, and Dynamodb to create the working Amazon Connect Flow. The flow works by first telling the caller that three vanity phone numbers will be provided to them at the end of the call. During this process a lambda integreation is used to send the caller's number to a lambda function to create all the number/ letter combinations possible for their phone number. The top five are selected and written to a dynamo database. A second lambda integration is then incorporated to return the three best vanity numbers to Amazon Connect to be read to the caller. 

Best Vanity Number Determination

The best vanity number was determined by picking a random number and using that as the best vanity number.


Difficulties and Improvements

In the future with more time allowed this project could be further improved. The first step in improving the project would be to make the code as efficient as possible by removing any unneccessary steps or variables within the code. Further improvement in the process would be to create a better method in order to determine the best vanity phone number. This could be achieved in a multitude of ways but a few that I would like to implement in the future are to personalize the vanity phone number for the caller or use an API to google or some other search engine to get the most searched for word in the vanity number list. In order to personalize the vanity number a step in the Amazon Connect Flow could be to ask the callers questions (ie. is this a business number?, what are your hobbies?, what is your favorite team or movie?). This further customization would allow for a more focused and descriptive search when determining the best vanity numbers. Also as mentioned about using a search engine list of most commonly used search terms would make determing the best vanity numbers better. Difficulties that I faced throught this project included learning how to  implement an Amazon Connect flow and tie it to lambda function and dynamodb.
