# Google Trends Slackbot
Hackathon Demo in UBC Local Hack Day 2018

A slackbot that randomly picks a Google Trends item and tells the summary of the result.

**Relying on Slackbot for the GUI is the biggest mistake**
- Multi-line message is still not supported as of December 01, 2018 
(earliest request started in 2015 https://twitter.com/slackhq/status/592923143309787136?lang=en)
- No custom styling for the option dropdown in interactive messages. If an item is too long, it is trimmed with '...'
- The request structures from Slack to your own server can be quite different, 
e.g. normal message (`application/json`) vs interactive messages (`application/x-www-form-urlencoded` with a key `payload`).