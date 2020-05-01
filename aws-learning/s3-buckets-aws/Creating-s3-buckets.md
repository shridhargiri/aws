**Here are the steps to create a S3 bucket in AWS:**
   1. After logging into your AWS console, select 'Services' from the top left corner. 
   2. Under Storage section, select 'S3'.
   3. Now, click on create bucket.
   4. As discussed earlier, enter an unique bucket name and the Region where the storage bucket need to be created.
   5. Once done with name and region, select the access settings for the bucket.
   6. Here, select the checkbox for 'Block all public access'(which is by default selected) if you want to keep the S3 bucket private and don't want any remote client to access the bucket. *[Click here to read more about access control list in AWS.](http:\\)*
   7. If you're creating this for the sake of practice or just want to use the bucket for normal Read/write storage, ignore the advanced settings by keeing it default. If you want to read more about Object lock, you can visit this link: *[Object lock in AWS](https://docs.aws.amazon.com/console/s3/object-lock)*
   8. That's it, click on 'Create Bucket'.
   9. Upon successful creation of the bucket, click on the bucket name to access it and here you use it to host a website and many such different applications.
