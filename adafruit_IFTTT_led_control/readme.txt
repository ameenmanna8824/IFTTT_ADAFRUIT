Steps to make your NodeMCU compatible with Arduino IDE:
1.Download Arduino IDE
2.Go to Tools>Boards Manager
3.Search for ESP8266 board and download it.
4.After download ,try programming NodeMCU by using simple blink program.
5.If blink works,then you are good to go.

IFTTT/Adafruit project:(In Arduino IDE)
1.Include Adafruit MQTT library in arduino IDE
2.In your program/code make sure to enter:
	a.SSID (wifi username)
	b.Password (Wifi password)
	c.AIO username (from adafruit.io dashboard)
	go to your dashboard and you see yellow button 
	with the name your SECRET ADAFRUIT I/O key.
	d.AIO KEY (from adafruit.io dashboard)
	e.Change your feed name at the end of line no 29 of code.
LINE 29:Adafruit_MQTT_Subscribe onoffbutton = Adafruit_MQTT_Subscribe(&mqtt, AIO_USERNAME "/feeds/BANGALORE");
In my case ,feed name is BANGALORE,you put your feed name

  AND MOST IMPORTANTLY ,IF EVER YOU ARE USING MOBILE HOTSPOT,TURN ON YOUR HOTSPOT
IF YOU WANT TO FIX THIS PERMANENTLY,IT IS ADVISED TO CONNECT ESP TO WIFI ROUTER 


(In Adafruit.io)
1.Create an Adafruit account.
2.Create a new dashboard and in dashboard click on the blue button(CREATE a NEW BLOCK)
3.Select the first Toggle switch>next >finish.
4.Now click on your toggle switch and check if it works

(In IFTTT)
TO connect to Google Assistant Service:
1.Download IFTTT app and Google Home app in your Smartphone and login using your Google account.
2.Onve you open the Google Home app,click on the settings button .
3.Now in the Settings menu click on "Works with Google" and Now seach for IFTTT service.
4.Click on IFTTT service and click on continue and you might have to give in your Google account details again
5.And Now you might get No Devices Connected.
6.Once you get no devices , then try creating a neww Applet and your Google Assistant is now connected


To create an APPLET:
2.Click on create and create an applet
3. If(THIS) THEN (THAT)
	THIS -GOOGLE ASSISTANT
	THAT -ADAFRUIT(VALUE TO SAVE SHOULD BE 1 FOR "ON APPLET")
		      (VALUE TO SAVE SHOULD BE 0 FOR "OFF APPLET")

EVEN AFTER TRYING IF YOU FAIL,FEEL FREE TO ASK ME
