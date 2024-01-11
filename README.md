# anomaly-detection-demo


1. Follow the [instructions for installing OpenDataHub on OpenShift](link to stage 1).

## Create an IBM Cloud Object Storage Bucket

Create a credential in your object storage instance and map to the following environment variables 

COS_API_KEY_ID == The "apikey" property
COS_AUTH_ENDPOINT: Usually set to "https://iam.cloud.ibm.com/identity/token" but other environments may require this to be changed 
COS_ENDPOINT == Select from the list available here https://control.cloud-object-storage.cloud.ibm.com/v2/endpoints
COS_INSTANCE_CRN == The "resource_instance_id" Property
REGION == The region you are using. If using a global storage mechanism leave blank.

## key management

If you are using ssh keys for your git login then set up a key on the environment using the terminal.

1. [Generate an SSH key on this server](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#generating-a-new-ssh-key)

1. [Add the key to your SSH account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account)


