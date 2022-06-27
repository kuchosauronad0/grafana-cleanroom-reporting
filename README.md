# grafana-cleanroom-reporting
These scripts will generate an email with images of grafana panels meant for weekly reports through a systemd-timer

| file | location | 
| ---  | -------- |
| grafana-cleanroom-reporting | /usr/local/bin/grafana-cleanroom-reporting |
| report.html | /usr/local/etc/grafana-cleanroom-reporting/report.html |
| grafana-cleanroom-reporting.service | /etc/systemd/system/grafana-cleanroom-reporting.service |
| grafana-cleanroom-reporting.timer | /etc/systemd/system/grafana-cleanroom-reporting.timer |

# Notes
* Grep for 'TODO:' and replace with whatever makes sense to you.
* There might be more changes needed depending on your grafana setup.
* The shell script has a limited debug functions to test pulling panel images called `basic_report` 


# Requirements:
* curl
* mutt
* grafana-image-renderer (needs to be available on the grafana server)
