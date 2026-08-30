## Mission Overview

This laboratory focused on investigating a Linux-based cloud environment and identifying the fundamental components of cloud infrastructure. The activity involved examining a cloud server, documenting its resources, researching major cloud providers, and designing a simple cloud infrastructure architecture.

## Objectives

The objectives of this laboratory were to:

- Investigate the configuration of a Linux cloud server.
- Identify compute, storage, networking, and operating system resources.
- Compare infrastructure services provided by AWS, Microsoft Azure, and Google Cloud Platform.
- Design a simple cloud infrastructure architecture.
- Practice technical documentation using Markdown and GitHub.

## Cloud Infrastructure Components

The main cloud infrastructure components identified during the laboratory were:

- *Compute:* The Linux environment uses an Intel Xeon E312xx processor with 1 CPU core.
- *Storage:* The environment has approximately 19 GB of disk capacity, with /dev/vda1 mounted as the main filesystem.
- *Networking:* The Linux environment has network connectivity and IP addresses including 172.30.1.2 and 172.17.0.1.
- *Operating System:* The environment runs Ubuntu 24.04.4 LTS with kernel version 6.8.0-138-generic.

## Tools Used

The following tools were used during the laboratory:

- KillerCoda
- Linux Terminal
- GitHub
- Markdown
- Draw.io / diagrams.net
- Web browser
- Microsoft Word for viewing the laboratory instructions

## Linux Commands Executed

The following Linux commands were used to investigate the cloud server:

```bash
cat /etc/os-release
uname -r
lscpu
nproc
free -h
df -h
hostname
hostname -I

## Skills Learned

During this laboratory, I learned how to investigate a Linux cloud environment using command-line tools. I learned how to identify CPU, memory, storage, networking, and operating system information. I also improved my understanding of cloud infrastructure services and learned how AWS, Microsoft Azure, and Google Cloud provide equivalent infrastructure services under different names. Additionally, I practiced using GitHub and Markdown to organize and document technical work.

## Challenges Encountered

One challenge was understanding the information returned by Linux commands and determining which values were relevant to the laboratory requirements. I also needed to understand the relationship between Linux resources and cloud infrastructure concepts. Creating and organizing the required Markdown files and screenshots in GitHub required careful attention to the folder structure and filenames. These challenges were addressed by reviewing the command output and documenting the results systematically.
