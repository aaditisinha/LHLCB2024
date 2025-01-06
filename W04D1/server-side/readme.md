### CRON
```bash
@reboot /Your/path/to/server.py &
```
think `2>> cron_error.txt` instead
~~Optional
/dev/null 2>&1
 to run in silence, standard out and standard error to /dev/null~~
```
Here is the project folder structure 
```bash
┌──(root㉿kali)-[/home/student/Documents]
└─$ tree        
.
├── log_monitor_messages
│   └── log_monitor_messages.txt
├── log_storage
│   ├── access_logs
│   │   ├── standard_access.log
│   │   └── urgent_access.log
│   ├── error_logs
│   │   ├── standard_error.log
│   │   └── urgent_error.log
│   └── unknown_logs
│       └── standard_unknown.log
└── python_scripts
    ├── log_monitor_script
    │   └── access_log_monitor.py
    └── server_client
        ├── server.py
        └── triage.py
```

## resources
[Sample Access logs](https://www.ossec.net/docs/log_samples/apache/apache.html#log-samples-from-apache)
[Apache 2.4 (current) Docs](https://httpd.apache.org/docs/2.4/logs.html)
