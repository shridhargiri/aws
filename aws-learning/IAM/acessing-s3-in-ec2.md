## ***Accessing S3 bucket in EC2 instance*** #
* Accessing the S3 bucket service directly from an instance is not possible.
* To access the S3 service, IAM role needs to be created which gives permission to our bucket to be accessed from the instance.
* Refer to this image from **Create Role** page on AWS console for information on roles in IAM:
> [roles_in_iam](https://github.com/shridhargiri/aws/blob/aws-learning/aws-learning/IAM/iam_roles.PNG)  

### *Steps for creating a rule to access S3 bucket in AWS instance* #
  1. In the AWS console, under 'Services', look for 'Security, Identity, & Compliance' section.
  2. Now, click on IAM.
  3. Within the list of options available in the left bar, select 'Roles'.
  4. Here you can see what exactly IAM roles are. Click on 'Create Role' to create a new role.
  5. Now here we can select the service on which we want to create the role.
  6. In our case, we'll select S3 service from the list as we want to give access of S3 to our instance.
  7. One the name of service is selected, the 'Next' button would be activated at the bottom. Click on this button.
  8. On the permissions page, there is a list of policies available that are pre-defined by AWS. Each policy contains a set of permissions for differet services in AWS. We can select a policy from this list or can even create our own
  9. As we want to give full access of our bucket to our instance, there is a policy pre-defined. The name of the policy is 'AmazonS3FullAccess'. We'll select this policy.(If we simply type 'S3' in the search, we'll be able to see all the pre-defined policies fort S3).
  10. Use the checkbox on the left to select this policy and click on 'Next'.
  11. On the next page, we can add tags if we want to. It is optional and you can click on 'Next' even without adding any tags.
  12. Next is the final page, the review page. Here you have to give a globally unique name to your role and review all the details you have entered.
  13. Once you have reviewed everything, you can proceed to click on 'Create Role'. This would create a role and you would be able to access your S3 bucket from your instance.


[References: https://www.awseducate.com ]
