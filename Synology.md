Problem: Can't update or install packages. Comes back with this error.
`This package requires you to enable "pgsql-adapter.service"`

SOLUTION:

SSH into Synology NAS and run this. Might need to run it as super user

`systemctl start pgsql-adapter.service`

If it works, then run 
And check if it ok:
`"systemctl status pgsql-adapter.service"`

Most likely, you will get a follow up error that says 

PROBLEM: 

`database cannot start because drive space is insufficient synology`

Solution:
Clearing Log + restart doesn't work

Running this will show available space in volumes and synology system

`df -h`

` du -h` plus file path will show file sizes for that particular folder. 
example `du -h folder_name` If already in the folder of interest, 
just run the command without the folder_name

