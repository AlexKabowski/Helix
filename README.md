# HybridOS
An experimental, secure, and modular hybrid operating system built on the seL4 microkernel and a BSD-based layer

# Overview
HybridOS is an operating system project that aims to explore hybrid kernel architecture, combining the security and isolation of a microkernel with the familiarity and robustness of a Unix-like userland.

Our goal is to create an operating system foundation that is:

Secure: Using the seL4 microkernel, which is formally verified to be secure.

Modular: Built from isolated components (drivers, servers, etc.) using the CAmkES tool.

Compatible: Offering a BSD-like service layer, facilitating the portability of tools and applications.

# System Architecture
The system is built in layers, with a licensing strategy that reflects its modularity:

Foundation (Kernel): The seL4 microkernel (GPLv2). This layer is responsible for managing communication and security between components.

Service Layer: The service layer, which includes drivers, file servers, and essential libraries.

# Project Status
This project is in its early stages of development. Currently, the focus is on configuring the build environment, understanding the initialisation flow, and creating the first minimalist components with CAmkES.

# How to Contribute
Contributions are welcome! If you are interested in collaborating, please read the build instructions and code documentation. You can report bugs, suggest improvements, or submit pull requests.
