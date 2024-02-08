# anomaly-detection-demo


1. Follow the [instructions for installing OpenDataHub on OpenShift](link to stage 1).

1. Create a workbook
   Using these instructions.
   
## Create an IBM Cloud Object Storage Bucket

Create a bucket in a cloud object storage instance - choose the quick start option.
Create a credential in your object storage instance and map to the following environment variables 

COS_API_KEY_ID == The "apikey" property
COS_AUTH_ENDPOINT: Usually set to "https://iam.cloud.ibm.com/identity/token" but other environments may require this to be changed 
COS_ENDPOINT == Find this on the bucket configuration tab in your cloud instance
COS_INSTANCE_CRN == The "resource_instance_id" Property
REGION == Find this on the bucket configuration tab in your cloud instance

## key management

If you are using ssh keys for your git login then set up a key on the environment using the terminal.

1. [Generate an SSH key on this server](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)

1. [Add the key to your SSH account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)

1. If you get an error `Load key "/opt/app-root/src/.ssh/id_ed25519": bad permissions` run the following command in a terminal.

```
chmod 600 /opt/app-root/src/.ssh/id_ed25519
```