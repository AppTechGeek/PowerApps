# File Uploader
> Upload files to a SharePoint Online library from a PowerApps canvas app using Power Automate Flow

![(./../FileUpload/UploadFiles.png)](./../FileUpload/UploadFiles.png)

### Custom Properties
![(./../FileUpload/UploadFilesProperties.png)](./../FileUpload/UploadFilesProperties.png)

### Implementation
- To show/hide the attachment dialog, add an icon or button to your application's screen and set the OnSelect property to:
```
  //Hide attachment dialog
  UpdateContext({locShowAttachmentDialog: !locShowAttachmentDialog})
```
- Set the component's Visible property to locShowAttachmentDialog
- To the Save OnSelect and Cancel OnSelect custom component properties add the statement below in order to hide the component when the corresponding icons are selected
``` UpdateContext({locShowAttachmentDialog: false})
