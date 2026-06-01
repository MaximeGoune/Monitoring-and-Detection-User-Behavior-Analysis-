# Monitoring-and-Detection-User-Behavior-Analysis-
Monitoring-and-Detection-User-Behavior-Analysis with Kibana


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
