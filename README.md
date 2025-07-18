# HealthCheck CLI – Server Health Monitoring Tool

## Description
HealthCheck CLI is a user-friendly command-line utility written in Go. It allows DevOps and backend engineers to monitor their server's CPU, memory, disk, and network statistics efficiently. With options for real-time data display and logging, it simplifies server health checks.

## Tech Stack
- Go programming language
- gopsutil package for system metrics
- Standard Go libraries for CLI and file handling

## Installation
To use HealthCheck CLI, clone the repository and build the binary:

```bash
git clone https://github.com/bitasmbl/bitasmbl-healthcheck-cli-server-health-monitoring-tool.git
cd bitasmbl-healthcheck-cli-server-health-monitoring-tool

go build -o healthcheck
```

## Usage
```bash
./healthcheck [--cpu] [--log=filename.log]

Flags:
  --cpu     Display CPU usage stats
  --log   Log output to specified file
  --help    Show usage information
```

Example:
```bash
./healthcheck --cpu --log=server_log.txt
```

This command will display CPU stats and log the output to `server_log.txt`.

## Implementation Steps
- Initialize the Go project and set up command-line flags.
- Fetch system metrics using gopsutil.
- Display data in the terminal when flags are used.
- Write logs to a file if `--log` is specified.
- Package and build the binary for easy distribution.

When you are done, submit the project from your profile: [https://bitasmbl.com/home/profile](https://bitasmbl.com/home/profile)