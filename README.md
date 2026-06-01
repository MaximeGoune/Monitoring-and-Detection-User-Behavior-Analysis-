# Monitoring-and-Detection-User-Behavior-Analysis-
Monitoring-and-Detection-User-Behavior-Analysis with Kibana


***Detecting Anonalous Account Activity

Access the Kibana web interface by, in Firefox, entering 127.0.0.1:5601 in the address bar, 

<img src="https://i.imgur.com/jaM2tUM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

 Click on the triple bars in the top-left, scroll-down and navigate to Management > Stack Management, then click on Kibana > Index Patterns.
<img src="https://imgur.com/3Y5rFZf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

This should result in the pattern showing 266 fields for auditbeat.

<img src="https://imgur.com/c7dOOD2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

you’re going to add one additional index pattern. For this click Index Patterns again (from the left menu), then on Create index pattern again, enter filebeat* as the Name (you should not have to type in the *), and choose @timestamp again from the drop-down.

<img src="https://imgur.com/j5ZWqBo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

Filter base on period

<img src="https://imgur.com/n33BpTK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<img src="https://imgur.com/VvHdu52.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
To better isolate events, in the Search field names box on the left side of the window. enter event.action.

This will filter the fields displayed below the text box. Once event.action is found hover over it, this will bring up a plus sign, click on this plus sign.

To better isolate events, in the Search field names box on the left side of the window. enter event.action.

This will filter the fields displayed below the text box. Once event.action is found hover over it, this will bring up a plus sign, click on this plus sign.

Note: If no event.action shows, the incorrect filter is likely chosen. Ensure auditbeat* is selected.

Repeat the process shown in task 14 with the following fields, adding each one: event.outcome, auditd.data.cmd, auditd.summary.actor.primary, auditd.summary.actor.secondary, process.executable, file.path, process.title, and message
event.outcome	                   Whether the action succeeded or failed
auditd.data.cmd	                  Command executed by the user
auditd.summary.actor.primary	      Primary user involved
auditd.summary.actor.secondary	    Secondary user involved
process.executable	              Full path of the executable that ran
file.path	                      File affected by the event
process.title              	Command line used to start the process
message	Human-readable event description

<img src="https://imgur.com/PuQndGw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://imgur.com/NgKFcSL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<img src="https://imgur.com/KZlmxb4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />

<img src="https://imgur.com/Gp3fvrB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
