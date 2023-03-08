
#script1.


LinuxStatus 	 
 navigate to the directory where it is saved and enter the following command:
        ./LinuxStatus.sh
The LinuxStatus script accepts command-line arguments to display the output of a specific option and exit. Here are the available arguments:

p: Displays the output of option 1 (list processes) and exits.

r: Displays the output of option 2 (memory status) and exits.

h: Displays the output of option 3 (hard disk usage) and exits.

a: Displays the output of option 4 (check Apache status) and exits.

Mix: You can use a combination of arguments, such as prah, to display the output of multiple options and exit.


To use these arguments, simply add them after the script name when running the script. For example, to display the output of option 1 and exit, you can run:
LinuxStatus p

display the output of options 1, 2, and 4 and exit, you can run:

LinuxStatus pra

Script 2: SimpleApacheApp
This script deploys a static web application.

How to Run
To run the script, navigate to the directory where it is saved and enter the following command:

./deploy_website.sh

Dependencies

Before running the script, you will need to make sure that Apache 2 is installed on your system.


Cronjob
To set up the cronjob to update the website daily at midnight, add the following line to your crontab file:

javascript
Copy code
0 0 * * * deploy_web.sh > /dev/null 2>&1
Replace /deploy_web.sh with the actual path to the script on your system.






