# Deploying the Trigger service to Cloud Function


1. Create a file named `.env.yaml` at the root of this folder. Copy the contents of `placeholder.env.yaml` and set the values

```
# Google Cloud project ID
GOOGLE_CLOUD_PROJECT: "INPUT_YOUR_GOOGLE_CLOUD_PROJECT_HERE"

# Region where this service will be deployed
GCLOUD_REGION: "europe-west1"

# Cloud storage bucket name where the files will be uploaded
BUCKET_NAME: "INPUT_YOUR_GOOGLE_CLOUD_STORAGE_HERE"

# Uploader service endpoint
UPLOADER_SERVICE: "<INPUT_SERVICE_ENDPOINT_HERE>/run"

# Header and token to be authenticated to call the Uploader service
UPLOADER_SERVICE_AUTH_HEADER: "Wizdam-Dev-Csc-Token"
UPLOADER_SERVICE_AUTH_TOKEN: ""

# Slack used for notification when errors are encountered. Can be left blank
SLACK_BEARER_TOKEN: ""
SLACK_CHANNEL_ID: ""
```

2. To deploy, run
```
sh deploy.sh
```
