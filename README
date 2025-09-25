# ChartDB Service

This repository provides a systemd service configuration to run a local development server for ChartDB, a Node.js-based application. The service automates the startup of the ChartDB server in development mode using npm run dev, ensuring it runs reliably in the background and restarts automatically if it crashes.

## Prerequisites

Before setting up the systemd service, you need to clone the ChartDB repository and install its dependencies.

1. Clone the ChartDB Repository:

```bash
git clone https://github.com/chartdb/chartdb.git

```
Follow the Repository README

2. Node.js Installation: Ensure Node.js and npm are installed on your system. You can install them via a package manager or nvm (Node Version Manager). For example:

```bash
sudo apt update
sudo apt install nodejs npm
```

## Service Description

The chartdb.service is a systemd unit file that:

- Starts the ChartDB development server using npm run dev (or the equivalent Node.js command, such as node server.js).
- Runs the server under a dedicated user (chartdb) to enhance security.
- Automatically restarts the server in case of failure.
- Logs output to the systemd journal for easy debugging.

# Installation

1. Create the Service File: Create a file named chartdb.service in /etc/systemd/system/:

```bash
sudo vim /etc/systemd/system/chartdb.service
```

2. Add the Service Configuration: Copy and paste the following configuration into chartdb.service. Adjust paths and user as needed
3. Reload systemd: 

```bash
sudo systemctl daemon-reload
```

4. Enable the Service (to start on boot):

```bash
sudo systemctl enable chartdb.service
```

5. Start the Service:

```bash
sudo systemctl start chartdb.service
```

6. Find the url:

```bash
sudo systemctl status chartdb.service
#exemple : ➜  Local:   http://localhost:5173/
```



