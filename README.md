# LiveSupport
Live Customer Service communication / chat tool. 

About:
------
-Designed with PHP pages that link to perl (cgi) chat pages.
-Uses a mySQL database to store logged in users, admins and room numbers.
-Uses php & file writing to store user logs, browser and os details collected.
-Users perl script to save chatroom logs.

Chat Logs:
-----------
The chat logs are currently saved at, per account: 
http://www.mbase.com.au/~helpbase/cust_serv_chat/chat/$account/


Original chat code from:
------------------------
BlueChat Copyright © 1999,2001 by Robert Fogt
http://www.bluesparks.com/                  webmaster@bluesparks.com

BlueChat is Free software. Use it at your own risk. You may use BlueChat in its unmodified form free of charge. If you modify BlueChat, please place a link to http://www.bluesparks.com/
somewhere on your site.

Note: The original BlueChat perl script has been taken back to very basics and therefore cannot be tied with the original script anymore. Therefore no risk of copyright.

-=>Basic Chat Setup<=-

Folder:
cust_serv_chat      -(directory 755) 
cust_serv_chat/chat -(chat directory 777)

Files included:
-chat.cgi         -main chat code
-chatbar.cgi      -user/customer chatbar
-chatbar_a.cgi    -admin chatbar

(Chmod all the cgi files 755)


NOTE: If the path to perl is not /usr/bin/perl then you will need to edit
each of the cgi files and change the first line to your perl path.

NOTE: If your server requires cgi files to be located in your cgi-bin
directory, you will have to do some additional setup.
The chat directory cannot be inside the cgi-bin directory. So create the
chat directory outside the cgi-bin directory and edit bc_chat.cgi and
change the $chatpath and $chaturl variables to where the chat directory is.



-=>Basic Cust Serv PHP files Setup<=-

Folder:
cust_serv 
cust_serv/images

Files included:
-all files in the folder must be keep together.
-images, there are a variety of required graphics here.

 *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  * 
*  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  * 

USING THE SYSTEM:
------------------
------------------

Login to accounts:
------------------
http://--your domain location--/cust_serv/
Username: as provided per account.
Password: as provided per account.
Use this area to customise color, logos, etc for an individual account.


Login to admin area, add users (accounts):
-------------------------------------------
http://--your domain location--/cust_serv/add_login.phtml
Username: admin
Password: (check via WebMin)


Graphics and coding:
------------------
You can find a sample graphic here:
http://www.mbase.com.au/~helpbase/cust_serv/images/live_support.gif
(Use this as an idea of other graphics for other websites)

Coding:

The following coding must go along with your graphic when placed into your web page.

	<script language="JavaScript">
	<!-- Hide the script from old browsers --
	function openNewWin1() {
	msgWindow=window.open('u_login.phtml?	account=**ACCOUNT**&location=**LOCATION**','Representative','toolbar= 0,location= 	0,status=0,menubar= 0,scrollbars= 0,resizable= 1,copyhistory= 1,width=250, height=300');
	if(navigator.appName.indexOf("Netscape")!=-1&&parseInt(navigator.appVersion)==4)
	msgWindow.resizeTo(250,400);
	}
	// finish hiding -->
	</script>

	a href="javascript:openNewWin1();"><img src="** URL TO GRAPHIC **" border="0" 	alt="** COMPANY / ACCOUNT NAME ** Live Customer Service"></a>


(Note: no breaks between continuing lines)

Fill in the blanks as required above:
**ACCOUNT**  = place the account name that is for this LiveSupport account.

**LOCATION** = put the page name or site location here (one word identifier). OPTIONAL, can 		   leave blank.

** URL TO GRAPHIC ** = url to the graphic that was created to advertise on your site.

**COMPANY / ACCOUNT NAME** = Your company name or account name to highlight your company in the    	         text description when mousing over the logo. Optional, can leave blank.


 *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  * 
*  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  *  * 


By: Nadia Kerr (formerly Nadia Lakatos)
15/03/2002
