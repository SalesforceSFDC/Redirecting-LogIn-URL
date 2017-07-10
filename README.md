# Redirecting-LogIn-URL
As Bob said, not 100% possible, since you can't guarantee the page they'll land on. You can influence their default login page by setting a page as the default (Setup > Create > Apps > Edit), which gives them a default page to land on when they switch to the app or login (so you could set it to cases, for example). Taking that a step further, you could create a Visualforce page (and corresponding tab) that takes them to ANY page you can imagine when they log in. This will only work if startURL is not specified (which would occur if they used login.salesforce.com, but not if they started from a bookmark or the login page shown after a user's session expires). So, you can heavily influence where they land, but any user that regularly uses bookmarks or lets their session expire without logging out probably won't benefit from your attempts.


##
Redirecting LogIn URL to last page used prior to session expiration.  

It is not 100% possible without a custom Visualforce page to guarantee user will land on the last activity page prior to session expiring.  

The current process takes the user to the Home Tab once the user logs back into SFDC after the session expires.  We can influence their default login page by setting a page as the default (Setup > Create > Apps > Edit), which gives them a default page to land on when they switch to the app or login.  We could create a Visualforce page (and corresponding tab) that takes them to ANY page when they log in.  This will only work if startURL is not specified (which would occur if they used login.salesforce.com, but not if they started from a bookmark or the login page shown after a user's session expires).  So, we can heavily influence where they land, but any user that regularly uses bookmarks or lets their session expire without logging out probably won't benefit from the attempts.
##
