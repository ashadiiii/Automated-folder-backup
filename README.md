Automated folder backup system

This automated system is created to build back-up directories of a specified directory in regular time intervals. The Automation system is created using the python language.

The following libraries were utilized in the program. 
- os library :  To interact with the operating system of the device and build a relavant file path to store our backup directories
- shutil :  To copy the files from the selected directory and then paste it in the backup directory
- datetime:  The backfolders are organised according to the date the backup was done. Hence in order to gain access to the date this library is used.
- schedule:  To assign a specific time to do the backup daily
- time:  To freeze the program for a given time limit
- sys:  To retrieve the source directory and destination directory through the terminal arguments

project description

The application assigns the source directory of where the backup should occur and destination directory which is where the back up is stored, into a 2 seperate variable. We then created a copy method that would copy the files in the source directory to the destination directory. The shutil copy tree method is used for this. When storing all the backup files for that specific day, it is stored under directory inside the destination directory. Each of these internal directories are named according the date of whenn the backup was done. A confirmation text would be sent once tthe back up is complete. 
One of the crucial aspects of the above application is to run the backup process only once a day. In order to achieve this we specify the time the backup should be donnen through the schedule library. 
