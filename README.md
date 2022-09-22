# lambda-layer-custom-delete


Lambda layers 

A Lambda layer is a .zip file archive that can contain additional code or other content. A layer can contain libraries, a custom runtime, data, or configuration files.

Lambda layers provide a convenient way to package libraries and other dependencies that you can use with your Lambda functions. Using layers reduces the size of uploaded deployment archives and makes it faster to deploy your code


Custom Resources

Custom resources enable you to write custom provisioning logic in templates that AWS CloudFormation runs anytime you create, update (if you change the custom resource), or delete stacks. For example, you might want to include resources that aren't available as AWS CloudFormation resource types. You can include those resources by using custom resources. That way you can still manage all your related resources in a single stack.

Prerequisites:

  For the layer creation I created the s3 bucket (lmda-layer-nodejs) where i put the NodejsLayer.zip file as its required for creating the layer. 
Note: Am doing this lab in us-east-1

Steps to create layers along with custom resources

   

1. Sign in to the AWS Management Console and open the AWS CloudFormation console at https://console.aws.amazon.com/cloudformation.
If this is a new CloudFormation account, choose Create New Stack. Otherwise, choose Create Stack.

2. In the Template section, select Upload a template file and upload layer-custom-delete.yml Click next.  

3. Click on next and give the stack name.

4. Click on next until you reach this step and click on create stack.

5. After stack creation successfully you can check the lambda layer in : https://us-east-1.console.aws.amazon.com/lambda/home?region=us-east-1#/layers




When you Delete the stack it automatically delete the layer that is part of this template you don't have to delete this layer manually. 

Helpfull links for Further Reading

  Cloud formation getting started : https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/GettingStarted.html
  Building layers                 : https://docs.aws.amazon.com/serverless-application-model/latest/developerguide/building-layers.html
  Building layers using CFT       : https://docs.aws.amazon.com/lambda/latest/dg/configuration-layers.html
  Custom resources                : https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/template-custom-resources.html
