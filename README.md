SmartThings TED5000 Device-Type
===================

## INSTALLATION

1. Connect to the web admin interface of your TED5000 (typically available at //TED5000 on your local network and make sure password protection is turned on for all access. See TED5000_Settings.png for an example.
 
2. Configure your firewall so that the TED5000 is visible outside your home network. This topic is beyond the scope of this code, but at the end you should be able to connect to your TED5000 from outside your home network     (your phone's browser is a good option for this if you turn off wifi). You'll test with a URL like this:
 
               http://YOUR_IP:YOUR_PORT/api/LiveData.xml
               
	But the portion you'll need for the preferences is just:
               
               http://YOUR_IP:YOUR_PORT
 
  
3. Don't even think about proceeding until the above is working! Create a new device type (https://graph.api.smartthings.com/ide/devices)
  
  	    Name: TED5000
		Author: badgermanus@gmail.com
      	Capabilities:
				Energy Meter
				Polling
				Power Meter
				Refresh
 
4. Create a new device (https://graph.api.smartthings.com/device/list)  
  
 		Name: Your Choice
 		Device Network Id: Your Choice
 		Type: TED5000 (should be the last option)
 		Location: Choose the correct location
 		Hub/Group: Leave blank
 
5. Update device preferences  
  
 		1.	Click on the new device to see the details.
 		2.	Click the edit button next to Preferences
 	    3. 	Fill in your device access information - username, password & URL
 
