# Cloud-Land-sample
[Use your own branded UI for user sign-in with App ID - IBM Cloud Blog](https://www.ibm.com/blogs/bluemix/2018/01/use-branded-ui-user-sign-app-id)</br>
Android application with custom sign-in screen, using App ID Cloud Directory APIs.

![alt text](/app/src/main/res/drawable/cloud_land_login.png)

## Before running 
1. Create App ID service from the [IBM Cloud services catalog](https://console.bluemix.net/catalog/services/app-id?taxonomyNavigation=apps).
2. In the App ID dashboard go to **Cloud Directory** tab under **Identity Providers**, and set: _Allow users to sign in without email verification_ to _Yes_.
3. In the App ID dashboard go to the **service credentials** tab, in the **Action** column click on **View credentials**. (or create new credentials).
4. Copy the `tenantId` GUID number.
5. Paste the `tenantId` to the [credentials.xml](/app/src/main/res/values/credentials.xml)
6. If your App ID service is not deployed on US region, go to [MainActivity.java](/app/src/main/java/com/ibm/bluemix/appid/cloud/directory/android/sample/appid/MainActivity.java) and change the region according to the region your App ID service is deployed.
7. Run the Cloud Land app.
