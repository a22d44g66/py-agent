# py-agent

Python agent for running a user service. This supports automatic relaunching and automatic backup. Read the `config.sample.ini` for further details.

## Sample Usage

Consider the following `config.ini`:

`config.ini`:

```
[mspaint]
exec_dir = C:\Users\me\AppData\Local\Microsoft\WindowsApps
exec_name = mspaint.exe
exec_setup_script = sleep 2
backup_interval = 10
backup_target_dir = C:\test_server_data
backup_dest_dir = C:\Users\me
poll_interval = 3
exec_launch_cooloff = 5
```

`cmd`:
```
python py-agent.py mspaint
```
