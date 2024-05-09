# PenTest-auto
Automated penetration testing script using different attack vectors


# Introduction
The script will map your current network and find different attack vectors. Based on the active hosts, open ports will be identified. 

Next, the script will find users with weak passwords and potential vulnerabilities based on service detection.

The user will be prompted to provide a list of Usernames and Passwords. The list will be used to check for weak passwords in the network services.

Finally, the user may view the results in the command line or, view it in a saved report file.

# Tools used
Tools used: nmap, hydra

[nmap] – at the first part of the script, the nmap tool was used to do active host discovery and port scanning. Next, the default nmap NSE “vuln” script was used to search for potential vulnerabilities in each active host.

[hydra] – the hydra tool was used to identify any available login service and brute force it.

# Possible Enhancements
Scope of the search for potential vulnerability could be expanded by using online databases, for example, scipag_vulscan resource. However, this would require a git clone to copy the repository into the user’s local directory.

User could be recommended a prepared list of password file templates, and the estimated time it might take to run the brute forcing. This allows the user to make a assessment weighing the scope, time and accuracy.

Multiple host & port scanning tools can be used to further enhance the accuracy of device & port scanning. For example, using nmap UDP scans as well as the massscan tool. However, this would greatly increase the time taken to complete the scan.
