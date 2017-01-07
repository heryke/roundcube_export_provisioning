Provisioning Export Plugin for Roundcube
========================================

Roundcube plugin that generates an email provisioning file.

## Installation
You can download the plugin directly form this repository, or via the [plugin repository for Roundcube](http://plugins.roundcube.net/).

## Usage
You can find a new settings tab named "Provisioning". From there you only have to choose an identity (or use the default one) and click on the dowload links.
One download link is generating a .mobileconfig file, suitable for iOS / OSX devices.
The other download link is generating a .iaf file, suitable for Outlook Express and Windows Live Mail.

## Plugin configuration
Plugin configuration is optional. If you need it, you can create a config.inc.php file inside the plugin folder, to alter parameters like IMAP or SMTP host and port. See config.inc.php.dist as an example.

## iOS provisioning
Send the .mobileconfig file via email (it's not working via iMessage), then open it. The device will ask for confirmation before installing the profile, that will appear as unsigned. Just click on "Install" and enter the access code if asked. Another confirmation is needed, so click in "Install" again. And... guess what? iOS is asking a third time if you really want to install. Click "Install", wait some seconds for installing, then click on "End".

## OSX provisioning
Just open the file, the profile installation will ask you for confirmation two times. Confirm and enjoy.

## Outlook Express provisioning
"Tools / Accounts", then click "Import" and choose the correct .iaf file.

## Windows Live Mail provisioning
"Tools / Accounts", then click "Import" and choose the correct .iaf file.

## Support
- Please report any bugs [here](https://github.com/paspo/roundcube_export_provisioning/issues/).
- Fork and pull requests are also welcome.

## TODO
- More localization.
- Option for sending the provisioning file via email.

## License
See the LICENSE file.
