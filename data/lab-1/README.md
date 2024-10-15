# Lab 1

This lab will be fairly simple, I won't make you do anything complex. It will be used as the prep for the next 2 labs.

## MISP

MISP is an open source software solution for collecting, storing, distributing and sharing cyber security indicators and threats about cyber security incidents analysis and malware analysis. MISP is designed by and for incident analysts, security and ICT professionals or malware reversers to support their day-to-day operations to share structured information efficiently.

MISP is regarded as the best platform for threat intelligence gathering, sharing and analysis. For that reason it will be one of the tools we will be using today. Luckily, we won't have to set it up from scratch, we will be using a Docker container.

### Set up process

1. Clone this repository:
```sh
git clone https://github.com/highpingblorg/threat-intel-workshop.git
```
2. Pull and rebase to fetch the MISP docker files

```sh 
git pull --rebase; git submodule --quiet sync; git submodule update --init --recursive --jobs 10
```
3. Enter the MISP directory
```sh
cd misp/
```
4. Pull and compose the Docker images
```sh 
docker compose up -d
```
5. Log in to MISP

Login: `admin@admin.test`

Password: `admin`

Now that you have logged into your own MISP instance - explore the tool, find all the different features. But you do have one main goal here, this step MUST be completed:

- Enable and fetch feeds from the OSINT feeds.

## GreyNoise

Greynoise is a platform that collects and analyzes Internet-wide scan and attack traffic. 

Your goals for this section are:

- Create an account on GreyNoise
- Browse through the different tabs and understand what each on is for

## VirusTotal

VirusTotal is a free online service that analyzes files and URLs to detect viruses, worms, trojans, and other kinds of malware using various antivirus engines and tools. Users can upload files or submit URLs to be scanned, and VirusTotal aggregates the results from multiple antivirus products and website scanners to provide a comprehensive report on the safety of the submitted item.

In addition to malware detection, VirusTotal also offers features like file and URL reputation analysis, community feedback, and the ability to search for previously scanned items. It is widely used by cybersecurity professionals, researchers, and individuals to assess the security of files and websites.

Your goals for this section are:

- Create an account on VirusTotal
- Explore the website a bit
- Look through different events on MISP and see if VirusTotal has more information on those IoC

## MITRE ATT&CK - The Adversarial Tactics, Techniques, and Common Knowledge

The MITRE ATTACK Framework is a curated knowledge base that tracks cyber adversary tactics and techniques used by threat actors across the entire attack lifecycle. The framework is meant to be more than a collection of data: it is intended to be used as a tool to strengthen an organization’s security posture.

For instance, because MITRE ATT&CK takes the perspective of the adversary, security operations teams can more easily deduce an adversary’s motivation for individual actions and understand how those actions relate to specific classes of defenses.

No account required for this website, I want you to explore the different Matrices, Techniques and Tactics.
