# LMA

Log. Monitor. Act.

## Abstract

LMA aims to provide a way to monitor logs and take actions.

## Concepts

### Log Backends

A log backends is used to access a specific type of logs.
It is not specific to any log input. It just provide a
general way to access these kind of logs.

#### File

Reads logs from a simple logfile, as `/var/log/syslog`.

#### Journald

Reads logs from journald.

#### Docker

Reads logs from Docker logs.

### Log Sources

A log source is a configured instance of Log Backends for specific logs.

### Rules

A rule is a collection of regular expressions used to match events on
logs.

### Actions

An action is triggered when a rule is matched.
