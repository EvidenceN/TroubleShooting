Windows SSH: Permissions for 'private-key' are too open (also applicable to AWS SSH login to EC2 instance)
Potential Solution - https://superuser.com/questions/1296024/windows-ssh-permissions-for-private-key-are-too-open#:~:text=436-,You%20locate%20the%20file,-in%20Windows%20Explorer

Solution details is in this video - 

Solution quick short cut: `sudo chmod 600 file.pem` but only if the file is in a linux directory (think WSL). 
If the file is in windows directory that command won't work even if you are accessing the file from WSL with mnt/c/directory 
