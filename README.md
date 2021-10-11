# AWS_developer-task1
1. Create a key pair 
2. Create a security group 
3. Launch an instance using the above created key pair and security group.
4. Create an EBS volume of 1 GB.
5. The final step is to attach the above created EBS volume to the instance you created in the previous steps.

Amazon Web Services is a cloud computing platform that provides customers with a wide array of cloud services. AWS (Amazon Web Services) is a secured cloud services platform that offers compute power, database storage, content delivery and various other functionalities also.

We have three ways to use AWS :

CLI (Command Line Interface)
WebUI
Through a program/code

Firstly create an account on aws and install AWS CLI program in your OS from the below link.
https://awscli.amazonaws.com/AWSCLIV2.msi

1. Now we have to provide the access key and secret key, the region for login to your account.
use aws configure command to do so

2. The next step is to create Key  :
use the below command to do so.
ec2 create-key-pair --key-name awskey1

This will give us the key name and key pairId.
And now the key pair have been successfully created. In the next step, we'll have to created a security group. 

3. To create a security group follow the line of command given in the below image.

note: While creating the security group using CLI, it is a must to provide some description of the security group. Else, it will throw an error. aws ec2 create-security-group --group-name awsg1 --description "my security". 

And now the security group will be created.

4. Now, it is time to create an instance using the AWS CLI. I have used the same key-pair and the security group that we created in the above steps. 

Note: If you don't provide the Security Group, it will use the default security group. The same will be used for the default Instance.

5. Now that the instance has been launched in the region we specified.

6. Now we will create a volume of 1 GB using the AWS CLI:

-we will also have to specify the size of the volume that we are attaching and the zone
-And to do that use the following command.


7. Now we have used AWS CLI again to attach this volume to the previously created instance:

And now, the volume is in use and it is attached to the instance as you can see and is ready to use.
- We can see the size and region have been selected as we specified.
- And we also have the attachment information given below.

And finally, all the objectives of the task have been successfully completed.
Hope all of you liked this article and enjoyed it .
Thank you .....happy learning!
