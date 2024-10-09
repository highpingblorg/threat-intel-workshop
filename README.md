# Threat Intelligence workshop

## Overview

This workshop is designed to be a introductory *course* to the niche security topic - Threat Intelligence.

I am by no means an expert but I believe this is a step in the right direction, after all learning a topic practically is always best.

## Requirements

- Internet Connection
- A Virtual Machine - any OS will work, but for ease of use a Linux VM will work great
- Git - https://git-scm.com/downloads
- Docker Compose - https://docs.docker.com/compose/install/

## Workshop Labs

The labs in this workshop are arranged in an ascending order, where the complexity rises with each lab. There are a total of 3 labs:

1. Install and explore the tools and platforms
2. Identify the Threat Actor
3. Analyze a breach and document your threat intelligence using MISP and MITRE ATT&CK

## Set up process

1. Clone this repository:
```sh
git clone https://github.com/highpingblorg/threat-intel-workshop.git
```
2. Pull and rebase to fetch the MISP docker files

```sh 
git pull --rebase; git submodule --quiet sync; git submodule update --init --recursive --jobs 10
```
3. Pull and compose the Docker images
```sh 
docker compose up -d
```
4. Log in to MISP

Login: `admin@admin.test`

Password: `admin`

5. Fetch OSINT Feeds
After you successfully log in and update the password, you will be greeted with the Home page which is empty. We need to pull some events into MISP, for that we will use the OSINT feeds. To fetch them follow this route `Sync Actions>Feeds>Load Default Metadata`, after that press the checkbox to select all the feeds, after that is done press `Fetch and store all feed data`.

Now sit back and wait until all the events are pulled (this might take a while).
