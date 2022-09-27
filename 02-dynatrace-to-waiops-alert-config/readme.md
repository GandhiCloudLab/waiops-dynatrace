# Dyantrace to WAIOps Alert Configuration

This document explains how to create alert notification in Dyantrace to push the alerts to WAIOps webhook.

## Create Notification entry in Dynatrace

1. Click on `Settings > Integration > Probelm Notifications`

![Dyna](images/image-00001.png)

2. Click on `Add Notification`

![Dyna](images/image-00003.png)

3. Enter the following.

- Display Name : Any text
- Webhook URL : WAIOPs Webhook URL Created .

![Dyna](images/image-00004.png)

3. Click on the `Create basic authentication header` button.

4. Enter the following.

- UserName : WAIOPs Webhook URL user.
- Password : WAIOPs Webhook URL password.

![Dyna](images/image-00005.png)

5. Copy and paste the custom payload from the file [files/dyna-mapping.json](./files/dyna-mapping.json).

This file needs to be updated with right mappings in future.

![Dyna](images/image-00006.png)

6. Try sending test notification to WAIOps using the `send test notification` button.

![Dyna](images/image-00007.png)

7. Click on `Save Changes` to save the entry.

8. See the noticiation entry created.

![Dyna](images/image-00008.png)

## View Alert in WAIOps

View the alert created for the test notification in WAIOps.

![Dyna](images/image-00009.png)


Note: This payload to be improved to have all the columns populated in the Alert.