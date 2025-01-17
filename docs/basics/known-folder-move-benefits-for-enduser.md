# Known Folder Move (KFM) Benefits for Endusers 

A little recap, KFM is a OneDrive sync feature that works with Windows 7, Windows 8/8.1, Windows 10. This feature allows business users to automatically backup/redirect their Windows clients Desktops, Documents and Pictures folders to OneDrive for Business. Personally I've only used and deployed KFM to Windows 10 platform. 

## Benefits of KFM:  

*   Automatic Backup of content on your device
*   You really don't need to worry about uploading your content, as everything you put on the Desktop/Documents/Pictures is uploaded automatically
*   Protection against &quot;ransomware&quot; attack on the device because OneDrive support in place file restore 
*   Seamles switching to another device and continue where you left your files
*   Dependent on your licensing, you will get at least 1 TB of personal backup storage
*   If your business are small without central IT, users can turn on this feature in a few easy steps
*   If your business are bigger and have central IT, you can turn on this with GPO's
*   If you have used Offline files before you might have experienced that it's a bit difficult to know if it have synchronized correctly with the file share you have been configured against. In my opinion it's a lot easier to catch synch issues with OneDrive and esier to fix.
*   KFM is a &quot;killer&quot; feature when migrating personal file shares to OneDrive



## How do you turn it on:

Follow this [Guide]( https://support.office.com/en-us/article/back-up-your-documents-pictures-and-desktop-folders-with-onedrive-d61a7930-a6fb-4b95-b28a-6552e77c3057?ui=en-US&rs=en-US&ad=US) at Microsoft support.


![KFMOptions](../../images/known-folder-move-benefits-for-endusers/KFM01.png)

![KFMOptions](../../images/known-folder-move-benefits-for-endusers/KFM02.png)


## Tips & Tricks to be aware of:

Here is a few things I've experienced with this feature that might help in case of troubleshooting:

1. KFM is similar to Windows Offline Files or folder redirection. Meaning they don't work well together so you need to turn of Offline files before using KFM. 
2. KFM uses your OneDrive site as storage, meaning the user account in question have to be "Site Collection Owner" of that OneDrive site, this is normally the case but if not then KFM won't work.
3. .PST files is not supported. This is often the case when users have limited mailbox storage on premises, normally we export the mailbox as backup and stores this in the Documents folder leading to error when activating the feature.
4. OneNote files outside of OneDrive is not supported. This is the case if you have used OneNote locally before KFM normally the OneNote apps stores the files in the Documents folder. Move the OneNote files to OneDrive first.
5. Beware of the 100,000 items recommended limit, if you are using KFM while synching SharePoint libraries. Performace decreases as the totalt numbers goes up, this limit also depends on your client device performance.  

---



**Principal author**: Jimmy Hang, MCT, MCSE: Productivity 

**LinkedIn**: https://www.linkedin.com/in/jimmyhang/

**Blog**: https://hangconsult.com

**Source**: https://docs.microsoft.com/en-us/onedrive/redirect-known-folders
