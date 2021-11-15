# Data Privacy and Backups: Best Solutions

## 3-2-1 Golden Rule of Data Backup

![Alt text](https://www.itguys.com/wp-content/uploads/2018/02/321Rule.jpg)

If you follow this rule the likelihood of losing any data permanently is *incredibly* low, however it can be a bit of a pain to setup. So what does this mean for researchers and different career stages?

**Principal investigator** 

If you're running a lab and generating lots of primary data, you should stick to rule very strictly. Ideally, you would have a departmental storage server that has multiple copies of this data and a copy of this data somewhere offsite using a cloud storage provider or an offsite data bank.

**Graduate/Undergraduate Student**

This is my current career stage, so I can give some guidance on my data backup practices! The 3-2-1 rule is always recommended, but given the high startup cost I chose to simplify it a bit for myself. I backup my data onto two local devices and one cloud storage provider. I have a local backup because it makes recovering any lost data *much* faster. For instance, imagine losing/accidentally deleting 100 GBs of data if you're computer suddenly crashes. If this data was only stored in the cloud, such as with Google Drive, it could take anywhere from 1 to 5 hours to recover all of your data, but if the data was stored on an external hard drive or you could be up and running in as little as 15 minutes!

Another great advantage of backing up your data is version tracking! I've made plenty of changes to manuscripts that I wanted to undo and with realtime backups I can easily revert a document to a previous version. Cloud storage providers and local backups support this feature, and it can be a lifesaver!

## How to Backup Your Data

You can use these links as resources in the future, but today we'll try to set up one of these cloud backups!

### Windows - FileHistory (Local)

[https://www.groovypost.com/news/microsoft-windows-10-cumulative-update-kb3081438/](https://www.groovypost.com/news/microsoft-windows-10-cumulative-update-kb3081438/)

### MacOS - Time Machine (Local)

[https://support.apple.com/en-us/HT201250](https://support.apple.com/en-us/HT201250)

### Google Drive (Cloud - Unlimited Space through UW-Madison)

[https://support.google.com/a/users/answer/9965580?hl=en](https://support.google.com/a/users/answer/9965580?hl=en)

### OneDrive (Cloud - Unlimited Space through UW-Madison)

[https://support.microsoft.com/en-us/office/turn-on-onedrive-backup-4e44ceab-bcdf-4d17-9ae0-6f00f6080adb](https://support.microsoft.com/en-us/office/turn-on-onedrive-backup-4e44ceab-bcdf-4d17-9ae0-6f00f6080adb)

### Box (Cloud - 500 GBs through UW-Madison)

[https://support.box.com/hc/en-us/articles/360043697194-Installing-Box-Sync](https://support.box.com/hc/en-us/articles/360043697194-Installing-Box-Sync)

## How to Recovery Your Data

### Windows - FileHistory (Local)

[https://support.microsoft.com/en-us/windows/backup-and-restore-in-windows-352091d2-bb9d-3ea3-ed18-52ef2b88cbef#WindowsVersion=Windows_10](https://support.microsoft.com/en-us/windows/backup-and-restore-in-windows-352091d2-bb9d-3ea3-ed18-52ef2b88cbef#WindowsVersion=Windows_10)

### MacOS - Time Machine (Local)

[https://support.apple.com/guide/mac-help/restore-files-mh11422/mac](https://support.apple.com/guide/mac-help/restore-files-mh11422/mac)

### Google Drive, OneDrive, Box

Go to the corresponding website and all of your lost files should still be there!

Google Drive: [https://drive.google.com/](https://drive.google.com/)

OneDrive: [onedrive.live.com/](onedrive.live.com/)

Box: [https://uwmadison.account.box.com/login](https://uwmadison.account.box.com/login)

## Privacy Best Practices

### Password Managers

Have any of your passwords been leaked in existing data breaches? Let's check:

https://haveibeenpwned.com/

#### BitWarden - Easy to Use and FOSS

Steps to install on Windows, MacOS, iOS, and Android

Installing BitWarden on your computer:

1. [Create a free account.](https://bitwarden.com/pricing)
2. [Import you existing passwords into Bitwarden.](https://bitwarden.com/help/article/import-data/)
3. Install Bitwarden browser extension into your preferred browser.
	* Firefox: https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/
	* Chrome: https://chrome.google.com/webstore/detail/bitwarden-free-password-m/nngceckbapebfimnlniiiahkandclblb
	* Safari: https://bitwarden.com/help/article/install-safari-app-extension/
4. Install/Setup Bitwarden on your mobile device:
	* https://bitwarden.com/help/article/getting-started-mobile/

### Platform Tracking

An immense amount of data is collected about us across every single website we visit and every app we open. While it is impossible to prevent all tracking performed by these services, it is possible to minimizing the tracking. Generally, social media platforms are the biggest culprits of data harvesting with Facebook, TikTok, WhatsApp, and Instagram retaining the most information about user action. There are a series of steps we can take to minimize tracking on these platforms are across these platforms. The recommendations below are listed in order from easiest to most difficult to implement.

#### *(Very easy)* Preventing cross-platform tracking across websites

* Prevent cross-site tracking cookies by using the [PrivacyBadger](https://privacybadger.org/) browser add-on developed by the Electronic Fronteir Foundation.
* Use Firefox/Safari instead of Google Chrome. Both of these browsers have more consumer friendly privacy policies than Google Chrome.
* Disable unnecessary permissions for apps on your phone.
	* iOS: Settings --> Privacy
	* Android: Settings --> Privacy --> Permission Manager
* Limit ad-tracking in iOS: Settings --> Privacy --> Tracking (make sure this is disabled)

#### *(Easy but takes time)* Changing privacy settings of social media services that you may use

* [Follow this guide to limit how much information is public about your Facebook profile](https://www.consumerreports.org/privacy/facebook-privacy-settings-a1775535782/#guard
)
* [Follow this guide to limit how much information is public about your Instagram profile](https://www.consumerreports.org/privacy/instagram-privacy-settings-a3036233134/
)

Using Signal or ether E2E chat apps

