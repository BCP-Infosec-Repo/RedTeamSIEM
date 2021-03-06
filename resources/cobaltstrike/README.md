# Cobalt Strike Resources

## Aggressor Scripts

**Event Logging**

The *eventlogger.cna* script will log various Cobalt Strike events to an **events.log** file in the Cobalt Strike root directory. This log file is intended to be used with Filebeats.

**Web Logging**

The **apache-style-weblog-output.cna** script will log the Cobalt Strike native web log to a **weblog.log** file in the Cobalt Strike root directory. This log file mirrors the format used by Apache for its web logs is intended to be used with Filebeats. 

Note:This script was written by bluescreenofjeff.

## Shell Scripts

**Cobalt Strike Beats**

Configures Filebeat and Metricbeat on a Debian-based server. Filebeat will push the above two logs to the user-specified Elasticsearch host.

Usage: ./csbeat.sh <es_host> <cs_path>

- es_host = Elasticsearch host (ip)
- cs_path = Cobalt Strike path (/path/to/cs)

This script is meant to be used with the Elastic configuration generated by https://github.com/sadsfae/ansible-elk
