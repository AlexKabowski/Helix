# HelixOS
An experimental, secure, and modular operating system built on the Linux 6.12 kernel, with principles from the seL4 microkernel.

# Overview
HelixOS is an operating system project that aims to exploit the Linux kernel architecture, combining the security and isolation of a microkernel with the familiarity and robustness of a Unix-like user environment.

Our goal is to create an operating system foundation that is:

Secure: using a combination of AppArmor, Capabilities, and Seccomp

Modular: built from isolated components (softwares and apps) using modules such as Namespace and Cgroup

Compatible: offering a service layer through Flatpak, facilitating the portability of tools and applications.

# System architecture
The system is built in layers, with a licensing strategy that reflects its modularity:

Foundation (Kernel): The Linux kernel (GPLv2). This layer is responsible for managing communication and security between components, as well as drivers and APIs.

Service layer: The service layer, which includes utility tools such as (shell, init, etc.) and other general-purpose programs (browsers, games).

Packaging: Use flatpak packaging technology; it is not yet defined whether there will be a package manager.

# Project status
This project is in its early stages of development. Currently, the focus is on setting up the build environment, understanding the startup flow, and creating the first minimalist components.