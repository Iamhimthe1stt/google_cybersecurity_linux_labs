# Lab 1: Add and Manage Users with Linux Commands

## Objective
Add a new user, assign primary and secondary groups, change file ownership, then delete the user.

## Commands used
```bash
sudo useradd researcher9
sudo usermod -g research_team researcher9
sudo chown researcher9 /home/researcher2/projects/project_r.txt
sudo usermod -a -G sales_team researcher9
sudo userdel researcher9
sudo groupdel researcher9
```

## Troubleshooting
I typed `-a -g` instead of `-a -G` and got an error. `-g` sets the primary group, `-G` sets secondary groups, and `-a` only works with `-G`. Options are case-sensitive.

## Takeaway
Managing groups carefully and removing accounts promptly supports least privilege.

## Screenshots
![Error](screenshots/primary-group-and-error.png)
![Fixed](screenshots/secondary-group-fixed.png)
![userdel message](screenshots/userdel-expected-message.png)
![Cleanup](screenshots/groupdel-cleanup.png)
