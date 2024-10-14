# Lab 2

The primary objective of this lab is to learn how to apply threat intelligence in an incident response scenario. Fortunately, this will be a straightforward example, so you won't need to analyze an .iso or a .pcap file to identify IoC.

In this lab, the IoC have already been identified; your task is to determine what is malicious about the IoC presented, albeit an IP or malicious file. Utilizing the tools from the previous lab or others discussed during the presentation, identify the Threat Actor associated with the following artifacts.

**PLEASE DOWNLOAD AND USE THESE FILES WITHIN A VM, SOME OF THE FILES ARE ACTUAL MALWARE**. Download the `.zip` file, the password is `infected`.

## Exercise 1

I accidentally downloaded and executed a weird `.exe`, it flashed red and I got scared and I unplugged my PC! Here is the file I downloaded, can you tell me what it is? 

Determine what file `1.exe`

## Exercise 2

The following IPs were doing some scary stuff on our infrastructure.. What were they trying to exploit?

```json
{
  "ips": [
    "110.152.70.140",
    "110.152.78.233",
    "112.43.108.134",
    "112.43.109.170",
    "8.218.168.197",
    "49.118.189.55",
    "49.118.191.140",
    "110.152.66.188",
    "112.43.108.189",
    "168.100.244.13"
  ],
  "metadata": {
    "total_ips": 10,
    "start_date": "2024-10-13T19:00:00Z",
    "end_date": "2024-10-14T19:00:00Z"
  }
}
```

## Exercise 3

Our Laravel application got hacked! Luckily, we found the IP address behind this breach, figure out what exploit could they have used to hack us! 

IP Address: `8.218.168.197`

## Exercise 4

No story for this one, who are the ~~morons~~ geniuses responsible for file 4?

## Exercise 5

Someone managed to create an insane **redacted**, find out:
- What that person managed to create
- Who that person is
- Who they might be associated to
- Where was this created
- Does this have a CVE ID
