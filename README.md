# Workstation

Reference for standing up a workstation for my use. This is generally OS agnostic.

## Software and Settings

I want to use:

### firefox

Make it default, simple home page (no distractions) and make it use private mode always. This is in "history" custom settings

### rclone

Use it to create a way to pull items from Google Drive, mainly my keepass database. My own client id and secret are available in Drive

After setting up "google" as the remote, try this for checking and syncing

```bash
# rclone sync [source] [destination]
# for example, to check and sync up to remote from local:
rclone check google/kpdb google:kpdb
rclone sync google/kpdb google:kpdb
```

### git

Set up to use SSH to enable simple editing of repos, default is fine. Log in using creds in keepass

### keepassxc 

Access the database when sync'd using rclone
