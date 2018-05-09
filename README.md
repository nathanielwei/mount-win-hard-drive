# Assess Windows dirve in Ubuntu  
## Error message  
### Unable to access “Data”
> Error mounting **/dev/sda7** at **/media/weizikai/Data**: Command-line `mount -t "ntfs" -o "uhelper=udisks2,nodev,nosuid,uid=1000,gid=1000" "/dev/sda7" "/media/weizikai/Data"' exited with non-zero exit status 14:   
> The disk contains an unclean file system (0, 0). Metadata kept in Windows cache, refused to mount. 
> Failed to mount '/dev/sda7': Operation not permitted  
> The NTFS partition is in an unsafe state.  
> Please resume and shutdown Windows fully (no hibernation or fast restarting), or mount the volume  read-only with the 'ro' mount option.

## Solution  
> sudo su  
> mount -t ntfs -o ro /dev/sda7 /media/weizikai/

## Reference  
[How To Mount Windows Drive In Unbuntu Linux]:https://www.youtube.com/watch?v=hIq1dIgZrOc  
by DevTech Solutions  
