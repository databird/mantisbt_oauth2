# mantisbt_oauth2

To enable XOAUTH2 (ie for O365), you can replace file "IMAPProtocol.php" in folder "/plugins/EmailReporting/core_pear/Net" by the one available in this repository

To obtain your tenantId & clientId, you can follow _(dont have a look on PHP sections)_ :
  https://vielhuber.de/en/blog/access-with-php-to-exchange-office-365/
  
  Or
  
  https://learn.microsoft.com/en-us/entra/identity-platform/quickstart-register-app
  https://learn.microsoft.com/en-us/exchange/client-developer/legacy-protocols/how-to-authenticate-an-imap-pop-smtp-application-by-using-oauth#use-client-credentials-grant-flow-to-authenticate-smtp-imap-and-pop-connections

Then, on Mantis EmailReporting configuration, set Username as following format :
  {email}|{tenantId}|{clientId}
(separator : pipe)

And select "XOAUTH2" on Authentication method

![mantis_xoauth2](https://github.com/databird/mantisbt_oauth2/assets/32749489/8b3c983e-0b6b-46e2-b5e9-6561876fef60)

Enjoy !
