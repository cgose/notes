# Ubuntu Management

## Adding a new drive

> In my case I had a spare drive I wanted to add to my media server for extra storage.
> I installed it and formatted it using ubuntu-mate's disks application. After doing so 
> I could mount the drive, but it would mount with weird permissions

### Steps to adding drive correctly and permanently
- use blkid to get new drives UUID
- create a new mount point for the new drive
'''
sudo mkdir media/storage1
''
- edit /etc/fstab with su permissions
- add new drive with the UUID you got earlier
- Add the following to the fstab file with the correct values
'''
UUID= UUID-for-new-disk /media/storage1 filesystem(ext4)	defaults	0	0
'''
- Not sure what the defaults and the zeros mean will need to look that up.

