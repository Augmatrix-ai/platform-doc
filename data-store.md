# Dataset Hub

## Data Privacy and Security

At Augmatrix.io, we prioritize data privacy and security, ensuring a safe environment. Here's how we maintain security and privacy.

1. Bring your Own Datastore.
2. Audit logs.
3. Credential vault

### **1. Bring Your Own Datastore:**

We provide users with the flexibility to configure your own cloud storage, ensuring data security without the risk of leakage. Users can either test sample datasets with Augmatrix.io's default datastore or configure your preferred cloud storage. We support various cloud storage capabilities, including.

<figure><img src=".gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

* **Amazon S3.**
* **Azure Blob Storage.**
* **Google Cloud Bucket.**
* **Including other cloud storages can be configured on the  requested based**

Below are step-by-step configurations for each cloud storage option:

#### **1. Let's Configure Amazon S3 In Augmatrix**&#x20;

1. Go to Augmatrix platform.&#x20;
2. Go to the Data Store page.
3. Click on "Mount New Drive".
4. Select "Amazon S3" as drive.
5. Provide any name for the drive.

#### Steps to Follow in AWS:

* Obtain the endpoint URL, access key, secret key and Region from your [Amazon S3 bucket](https://docs.aws.amazon.com/AmazonS3/latest/userguide/configuring-bucket-key.html).
  1. Create a bucket on Amazon S3.
  2. Copy the bucket's URL (remove the "https" part) for the endpoint section.
  3. Access IAM on Amazon and create access keys. Use the access and secret keys for Augmatrix platform.
* Set "Secret" to True and specify the region for the bucket.
* Configure bucket permissions by adding CORS code for data extraction to Augmatrix platform.

```
[    
   {    "AllowedOrigins": ["https://stage.augmatrix.ai"],
        "AllowedMethods": ["GET", "PUT", "POST"],
        "AllowedHeaders": ["*"],
        "MaxAgeSeconds": 3000
    }
]
```

5. After Providing Required details.&#x20;
6. Click on Test after successful connection.
7. Click  on Add Drive.
8. Drive is ready to upload dataset.&#x20;

#### **2. Let's configure Azure Blob Storage In Augmatrix**

1. Go the Augmatrix platform.
2. Navigate to the Data Store page.
3. Click on "Mount New Drive."
4. Select  "Azure" as drive.
5. Provide any name for the drive.

**Steps-to-follow in Azure:**

* Enter the storage account name and account key (connection string).
* Visit[ azure portal](https://learn.microsoft.com/en-us/azure/storage/common/storage-account-create?tabs=azure-portal).
* Create a storage account on Azure.
* Inside the storage account, create a container.
* Obtain the account name and key from the Azure portal for Augmatrix platform.

<figure><img src=".gitbook/assets/Untitled design (3).jpg" alt=""><figcaption><p>Azure images</p></figcaption></figure>

5. After Providing Account name and keys.
6. Click Test after successful connection.
7. Click Add Drive.
8. Drive is ready to upload dataset.&#x20;

#### **3. Google Storage Configuration In  Augmatrix**

1. Go to Augmatrix platform.
2. Visit the Data Store page.
3. Click on "Mount New Drive"'
4. Select Google Cloud as Drive.
5. Provide any name for the drive.

**Steps-to-Follow Inside Google Cloud:**

* Enter the account key obtained from the Google Cloud console.
  1. Create a bucket in Storage Management on Google Cloud.
  2. Grant READ and WRITE permissions.
  3. Generate an API key in the [Google Cloud console](https://cloud.google.com/docs/authentication/api-keys) and paste it into the Augmatrix.io platform.

5. After Providing Bucket name and keys.
6. Click Test after successful connection.
7. Click Add Drive.
8. Drive is ready to upload dataset.&#x20;

Follow these steps carefully to ensure seamless integration and secure handling of your data. For detailed instructions on creating buckets and obtaining keys, refer to the provided links.

### 2. Audit logs:&#x20;

Audit logs will help to understand the events or actions that are captured and stored by the application for the purpose of tracking and monitoring user activity. It provides a way to review and investigate past actions in order to identify any security incidents or compliance violations.



### 3. Credential Vault

Credential vault keeps your important information like credentials, and keys. It uses strong security methods to protect your data.  The above cloud configuration keys can also be stored in this credential vault.&#x20;

Our credential vault is a secure storage system that is used to manage sensitive information such as passwords, API keys, certificates, and other secrets.
