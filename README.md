Hourly automation
•	Schedule: every hour on the hour, Eastern time. The first run is today at 1:00 PM ET.
•	What it checks: each run looks at NWS active alerts for JFK, plus SIGMETs, Convective SIGMETs, AIRMETs and Center Weather Advisories whose area covers the airport.
•	When it notifies you: only when a new hazard appears or an existing one changes. Quiet runs just log a one-line “no new hazards” result. Notifications are set to go to your phone as push alerts.
•	Where it runs: in its own separate conversation, using the light mode to keep each run cheap.

Web version of the script
The page is in the attached preview. You can type an airport code (like KDEN) or a latitude and longitude, or press “Check now,” and it refreshes itself every 15 minutes. Results are grouped into NWS alerts, SIGMETs/AIRMETs and Center Weather Advisories, each with the full alert text.
I tested it on the hosted preview with JFK and Denver, which had no active hazards. I also tested a point in Texas that sat inside a real active Convective SIGMET, and it showed it correctly with altitudes, valid times and the full text.
Limitation to know about: the Aviation Weather Center blocks browser pages from fetching its data directly. So the page gets SIGMETs, AIRMETs and advisories through a small relay program I’m running alongside it. If that relay goes offline, those sections will show an error, but NWS alerts will still load because the page fetches those directly. The hourly automation doesn’t use the relay, so it isn’t affected.
