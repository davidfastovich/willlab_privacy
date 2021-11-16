# Data Privacy and Backups: Best Practices

After this lab meeting you should have a laptop and phone that is actively being backed up, with stored and synchronized passwords, that limits ad-tracking across the internet.

*Goals:*

1. Reduce digital footprint
2. Start using a password manager
3. Start peforming real-time cloud backups

# 1. Reduce digital footprint

An immense amount of data is collected about us across every single website we visit and every app we open. While it is impossible to prevent all tracking performed by these services, it is possible to minimizing the tracking. Generally, social media platforms are the biggest culprits of data harvesting with Facebook, TikTok, WhatsApp, and Instagram retaining the most information about user action. There are a series of steps we can take to minimize tracking on these platforms are across these platforms. The recommendations below are listed in order from easiest to most difficult to implement.

## *(Very easy)* Preventing cross-platform tracking across websites

* Prevent cross-site tracking cookies by using the [PrivacyBadger](https://privacybadger.org/) browser add-on developed by the Electronic Fronteir Foundation.
* Use Firefox/Safari instead of Google Chrome. Both of these browsers have more consumer friendly privacy policies than Google Chrome.
* Disable unnecessary permissions for apps on your phone.
	* iOS: Settings --> Privacy
	* Android: Settings --> Privacy --> Permission Manager
* Limit ad-tracking in iOS: Settings --> Privacy --> Tracking (make sure this is disabled)

## *(Easy but takes time)* Changing privacy settings of social media services that you may use

* [Follow this guide to limit how much information is public about your Facebook profile](https://www.consumerreports.org/privacy/facebook-privacy-settings-a1775535782/#guard
)
* [Follow this guide to limit how much information is public about your Instagram profile](https://www.consumerreports.org/privacy/instagram-privacy-settings-a3036233134/
)

## *(Advanced)* Move to social network/chat apps that are end-to-end encrypted

End-to-end (E2E) encrypted messages mean that any messages you send to a receivers cannot be read by the service that is delivering the message. For instance, WhatsApp and iMessage both use E2E encryption for their messages so that means neither Facebook nor Apple can read the contents of the messages that are sent using their services. This is fantastic, but not all messaging platforms are created equally. WhatsApp still collectings a tremendous amount of data from their users outside of the contents of messages while Apple claims to keep as little information as possible. This does not mean I endorse using iMessage as a secure chat platform. Rather, it illustrates how complicated the landscape is when it comes to data privacy on messaging platforms. I suggest using platforms that use E2E encryption for messages and are *transparent* about the data they retain from their customers. Apple falls into the opaque category, while a service like Signal is much more transparent. Moreover, Signal is entirely open source so third parties can audit the code to make sure Signal is not up to anything nefarious. Lastly, there is the category of messaging services that claim to privacy oriented and transparent, like Telegram, while not being either in practice. By default, no messages on Telegram are E2E encrypted - conversations must be made "Secret" to enable encryption. Additionally, their encryption algorithm is not as well regarded as the industry standard algorithms used by Signal.

Making this transition is difficult because you need to get your friends and family aboard the Signal ship to maintain that all of your digital conversations are private.

Instructions for installing Signal: [https://support.signal.org/hc/en-us/articles/360008216551-Installing-Signal](https://support.signal.org/hc/en-us/articles/360008216551-Installing-Signal)

# 2. Start using a password manager

Have any of your passwords been leaked in existing data breaches? Let's check:

https://haveibeenpwned.com/

One of the biggest internet security risks we all share are old, simple, and reused password littered across a variety of sites and accounts. Passwords **should** be long and complex, but that makes them very difficult to remember. This is where password managers come to the rescue! Password managers are programs that allow you to create and store long, complex passwords without having to remember them. Generally, password managers operate by creating a database that is encrypted by a single "master" password. Once you type in your master password you unlock the database and have access to all of the stored passwords. Many password managers exist and all offer unique features, benefits, and costs. Ideally we want a password manager that is secure and transparent, stored in a way that only you can ever see the contents of your password database. There are two options that fulfill these requirements: Bitwarden and KeePass. KeePass is the gold standard for password security. KeePass databases are entirely offline (not stored on any servers) encrypted by advanced algorithms that make cracking your database encryption impossible. However, KeePass can be hard to setup and even harder to make work across multiple devices. This is where Bitwarden comes in. Bitwarden is a company and password manager that simplifies the process quite a bit. Bitwarden automatically syncs your passwords across all of your devices making setting up and using your password database very simple! Unfortunately, this comes with risks. While your databse is encrypted, it is still stored on their servers which does contain some risk, although minimal. Given all of the transparency and quality of life benefits of Bitwarden, thats what we'll be setting up today! Follow the instructions below to install Bitwarden on your computer:

1. [Create a free account.](https://bitwarden.com/pricing)
2. [Import you existing passwords into Bitwarden.](https://bitwarden.com/help/article/import-data/)
3. Install Bitwarden browser extension into your preferred browser.
	* Firefox: https://addons.mozilla.org/en-US/firefox/addon/bitwarden-password-manager/
	* Chrome: https://chrome.google.com/webstore/detail/bitwarden-free-password-m/nngceckbapebfimnlniiiahkandclblb
	* Safari: https://bitwarden.com/help/article/install-safari-app-extension/
4. Install/Setup Bitwarden on your mobile device:
	* https://bitwarden.com/help/article/getting-started-mobile/

# 3. Start peforming real-time cloud backups

## 3-2-1 Golden Rule of Data Backup

![Alt text](https://www.itguys.com/wp-content/uploads/2018/02/321Rule.jpg)

If you follow this rule the likelihood of losing any data permanently is *incredibly* low, however it can be a bit of a pain to setup. So what does this mean for researchers and different career stages?

**Principal investigator** 

If you're running a lab and generating lots of primary data, you should stick to rule very strictly. Ideally, you would have a departmental storage server that has multiple copies of this data and a copy of this data somewhere offsite using a cloud storage provider or an offsite data bank.

**Graduate/Undergraduate Student**

This is my current career stage, so I can give some guidance on my data backup practices! The 3-2-1 rule is always recommended, but given the high startup cost I chose to simplify it a bit for myself. I backup my data onto two local devices and one cloud storage provider. I have a local backup because it makes recovering any lost data *much* faster. For instance, imagine losing/accidentally deleting 100 GBs of data if you're computer suddenly crashes. If this data was only stored in the cloud, such as with Google Drive, it could take anywhere from 1 to 5 hours to recover all of your data, but if the data was stored on an external hard drive or you could be up and running in as little as 15 minutes!

Another great advantage of backing up your data is version tracking! I've made plenty of changes to manuscripts that I wanted to undo and with realtime backups I can easily revert a document to a previous version. Cloud storage providers and local backups support this feature, and it can be a lifesaver!

## Today: How to Backup Your Data with a cloud provider

After todays lab meeting you should have a folder on your computer that contains all of your important documents that is backed up to the cloud in real-time. That means the second you make an edit on a Word document and hit save, it starts to get uploaded to your cloud provider of choice. The name of this folder varies by operating system and cloud storage provider. For instance, on a Mac Google Drive creates a new volume that appears under "Favorites" or "Volumes" on the left hand side of Finder. In contrast, on a Windows computer Google Drive creates a "Google Drive" folder in My Documents where all of your Google Drive files live. The contents of these folders are actively backed up to Google Drive which means that after you install and setup your cloud service of choice, you'll have to move (not copy) all of your important data into these folders to that they get backed up. Additionally, when you create new documents/pictures/etc., you'll need to save them to this folder.

Each cloud storage provider has their own benefits and costs, luckily if you are a part of the UW-Madison system as a student, researcher, or faculty member you get access to several services entirely for free! I don't really have any recommendations as they all share important features: real-time backups and version history. However, there are some considerations. For instance, OneDrive is *baked into* Windows which means you won't have to install anything - all you have to do is login to OneDrive program on your computer using your @wisc.edu email address. Similarly, iCloud Drive is baked into MacOS. For reference, I use Google Drive because I'm a big fan of Google Photos as a way to backup and access all of my photos across any device but you can't make a wrong decision. Follow the steps below to get your important data backing up to the cloud:

1. Install a cloud backup service (all below are free through UW-Madison):
	* [Google Drive](https://support.google.com/a/users/answer/9965580?hl=en)
	* [OneDrive](https://support.microsoft.com/en-us/office/turn-on-onedrive-backup-4e44ceab-bcdf-4d17-9ae0-6f00f6080adb)
	* [WiscBox](https://support.box.com/hc/en-us/articles/360043697194-Installing-Box-Sync)
2. Locate the folder/volume created during the installation process that get's backed up
3. Move all of your important data into that folder
4. Wait until all data is uploaded to the cloud service (may take 30 minutes to hours depending on how much data you have)
5. Done! Be sure to only edit files within this folder/volume to ensure that your cloud backup is always up-to-date. That is, you don't accidentally create a file in "Documents" that isn't backed up.
6. In case you need to revert any changes or recover any lost data simply reinstall the program, login, and everything will start syncing. You could also go to each programs corresponding website to see your backed up data.
	* [Google Drive](https://drive.google.com/)
	* [OneDrive](onedrive.live.com/)
	* [WiscBox](https://uwmadison.account.box.com/login)

## Homework: Setup a local backup using these guides

### Windows - FileHistory (Local)

[https://www.groovypost.com/news/microsoft-windows-10-cumulative-update-kb3081438/](https://www.groovypost.com/news/microsoft-windows-10-cumulative-update-kb3081438/)

### MacOS - Time Machine (Local)

[https://support.apple.com/en-us/HT201250](https://support.apple.com/en-us/HT201250)

### Windows - FileHistory Data Recovery

[https://support.microsoft.com/en-us/windows/backup-and-restore-in-windows-352091d2-bb9d-3ea3-ed18-52ef2b88cbef#WindowsVersion=Windows_10](https://support.microsoft.com/en-us/windows/backup-and-restore-in-windows-352091d2-bb9d-3ea3-ed18-52ef2b88cbef#WindowsVersion=Windows_10)

### MacOS - Time Machine Data Recovery

[https://support.apple.com/guide/mac-help/restore-files-mh11422/mac](https://support.apple.com/guide/mac-help/restore-files-mh11422/mac)

