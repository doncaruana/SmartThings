# SmartThings
For Smart Things

Some things I've learned abuot device handlers...

All DTHs should just be set to encapsulate commands for security in case they are in secure mode (check if secure, encapsulate if so).<br/>
Devices connected securely will ignore unencapsulated commands<br/>
Battery-powered devices won't accept commands unless they are awake.<br/>
commands issued while sleeping are lost<br/>
Wakeup Interval is set to 4 hours by hub on inclusion<br/>
wakeupIntervalGet doesn't seem to work<br/>
can't set default value for enum in preferences<br/>
configuration parameter values have to use a variable or use scaledConnfigurationValue if using a number directly (even if size is 1)<br/>
$ for variable, use {} inside variable for inline calcs<br/>
time is in epoch time (milliseconds since 1970)<br/>
Tiles can't be changed programmatically<br/>


Device fingerprints:<br/>
--Aeotec recessed door sensor-- zw:Ss type:0701 mfr:0086 prod:0102 model:0059 ver:1.13 zwv:3.92 lib:03 cc:5E,86,72,98 ccOut:5A,82 sec:30,80,84,70,85,59,71,7A,73 role:06 ff:8C00 ui:8C00<br/>
--Aeotec Dry Contact-- zw:S type:0701 mfr:0086 prod:0102 model:0061 ver:1.04 zwv:4.05 lib:03 cc:5E,86,72,85,59,73,71,84,30,80,70,7A ccOut:5A,82 role:06 ff:8C05 ui:8C05<br/>
--SmartSense Multipurpose Sensor-- 01 0104 0402 00 08 0000 0001 0003 0020 0402 0500 0B05 FC02 01 0019<br/>
--Smartsense Motion Sensor--	01 0104 0402 00 07 0000 0001 0003 0020 0402 0500 0B05 01 0019<br/>
--GE 12724 Dimmer-- zw:L type:1101 mfr:0063 prod:4944 model:3031 ver:3.37 zwv:3.67 lib:06 cc:26,27,73,70,86,72,77<br/>
--SmartSense Power Outlet--	01 0104 0100 00 07 0000 0003 0004 0005 0006 0B04 0B05 01 0019<br/>
--GoControl GD00Z-4-- zw:Ls type:4007 mfr:014F prod:4744 model:3530 ver:2.01 zwv:4.05 lib:03 cc:5E,5A,72,73,98 sec:86,85,59,66,22,71 role:05 ff:8C06 ui:8C06<br/>
