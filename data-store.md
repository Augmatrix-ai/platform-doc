# Data store

**1.DATA PRIVACY AND SECURITY**

Augmatrix.io is a platform that places great importance on high data privacy and security, both for the platform itself and its users. To ensure the highest level of security and privacy, Augmatrix.io has implemented various features for privacy and security.\
1.1 **Datastore** \
We are very concerned about users' data privacy and security. we are providing a feature to configure their own cloud storage to the user to secure their data without any fear of data leakage.

If you want to test out your own data without configuring datastore.

The [Augmatrix.io](http://augmatrix.io/) we are providing the default storage to test out your own data to default store

We came up with different cloud storage capability, they are

1. Amazon S3
2. Azure Blob storage
3. Google cloud bucket

Here we have provided step by step configurations of different cloud storages but **any of them are important to configure**

&#x20;

**1.0 Amazon S3** **configuration with Augmatrix.io platform**

1. Go to data\_manger page
2. Click on Mount New Drive
3. you can see the pop-up comes with object Drive store
4. Select store as Amazon S3
5. Give any name to the drive
6. Get the End-point of S3 bucket
7. Access key
8. Secret Key

For extracting the End-point URL, access keys and Secret key. Follow these steps in Amazon console

A. Open the Amazon s3 buckets

B. Create a bucket with the name of user or \<any name >

C. Select the bucket and copy URL \<paste it in end point section without the https>

D. Open the IAM on Amazon

E. Go to access management

F. Create access key at point of creation you will get secret key paste it in

Augmatrix platform

To create the Amazon s3 bucket, follow these steps as in given link

1.[https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.htm)

To create the Access key from IAM follow these guide

1.[https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html](https://docs.aws.amazon.com/powershell/latest/userguide/pstools-appendix-sign-up.html)

9\. Secret set as True

10. Region set as \<your bucket region>

for extracting the data from the s3 to Augmatrix platform

1. Go the bucket permission
2. add CORS code
3. Sample code

`[ { "AllowedOrigins": ["https://stage.augmatrix.ai"],`

`"AllowedMethods": ["GET", "PUT", "POST"],`

`"AllowedHeaders": ["*"],`

`"MaxAgeSeconds": 3000`

`}`

`]`

**2.0 Azure storage Blob configuration with Augmatrix.io platform**

1. Go to data\_manger page
2. Click on Mount New Drive
3. You can see the pop-up comes with object Drive store
4. Select Azure as storage
5. Give any name to the drive name
6. Give the Storage account name
   1. &#x20;To create the storage account follow the instructions in the given link [https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal](https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal)
   2. Paste the account name in the storage account name
7. Give the Account key (Connection String)

<figure><img src=".gitbook/assets/att_4_for_16384134 (1).png" alt=""><figcaption></figcaption></figure>

&#x20;

To get the account name and account key go the azure portal

A. create a storage account with any name

B. Inside the storage account, create the Container name as user \<any name>

C. Go to the storage account and find access keys section

D. go to the access keys section and find the connection string

8. Paste those keys in the Augmatrix.io platform

&#x20;

**3.0 Google storage configuration with Augmatrix.io Platform**

1. Go to data\_manger page
2. Click on Mount New Drive
3. You can see the pop-up comes with object Drive store
4. Give the Drive name (bucket name)
5. Give the Account key

To get the Account key in google console follow these steps

A. go the google cloud console

B. Go Storage management and create a bucket and give the READ, WRITE Permissions

C. go APIs dashboard in the google cloud account

D. go to the credentials

E. create a API key paste the key in the Account Key section in Augmatrix.io

platform

**DONE**

Follow these steps to understand the getting the bucket and keys

1. Creating google cloud bucket [https://cloud.google.com/storage/docs/creating-buckets](https://cloud.google.com/storage/docs/creating-buckets)
2. Get the Api keys

[https://cloud.google.com/docs/authentication/api-keys](https://cloud.google.com/docs/authentication/api-keys)\
