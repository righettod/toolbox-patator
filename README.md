# 💻 Patator toolbox

[![Build and deploy the toolbox image](https://github.com/righettod/toolbox-patator/actions/workflows/build_docker_image.yml/badge.svg?branch=main)](https://github.com/righettod/toolbox-patator/actions/workflows/build_docker_image.yml) ![MadeWitVSCode](https://img.shields.io/static/v1?label=Made%20with&message=VisualStudio%20Code&color=blue&?style=for-the-badge&logo=visualstudio) ![MadeWithDocker](https://img.shields.io/static/v1?label=Made%20with&message=Docker&color=blue&?style=for-the-badge&logo=docker) ![AutomatedWith](https://img.shields.io/static/v1?label=Automated%20with&message=GitHub%20Actions&color=blue&?style=for-the-badge&logo=github)

## 🎯 Description

Toolbox to have a always up to date docker image of the tools named [Patator](https://github.com/lanjelot/patator).

## 📦 Build

> [!IMPORTANT]
> Currently the original dockerfile, is replaced by this [one](Dockerfile), due to this [issue](https://github.com/lanjelot/patator/issues/209) (Dockerfile was taken from the author of the issue).

The image is build every week and pushed to the GitHub image repository. You can retrieve it with the following command:

`docker pull ghcr.io/righettod/toolbox-patator:main`

## 👨‍💻 Usage

Use the following command from a PowerShell shell:

```powershell
PS> docker run -it --rm -v $pwd`:/work ghcr.io/righettod/toolbox-patator:main --help
Patator 1.1-dev (https://github.com/lanjelot/patator) with python-3.10.12
Usage: patator.py module --help

Available modules:
  + ftp_login     : Brute-force FTP
  + ssh_login     : Brute-force SSH
  + telnet_login  : Brute-force Telnet
  ...
```  

## 🤝 Sources & credits

* [Patator author](https://github.com/lanjelot/patator).
