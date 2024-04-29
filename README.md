## Kernel Source Package Builder
This repository contains GitHub Actions workflows to automate the building of Debian packages __.deb__ from a Linux kernel source 


## Workflow Overview
The workflow __deb.yml__ consists of several steps:

- Checkout repository: This step checks out the repository code to the runner.
- Install necessary packages: Installs required dependencies on the GitHub Actions runner.
- Get kernel source: Downloads the Linux kernel source from the official repository.
- Extract kernel source: Extracts the downloaded kernel source.
- Make configuration ARCH: Configures the kernel build for the desired architecture.
- Change var configuration: Modifies kernel configuration variables if necessary.
- Make kernel: Builds the kernel and generates Debian packages.
Additional Notes