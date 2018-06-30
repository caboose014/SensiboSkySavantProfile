This profile is created to control any Sensibo (https://sensibo.com) unit that uses Sensibo's API. This has been written to work with the Savant Pro 8 app. Not all featurs of the API are available due to limiting UI design in the Pro 8 app.

You *MUST* assign 'https://home.sensibo.com' to the wire in RacePoint - the 'https://' is very important here.

*DONT* change the thermostat address in the data table. 
You may enable/disable the features of your unit using the check boxes.
1 profile should be placed for each unit you want to control. Data table entries will be added automaticly.

You need to generate an API key using your Sensibo account online. Log in here: https://home.sensibo.com/me/api and generate your api key.
If you need to find your unit's ID, open Terminal and use the following command (ensuring to put in your acutal api key at the end):
	> curl "https://home.sensibo.com/api/v2/users/me/pods?apiKey=yourapikeyhere"
This will return a json array of all the units on your account. Select the one you want to conrol for the step bellow.

Update the state varables in RacePoint. Inspect your Sensibo component, from the 'Show' dropdown box select "State Vairables".
Change api_key to your own api key
Change unit_id to the id of the unit you wish to control
Change ThermostatCurrentSetPointUnits to F or C depending on which units you want to control your unit in.

After you upload you can check the state 'ThermostatCurrentName' to see if the units match the zones you have assigned them. This will display the name you have assigned during the seutp on your Sensibo Sky unit.



If there are feautres or commands you would like added to the profile, please let me know and I'll do my best to get them put in.
