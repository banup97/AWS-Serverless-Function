# AWS-Serverless-Function
Serverless Function deployment using AWS Lambda and API gateway 

To understand serverless computing by creating and deploying a simple AWS Lambda function that runs automatically when triggered.
Tools Used:

AWS Lambda (Free Tier)
API Gateway (HTTP Trigger)
CloudWatch (Monitoring & Logs)
Browser

A serverless fucntion runs your code in response to an event (like an HTTP request ) - without the need to manage servers.

python version Function Code (main.py)

def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from my first cloud function!'
    }

Deployment Steps
1. Open AWS Console → Navigate to Lambda > Create function
2. Choose Author from scratch → Runtime = Python 3.x
3. Scroll down to Code source, paste above code
4. Click Deploy 
5. Under Configuration > Triggers, add API Gateway (HTTP API)
6. Copy the Invoke URL and test it in browser.
7. Check CloudWatch Logs for START – END – REPORT messages
8. CloudWatch log (START / END / REPORT messages)

   Invoke URL: https://<Asia pacific mumbai>.amazonaws.com/default/helloServerless

After testing, deleted the lambda function.

Outcome: 
Learned about Function-as-a-Service (FaaS) and event-driven architecture.
Successfully deployed and tested a serverless function on AWS.
Monitored execution and verified results using CloudWatch Logs.
Documented the complete workflow with screenshots for submission.
    
