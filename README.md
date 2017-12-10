# Cloud-Land-sample
Android application with custom sign-in screen, using App ID Cloud Directory API.

![alt text](/app/src/main/res/drawable/cloud_land_login.png){:height="36px" width="36px"}

## Before running 
1. Create App ID service from the [IBM Cloud services catalog](https://console.bluemix.net/catalog/services/app-id?taxonomyNavigation=apps).
2. In the App ID dashboard go to _Cloud Directory_ tab under _Identity Providers_, and set: _Allow users to sign in without email verification_ to _Yes_.
2. In the App ID dashboard go to the _service credentials_ tab
3. In the _Action_ column click on _View credentials_. (or create new credentials if there aren't)
4. Copy the _tenantId_ GUID number.
5. Paste the _tenantId_ to the [_credentials.xml_](/app/src/main/res/values/credentials.xml)
6. Go to MainActivity.java and change the region according to the region your App ID instance is deployed.
7. Run the Cloud Land app.
