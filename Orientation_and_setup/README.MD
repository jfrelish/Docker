## Docker concepts
Docker is a platform for developers and sysadmins to build, share, and run applications with containers. The use of containers to deploy applications is called containerization. Containers are not new, but their use for easily deploying applications is.


* Containerization is increasingly popular because containers are:
* Flexible: Even the most complex applications can be containerized.
* Lightweight: Containers lerage and share the host kernel, making them much more efficient in terms of system resources than virtual machines.
*Portable: You can build locally, deploy to the cloud, and run anywhere.
*Loosely coupled: Containers are highly self sufficient and encapsulated, allowing you to replace or upgrade one without disrupting others.
*Scalable: You can increase and automatically distribute container replicas across a datacenter.
*Secure: Containers apply aggressive constraints and isolations to processes without any configuration required on the part of the user.

## Notes to self: Hyper v enable and disable from terminal:


* bcdedit /set hypervisorlaunchtype auto 
* bcdedit /set hypervisorlaunchtype off


## Install 

Install docker from [dockerhub](https://hub.docker.com/?overlay=onboarding)

# System Requirements: 


* Windows 10 64-bit: Pro, Enterprise, or Education (Build 15063 or later).
* Hyper-V and Containers Windows features must be enabled.
* The following hardware prerequisites are required to successfully run Client Hyper-V on Windows 10:
    64 bit processor with Second Level Address Translation (SLAT)
    4GB system RAM
    BIOS-level hardware virtualization support must be enabled in the BIOS settings. For more information, see Virtualization.
