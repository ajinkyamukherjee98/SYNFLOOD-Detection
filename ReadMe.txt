Steps To Open  and Run the project.

1.	Import the TCP dump file to Wireshark.
2.	The local snort.conf file was changed by making the $HOME_NET var as a list of Destination IP addresses found in the file using Wireshark.
3.	Commands to run the rules along with 
a.	Edit the local.rules file: sudo vim /etc/snort/rules/local.rules
b.	Validate the rule configuration: sudo snort -T -c /etc/snort/snort.conf 
	     c. Run the tcpdump file with our custom rules: sudo snort -r /home/Ajinkya/Desktop/	ssignment1/outside.tcpdump -c /etc/snort/snort.conf -A console

To Import Snort Files:
1. Chopse the  Snort log File you want to open:
	Example: If you want to open snort.logR1T5P1.1605547494  Right click on the file, open with Wireshark.
This will help view the alert logs generated by the rules

The log files are saved as snort.log.RuleNumberThresholdvalueSamplingPeriod.Number

