# Feedback_collecter_cloudformation
To automate the creation of a real-world feedback collection system with web hosting, data capture, and email alerts . Showing full-stack AWS capability using Infrastructure as Code.

## Step 1 : Open CloudFormation Console
1. Click on “Create stack”
2. Select "Upload a template file"
3. Create a template file in notepad or vscode
4. Upload the "webserver.yml" file
5 .Click "Next" ( Screenshot is attached Creation of stack)

## Step 2: Specify Stack Details
1. Stack name → Enter a name like: WebserverStack
2. Click" Next "

## Step 3: Configure Stack Options
1. This page lets you add tags, permissions, notifications, etc.
Leave everything as default
2. Click the “Next” button
   
## Step 4 : Review and create stack
1. Scroll down and review the settings (you don’t need to change anything).
2. Click "Submit"
   
## Step 5: View the Output (Public IP)
1. Click on the stack name WebServerStack
2. Go to the Outputs tab
3. You’ll see a key called:" Piblic IP"
4 .Copy the IP address shown

### Attached Screenshoots for the above steps.


###  Adding S3 + IAM Role to Your Existing Template and Update the Stack

## Step 1: Open Your Existing CloudFormation Template
   1. Opening the file feedback-app.yml
   2. Add the S3 Bucket + IAM Role + Instance Profile in yaml code
      
## Step 2: Modify the EC2 Resource to Attach IAM Role
  1. In existing WebAppInstance: resource, adding this line: "IamInstanceProfile: !Ref EC2InstanceProfile"

## Step 3:  Updating Your CloudFormation Stack
  1. AWS Console → CloudFormation(FeedbackCollectorApp)
  2. Click Update
  3. Choose “Replace current template”, and upload the new feedback-app.yml file
  4. Click Next → Next → Review → Click “Update stack”

### Screenshot attached updating stack 





