# Cloud-Land-sample
Android application with custom sign-in screen, using App ID Cloud Directory API.

![alt text](/app/src/main/res/drawable/cloud_land_login.png)

## Before running 
1. Create App ID service from the [IBM Cloud services catalog](https://console.bluemix.net/catalog/services/app-id?taxonomyNavigation=apps).
2. In the App ID dashboard go to **Cloud Directory** tab under **Identity Providers**, and set: _Allow users to sign in without email verification_ to _Yes_.
2. In the App ID dashboard go to the **service credentials** tab
3. In the **Action** column click on **View credentials**. (or create new credentials).
4. Copy the `tenantId` GUID number.
5. Paste the `tenantId` to the [credentials.xml](/app/src/main/res/values/credentials.xml)
6. Go to [MainActivity.java](/app/src/main/java/com/ibm/bluemix/appid/cloud/directory/android/sample/appid/MainActivity.java) and change the region according to the region your App ID instance is deployed.
7. Run the Cloud Land app.
