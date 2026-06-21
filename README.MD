# Task 6: Set Up a Serverless Function

## Objective
Create and deploy a serverless function using AWS Lambda and access it through a Function URL.

## Services Used
- AWS Lambda
- Function URL
- Python 3.13

## Steps Performed

### Step 1: Create Lambda Function
- Open AWS Lambda Console.
- Click Create Function.
- Select Author from Scratch.
- Function Name: Task6-Lambda
- Runtime: Python 3.13

### Step 2: Write Lambda Code

```python
def lambda_handler(event, context):
    return {
        'statusCode': 200,
        'body': 'Hello from RD INFRO TECHNOLOGY Task 6 Lambda Function'
    }
