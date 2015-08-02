# android-sms
This application allows you to automatically backup SMS messages on your Android device to Gmail.

You'll be able to browse and search your incoming and outgoing messages - neatly put into threads - under the "SMS" label in Gmail. To browse your backed up messages, log into Gmail and click on "SMS" in the labels box, which is located in the left sidebar.
Prerequisites

You need to have a Gmail account with IMAP enabled. See the Enabling IMAP Gmail help page to learn how to enable IMAP for your Gmail account.
Installation

SMS Backup can be downloaded and installed from Android Market. Go directly to the Android Market listing by clicking the following link on your device: Android Market listing. Click the "Install" button and confirm the required permissions.
Configuration

After starting SMS Backup, enter your Google username and password. Note that the password will be stored unencrypted on your device. It is, however, only used to log into Gmail using a secure SSL connection and is not readable by other applications. See below for a description of the advanced settings.
Usage
Initial Backup

It is important that you perform the first backup manually. SMS Backup needs to know whether you want to upload messages currently stored on your device or not. After having entered your login information, SMS Backup will ask you to perform a first sync.

If you choose to Backup, SMS Backup will start backing up your messages to Gmail. The maximum number of messages backed up at a time is set to 100 by default, so if you have a lot of messages, it will take multiple runs to completely backup everything.

If you choose to Skip, nothing is sent to Gmail and all messages currently stored on your device are simply marked "backed up". This option is handy if you previously uninstalled SMS Backup and do not want to send your messages again to Gmail. Please note that any messages arrived after you last uninstalled SMS Backup and this initial backup won't ever be backed up to Gmail.

After you performed your initial backup, SMS Backup is ready to run in the background and finish uploading all of your current and future messages.
Auto Backup

By default, SMS Backup runs in the background to automatically backup any new arriving and outgoing messages. Incoming messages are backed up 20 seconds after they arrived on the device, while outgoing messages are backed up after a maximum of 30 minutes.

You should regularly check if there was an error backing up in the background by starting SMS Backup and looking at the state. In the future, we plan to put up a notification when an error is encountered during a background backup.
Manual Backup

You can at any time initiate a manual backup by starting SMS Backup and clicking on the "Backup" button. The progress of the backup will be shown on the screen.
Stop Ongoing Backup

Click the "Stop backup" button in order to cancel an ongoing backup. The next backup will continue exactly were the current backup left off. (Since version 1.1.0)
Update

Either look for Android Market notifications for new application versions or regularly check for updates by starting SMS Backup, pressing the menu key, then choosing "Update". This will send you to the Android Market listing of SMS Backup where the installation status changes to "Update available" if there is a new version available.
Share the Love

If you enjoy using SMS Backup, you can recommend this application to your friends by e-mail using the "Share" menu item.

If you LOVE SMS Backup, feel free to donate an amount of your choice! It will be much appreciated.
Advanced Settings

The advanced settings screen allows you to configure the following settings:

    Mark as read (Since version 1.1.0)

        When this setting is enabled, SMS Backup will mark the e-mails generated on Gmail as read, otherwise they'll appear as unread. 

    Gmail label assigned to SMS

        SMS Backup will assign this label to backed up messages in Gmail. 

    Maximum number of items per backup

        If your device gets slow when backing up a lot of messages at once, this settings allows you to limit the number of messages sent during one batch. Any messages that are not backed up during that batch will be backed up as part of a later batch. 

Required Permissions

SMS Backup requires the following system permissions:

    Full Internet access

        This is required to be able to connect to the Gmail server and send your messages. Note that the connection to the Gmail server is SSL encrypted. 

    Prevent phone from sleeping

        This will keep your device awake while SMS Backup does its work. Usually, SMS Backup is only active for very short periods and should not draw a lot of your battery. 

    Read SMS or MMS, receive SMS

        This is required to be able to actually make a listing and send your messages to Gmail. 

    Read contact data

        This is required to be able to associate every message with its sender or recipient, which will be assigned to the from or to field in Gmail, respectively. 

NOTE: This project is automatically exported from https://code.google.com/p/android-sms/
