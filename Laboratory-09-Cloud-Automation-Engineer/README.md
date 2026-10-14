# Laboratory 09: The Cloud Automation Engineer

## Mission Overview
This laboratory activity focuses on using Bash scripting and cron jobs to automate backup operations in a Linux environment. The goal is to reduce manual work and protect important application data.

## Objectives
- Understand Bash scripting and variables.
- Create and execute a backup script.
- Manage script permissions using `chmod`.
- Schedule automatic backups using cron.
- Document the process in a GitHub portfolio.

## Commands Executed

```bash
mkdir app-data
echo "This is critical client data." > app-data/data.txt
nano backup.sh
chmod +x backup.sh
./backup.sh
ls -l backups/
crontab -l
env EDITOR=nano crontab -e
```

## Skills Learned
- Writing basic Bash scripts.
- Using variables to organize commands.
- Compressing files with `tar`.
- Changing executable permissions.
- Scheduling recurring tasks with cron.
- Documenting technical procedures using Markdown.

## Expected Output
The script creates a `backups` directory containing a compressed `.tar.gz` file. The cron configuration schedules the backup script to run every day at 2:00 AM.

## Screenshots
- `script-execution.png`
- `cron-schedule.png`
