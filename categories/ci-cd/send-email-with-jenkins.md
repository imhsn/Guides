## Send Email with Jenkins

### Environment
- Email Extension Plugin
- Jenkins
- Maven
- git
- Oracle JDK

### Install Email Extension Plugin

Install *Email Extension Plugin* at plug-in install page of Jenkins.

### Configure System

### “Jenkins Location” section

Enter valid email address to “System Admin email address” 

### “Extended Email Notification” section
- Enter your SMTP server name to “SMTP server”
- Click “Advanced”
- Click “Use SMTP Authentication”
- Enter the required information
- Enter your email address to “Default Recipients”

### “Email Notification” section

- Enter your SMTP server name to “SMTP server”
- Click “Advanced”
- Click “Use SMTP Authentication”
- Enter the required information
- Check “Test configuration by sending test email"
- Click “Test configuration” to send a test email"
- Click “Save” in the bottom of the page

#### [Get an app pwd from google](https://www.lifewire.com/get-a-password-to-access-gmail-by-pop-imap-2-1171882)

### Configure a project to send an email at every build

- Click “Add post-build action”
- Click “Editable Email Notification”
- Click “Advanced Settings…”
- Click “Add Trigger”
- Click “Always”
- Then Save

### Test Run

- Click “Build Now” 
- Check Console output and received email

### Reference

- [Send email from a printer, scanner, or app](https://support.google.com/a/answer/176600?hl=en)
