# Fyers
---

* Official Website: [https://login.fyers.in/](https://login.fyers.in/)

* Trading Website: [https://login.fyers.in/](https://login.fyers.in/)

* Markets Supported: India

## 1. Important Point(s) to Note

---

* It is required to login **once** daily (at the start of the trading day).

## 2. Login and Set up your Fyers Account
---
This section will take you through the step-wise instructions to log in, setup, and bind your broker into your AlgoBulls Account.

### i. Before you Start
---
Keep the following information available before you start:

1) AlgoBulls Account Credentials

* Phone Number

* Password

2) Broking Account Credentials

* App ID

* Secret ID

* 4-digit Pin

!!! Note
    To get the App ID and Secret ID, you'll have to create an [App](https://myapi.fyers.in/docsv3#tag/App-Creation/Individual-Apps) in your Fyers account. Please follow the below steps to create an app in your Fyers account.

### ii. App Creation

* Login to your Fyers account and click on the **Create App** button.

[![Fyers](imgs/fyers/create_app.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/create_app.png)

* Give the **App Name** as **AlgoBulls**
* Give the **Redirect URL** as **https://app.algobulls.com/loading**

[![Fyers](imgs/fyers/app_creation_details.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/app_creation_details.png)

1. Scroll down and delete the default **Webhook/Postbacks**.

2. Check all the checkboxes in the **App Permission** section.

3. Check the **Terms and Conditions** checkbox.

4. Click on the **Create App** button at the bottom.

[![Fyers](imgs/fyers/create_app_terms.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/create_app_terms.png)

* Once the app is created, copy the App ID and Secret ID for the next steps.

[![Fyers](imgs/fyers/app_created_successfully.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/app_created_successfully.png)

### iii. One-Time Activity
---
* Visit the AlgoBulls [Login Page](https://app.algobulls.com/user/login).

[![Fyers](imgs/algo_home.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/algo_home.png)

* If you do not see your broker name, then type **Fyers** in the Search Box. and then click on the Broker Link that shows **1-time-activity** as the tooltip.

[![Fyers](imgs/fyers/one_time_activity.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/one_time_activity.png)

* Login to your AlgoBulls account.

* Once you login you'll be redirected to the pane with the Fyers 1-time activity selected. Click on **Next**.

[![Fyers](imgs/fyers/one_time_activity_selected.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/one_time_activity_selected.png)

* Enter your App ID in the **CLIENT_API_KEY** field and your Secret ID in the **CLIENT_SECRET_KEY** field. Click on **Confirm**.

[![Fyers](imgs/fyers/one_time_activity_creds.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/one_time_activity_creds.png)

* Your 1-time activity is complete.

[![Fyers](imgs/fyers/non_oauth_broker_added.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/non_oauth_broker_added.png)

* You can see the broker added in the Broking Details section.

[![Fyers](imgs/fyers/non_oauth_broker_visible.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/non_oauth_broker_visible.png)

### iv. Daily Activity (Login)

* Now click on **Add Broker**, type **Fyers** in the search bar and click on the Broker Link that shows **Daily Login** as the tooltip.

[![Fyers](imgs/fyers/select_oauth_broker.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/select_oauth_broker.png)

* You'll be redirected to the **Fyers** login page. Enter your mobile number and click on **Continue**.

[![Fyers](imgs/fyers/oauth_login_1.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_1.png)

* Type the OTP that you receive and click on **Confirm OTP**.

[![Fyers](imgs/fyers/oauth_login_2.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_2.png)

* Enter your 4-digit Pin and click on **Sign in**.

[![Fyers](imgs/fyers/oauth_login_3.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_3.png)

* You'll be redirected back to the AlgoBulls Broking Details section where you can see the broker added.

[![Fyers](imgs/fyers/oauth_broker_added.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_broker_added.png)

### v. Another way to login

#### a. One-Time Activity

* Login to your AlgoBulls account

[![Fyers](imgs/algo_home.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/algo_home.png)

* Go to the **Broking Details** section and click on **Add Broker**.

[![Fyers](imgs/broking_details.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/broking_details.png)

* Select the Non OAuth broker and click **Next**.

[![Fyers](imgs/fyers/search_broker_nonoauth.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/search_broker_nonoauth.png)

* Enter your App ID in the **CLIENT_API_KEY** field and Secret ID in the **CLIENT_SECRET_KEY** field. Click on **Confirm**.

[![Fyers](imgs/fyers/one_time_activity_creds.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/one_time_activity_creds.png)

* Broker is binded to your account.

[![Fyers](imgs/fyers/non_oauth_broker_added.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/non_oauth_broker_added.png)

[![Fyers](imgs/fyers/non_oauth_broker_visible.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/non_oauth_broker_visible.png)

#### b. Daily Activity (Login)

* Click on **Add Broker**, type **Fyers** in the search bar and select the broker.

[![Fyers](imgs/fyers/select_oauth_broker.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/select_oauth_broker.png)

* You'll be redirected to the **Fyers** login page, Enter your mobile number and click on **Continue**.

[![Fyers](imgs/fyers/oauth_login_1.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_1.png)

* Type the OTP that you receive and click on **Confirm OTP**.

[![Fyers](imgs/fyers/oauth_login_2.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_2.png)

* Enter your 4-digit Pin and click on **Sign in**.

[![Fyers](imgs/fyers/oauth_login_3.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_login_3.png)

* You'll be redirected back to the AlgoBulls Broking Details section where you can see the broker added.

[![Fyers](imgs/fyers/oauth_broker_added.png "Click to Enlarge or Ctrl+Click to open in a new Tab") ](imgs/fyers/oauth_broker_added.png)

## 3. Support
---

For Help and Support, contact us on +91 80692 30300 or email us.